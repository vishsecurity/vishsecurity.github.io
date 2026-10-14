# Building GovernanceGuard: A Local-First GRC Audit Workbench

Most GRC (Governance, Risk and Compliance) tools are heavy, expensive, and live in someone else's cloud. I wanted something different: a small audit workbench that runs on my own machine, keeps its data in a single SQLite file, and follows a real audit lifecycle instead of just being a pile of spreadsheets with a nicer font.

That project became **GovernanceGuard**.

> **Repo:** [vishsecurity/vishGRC.github.io](https://github.com/vishsecurity/vishGRC.github.io)

---

## What it is

GovernanceGuard is a browser-based GRC audit workbench backed by a Node.js/Express API and a persistent SQLite database. One dashboard covers:

- **Audit programs**: plans, workpapers, tests, and findings
- **Risk register**
- **Control register**
- **AI systems and AI risks**
- **Regulatory obligations**
- **Board reporting**, with a CSV snapshot export
- **Evidence attachments** on individual workpaper tests
- **User accounts and roles**

On first start it seeds clearly labeled *illustrative* records, so you can click around right away. They are examples to be replaced, not authoritative content.

---

## Why local-first?

Audit data is sensitive. A local-first design gives you:

1. **Control over where the data lives.** The database is `data/grc.sqlite`, and evidence files sit in `data/evidence/`.
2. **No accounts to create on a third-party service.**
3. **A small attack surface.** The server binds to loopback (`127.0.0.1`) by default and serves only the app page and the API, never project files, the database, or attachment storage.

---

## The audit workflow

The workbench is organized around a practical lifecycle informed by **ISO 19011**, the guidance standard for auditing management systems:

| Stage | What you record |
|---|---|
| **Initiate and plan** | Authority, objectives, scope, criteria, risk priorities, audit team, impartiality safeguards, dates |
| **Prepare** | Audit tests, sampling method and rationale, procedures, expected evidence |
| **Perform** | Workpaper results, evidence references, notes, tester |
| **Report** | Findings with criteria, condition, cause, impact, severity, and owner |
| **Follow up** | Due dates, corrective actions, retest and closure states with closure evidence |

The UI also surfaces the ISO 19011 auditing principles (integrity, fair presentation, due professional care, confidentiality, independence, and evidence-based and risk-based approaches) as quality prompts while you work.

**A note on scope:** ISO 19011 is *guidance for auditing*, not the criteria you audit against. For each engagement you enter the criteria that apply (an ISO management-system standard, a NIST framework, a regulation, a contract, or an internal policy). The project deliberately does not reproduce standard text or claim compliance, certification, or an audit opinion.

---

## Accounts, roles, and sessions

There is no default account and no public registration. On a fresh database, a one-time setup page creates the first administrator. It only accepts requests from the same machine and closes after the first account exists.

| Role | Can do |
|---|---|
| **Admin** | Manage settings, create and deactivate accounts, assign roles, reset passwords |
| **Editor** | Create and maintain GRC records, upload evidence |
| **Viewer** | Read-only |

Under the hood:

- Passwords are stored as **salted scrypt hashes**.
- Sessions use random opaque tokens, stored as **hashes** in SQLite, delivered in `HttpOnly`, `SameSite=Strict` cookies.
- Sessions expire after **eight hours**, and are revoked on sign-out, deactivation, or password reset.
- Sign-in attempts are **rate-limited** per process and client address.
- Inputs are validated server-side, and all SQL uses **parameterized queries**.

---

## Evidence handling

Evidence attaches to individual audit workpaper tests. PDF, PNG, JPEG, GIF, WebP, and common Word, Excel, and PowerPoint formats are accepted, up to 10 MB each. The server checks the extension, the declared media type, and basic file signatures. Files are stored outside the web root, and download and delete both require sign-in.

---

## Tech stack

- **Backend:** Node.js 20+, Express
- **Database:** SQLite (single file, easy to back up)
- **Frontend:** single-page HTML dashboard plus a sign-in page
- **Tests:** API integration tests covering persistence, validation, authentication, role restrictions, and the evidence lifecycle

Run it yourself:

```bash
git clone https://github.com/vishsecurity/vishGRC.github.io.git
cd vishGRC.github.io
npm install
npm start
# open http://127.0.0.1:3000 and create the admin account
```

Run the tests with `npm test`.

---

## Hosting it for free (and why GitHub Pages isn't enough)

The repo is named `*.github.io`, so the obvious idea is to host it on GitHub Pages. But GitHub Pages serves **static files only**. GovernanceGuard needs a running Node.js server and a writable disk for SQLite and evidence. For the full app, these are the realistic free-ish options:

1. **Your laptop.** Run `npm start`. To share on a trusted LAN, run `HOST=0.0.0.0 PORT=3000 npm start`. It's plain HTTP, so never use it on public Wi-Fi.
2. **A free-tier cloud VM with persistent disk**, such as Oracle Cloud Always Free where available. Run it behind Caddy for automatic HTTPS, with systemd to keep it alive and a dedicated non-root service account. Free-tier terms change, so check current availability.
3. **A static demo on GitHub Pages.** Ship a read-only build with sample data baked in. This is fine for showing what the UI looks like, but nothing persists.

Free container platforms with ephemeral disks are a poor fit. Restarts and redeploys can wipe the database and evidence.

---

## Honest limitations

This is a **prototype, not production software**. It does not have:

- Multi-factor authentication
- Email verification or self-service password recovery
- Encryption-at-rest management for evidence
- Malware scanning of uploads
- A tamper-proof audit trail
- Managed backups or retention policy
- Tenant isolation

So keep it on a trusted machine, don't put client-confidential evidence in it, and don't use it to make compliance decisions without a proper security and privacy review. HTTPS and a firewall alone don't change that.

Board figures are **live snapshots of the registers**, not historical trends. The app doesn't keep period-end snapshots, and it doesn't claim a change over time. The regulatory tracker and framework crosswalk are illustrative reference content, not authoritative guidance.

---

## What's next

Ideas on the roadmap:

- MFA and stronger password policy
- Period-end snapshots for real trend reporting
- Encrypted evidence storage and malware scanning
- Backup and restore tooling
- A static demo mode for GitHub Pages

Contributions, issues, and feedback are welcome on [GitHub](https://github.com/vishsecurity/vishGRC.github.io).

*Made by Vishal Chaudhary.*
