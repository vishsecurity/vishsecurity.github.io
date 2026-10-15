# Why We Hear About ISO 27001 More Than HIPAA, HITRUST, DORA, CMMI, COBIT and COSO

If you work in security, compliance, or sales, you have probably noticed something. Customers, tenders, and vendor questionnaires keep asking, "Are you ISO 27001 certified?" Far less often do they ask, "Are you COSO compliant?" or "Do you hold a CMMI certificate for security?"

That is not because the other frameworks are weaker or less important. It is because they were built for different jobs. This post explains what each one actually is, and why ISO 27001 ended up as the name everyone knows.

## The short answer

ISO 27001 is the rare standard that is **international, industry-neutral, security-specific, and certifiable by an independent auditor**. Most of the others fail at least one of those four tests. They are either tied to one country or sector, aimed at a different problem (governance, finance, process maturity), or they are laws you must obey rather than badges you can earn.

## What ISO 27001 is

ISO/IEC 27001 is the international standard for an **Information Security Management System (ISMS)**. It does not just list technical controls. It asks an organization to build a repeatable management process: define scope, assess risks, choose controls, monitor, audit, and improve. The 2022 edition includes Annex A with 93 controls grouped into four themes (organizational, people, physical, technological).

Three things make it travel well:

- **Certifiable.** An accredited certification body audits you and issues a certificate, valid for three years with annual surveillance audits.
- **Global.** It is recognized in Europe, Asia, the Middle East, and the Americas, so one certificate answers many customers.
- **Any industry, any size.** A 20-person SaaS startup and a multinational bank can both certify.

A certificate is easy to put on a website, attach to a proposal, or reference in a contract. That portability is the main reason it dominates conversations.

## The others, and why they come up less

### HIPAA: a law, not a certificate

The Health Insurance Portability and Accountability Act is a **US law** protecting patient health information. Its Security Rule requires safeguards for electronic protected health information, but there is **no official HIPAA certification**. Anyone claiming to be "HIPAA certified" is usually referring to a vendor's own training or an assessment, not a government-issued credential.

You hear about HIPAA mainly if you touch US healthcare data. Outside that context, it is irrelevant. Inside it, it is mandatory, so it is discussed as an obligation rather than a differentiator.

### HITRUST: powerful, but narrower and costlier

HITRUST CSF is a **certifiable framework** that harmonizes requirements from ISO 27001, NIST, HIPAA, PCI DSS, and others into one control set. It is very well regarded in US healthcare, where many large providers and payers ask vendors for it.

Why it is mentioned less than ISO 27001:

- It is a **commercial framework** run by one organization, with assessment fees and a more prescriptive, heavier process.
- Its recognition is strongest in **US healthcare**. Outside that market, buyers rarely ask for it.
- Because it maps to ISO 27001, many organizations start with ISO and add HITRUST only when a healthcare customer demands it.

### DORA: a regulation for financial entities in the EU

The Digital Operational Resilience Act applies in the **European Union** and has been in force since January 2025. It covers banks, insurers, investment firms, and other financial entities, as well as their critical ICT service providers. It addresses ICT risk management, incident reporting, resilience testing, and third-party risk.

Like HIPAA, DORA is **mandatory law with no certificate**. You comply or you don't, and supervisors decide. It is a hot topic right now, but only for a defined group of regulated firms and their suppliers. Many organizations use ISO 27001 as a foundation that supports DORA readiness, though it does not by itself make you compliant.

### CMMI: about process maturity, not security

The Capability Maturity Model Integration is a **process improvement model**, originally from software engineering. It rates how mature your processes are, from ad hoc to optimized. CMMI does have appraisals and maturity levels, but it is not a security standard. It is common in software delivery and government contracting in some regions, especially for IT services exports.

So it comes up when buyers care about **delivery quality**, not when they care about **data protection**. Different question, different framework.

### COBIT: governance for IT management

COBIT, from ISACA, is a framework for **governance and management of enterprise IT**. It helps boards and executives align IT with business goals, manage risk, and measure performance. Security is one part of it, not the whole point.

COBIT is mostly an internal tool used by CIOs, auditors, and risk teams. It is **not typically certified at the organization level**, so it rarely appears on customer questionnaires. It also pairs well with ISO 27001 rather than competing with it.

### COSO: internal control and enterprise risk

COSO publishes frameworks for **internal control** and **enterprise risk management**. Its Internal Control framework is the backbone of financial reporting controls, especially for US-listed companies under Sarbanes-Oxley. Auditors use it constantly.

But it is about financial and operational control, not information security specifically, and there is **no COSO certificate**. Customers do not ask vendors for it. Finance and audit teams care about it instead.

### SOC 2 Type 2: the closest rival, but an audit report rather than a certificate

SOC 2 comes from the AICPA, the US accounting body. A licensed CPA firm examines your controls against the Trust Services Criteria: security, availability, processing integrity, confidentiality, and privacy. **Type 1** reports on whether controls are designed properly at one point in time. **Type 2** reports on whether they **worked in practice over a period**, commonly 3 to 12 months, so buyers trust it more.

SOC 2 Type 2 is the one most likely to compete with ISO 27001 in a questionnaire, especially for US SaaS and cloud vendors. It is mentioned less globally because:

- It is an **attestation report**, not a certificate. The report is long, usually shared under NDA, and has to be read rather than glanced at.
- It is **strongest in North America**. Outside the US, buyers tend to ask for ISO 27001 first.
- The scope and criteria are chosen by the company, so two SOC 2 reports can differ a lot.

Many vendors end up holding both, since the control work overlaps heavily.

### TISAX: a passport for the automotive supply chain

TISAX (Trusted Information Security Assessment Exchange) is run by the ENX Association on behalf of the German automotive association VDA. Assessments are done against the **VDA ISA catalog**, which is built on ISO 27001 controls and adds automotive-specific topics such as prototype protection and data protection. Results are shared through the ENX portal as an assessment label that partners can check.

It is rarely mentioned outside one industry because it is **sector-specific**. If you supply German car makers or their tier-1 suppliers, TISAX is effectively required, and ISO 27001 knowledge helps you get there. For everyone else, it never comes up.

### ITGRC: a discipline and a tool category, not a standard

ITGRC stands for IT Governance, Risk and Compliance. It describes an **approach**, and a family of software platforms, for managing IT policies, risks, audits, and regulatory obligations in one place. It does not define requirements of its own, and there is no ITGRC certificate.

That is why it appears in job titles and tool comparisons but not in customer contracts. ITGRC is how you run ISO 27001, SOC 2, or DORA work day to day, not a framework you are measured against.

### ITAC: controls inside the application, an auditor's term

ITAC usually means IT Application Controls: checks built into a business application, such as input validation, calculation accuracy, approval workflows, and access rights inside an ERP or billing system. They sit alongside IT General Controls (ITGC), which cover the environment around the applications, like access management and change management. (If you meant a different ITAC, tell me and I will adjust this section.)

This is **audit vocabulary**, used mainly in financial statement audits and SOX testing, usually together with COSO. It is not a standard and has no certificate, so customers do not ask for it. Auditors do.

### NIST SP 800-53: the US government's control catalog

NIST Special Publication 800-53 (currently Revision 5) is a large catalog of security and privacy controls, organized into control families and applied through low, moderate, and high baselines. It was written for **US federal information systems**, and it underpins programs such as FISMA and FedRAMP.

It is a free publication, not a certifiable standard. No body issues a "NIST 800-53 certificate"; federal agencies grant their own authorization to operate, and FedRAMP authorizes cloud services for government use. That is why you hear about it from US government contractors and cloud providers, but rarely in commercial questionnaires. Because NIST publishes mappings to ISO 27001, many organizations use the two together.

### NIST SP 800-61: an incident response guide, not a compliance scheme

NIST SP 800-61 is the guide to **computer security incident handling**: preparing for incidents, detecting and analyzing them, containing and recovering, and learning afterward. The latest revision (Revision 3, 2025) ties incident response into the NIST Cybersecurity Framework 2.0 rather than treating it as a standalone process.

It is **guidance**, so there is nothing to certify. Security teams lean on it to build playbooks, while auditors and regulators may ask whether you follow a recognized incident response approach. ISO 27001 sits above it: the standard requires an incident management process, and 800-61 is one good way to build it.

### PCI DSS 4.0.1: a contractual standard for card data

The Payment Card Industry Data Security Standard is maintained by the PCI Security Standards Council and applies to any organization that stores, processes, or transmits **payment card data**. Version 4.0.1, published in 2024, is the current version. It replaced 4.0, which was retired at the end of 2024, and its newer "future-dated" requirements became mandatory on 31 March 2025.

PCI DSS is neither a law nor an ISO-style certificate. It is enforced through **contracts with card brands and acquiring banks**, and compliance is validated by a Qualified Security Assessor or a self-assessment questionnaire, depending on volume. The outcome is an Attestation of Compliance.

It stays out of general security conversations because it is **narrow by design**: it protects cardholder data, not the whole organization. If you take card payments you must comply, whatever else you hold. ISO 27001 helps with the management system around it, but does not replace PCI DSS.

### EU AI Act: a new regulation for AI systems

The EU AI Act (Regulation (EU) 2024/1689) regulates AI by risk level, from banned practices to high-risk systems to simple transparency duties. It applies to providers and deployers whose AI is placed on the EU market or used in the EU, wherever they are based.

It is a **law with a phased timeline**, and there is no certificate for the Act as a whole. Obligations for general-purpose AI models have applied since August 2025. Under the Digital Omnibus on AI, which entered into force in mid-2026 according to [K&L Gates](https://www.mondaq.com/eu-digital-omnibus-on-ai-enters-into-force/1825722), stand-alone high-risk obligations moved from 2 August 2026 to 2 December 2027, and those for AI embedded in regulated products to 2 August 2028. Check the official text before relying on these dates.

It is not yet a daily topic because the heaviest duties are still ahead and it covers AI specifically. The ISO sibling you may hear about is ISO/IEC 42001, a certifiable AI management system standard that follows the same management-system logic as ISO 27001, and many companies use it to prepare.

## Side-by-side view

| Framework | Type | Scope | Certifiable? | Typical audience |
| --- | --- | --- | --- | --- |
| ISO 27001 | International standard | Information security management | Yes | Any industry, worldwide |
| HIPAA | US law | Health data privacy and security | No | US healthcare and their vendors |
| HITRUST | Commercial framework | Security and privacy, harmonized | Yes | Mainly US healthcare |
| DORA | EU regulation | Digital operational resilience | No | EU financial entities and ICT providers |
| CMMI | Maturity model | Process capability | Appraisal rating | Software and IT delivery |
| COBIT | Governance framework | Enterprise IT governance | Not typically | CIOs, boards, auditors |
| COSO | Control framework | Internal control and ERM | No | Finance, audit, SOX |
| SOC 2 Type 2 | Audit report (AICPA) | Trust Services Criteria, tested over a period | Report, not a certificate | Mainly US SaaS and cloud vendors |
| TISAX | Industry assessment (ENX/VDA) | Automotive information security (VDA ISA) | Yes, assessment label | Automotive supply chain |
| ITGRC | Discipline and tooling | IT governance, risk and compliance management | No | Risk, compliance and IT teams |
| ITAC | Audit concept | Controls inside business applications | No | Auditors, SOX teams |
| NIST SP 800-53 | US government control catalog | Security and privacy controls for information systems | No (agency authorization, FedRAMP) | US federal agencies and contractors |
| NIST SP 800-61 | Guidance | Incident response | No | Security and incident response teams |
| PCI DSS 4.0.1 | Industry standard, contractually enforced | Payment card data protection | Validated by assessor or self-assessment | Merchants, processors, service providers |
| EU AI Act | EU regulation | Risk-based rules for AI systems | No (conformity assessment for high-risk AI) | AI providers and deployers in the EU market |

## Why ISO 27001 wins the conversation

1. **It answers the trust question directly.** Buyers want proof that a vendor protects information. A third-party certificate is faster to evaluate than a long questionnaire.
2. **It is portable.** One certificate works across countries and sectors, so it scales commercially.
3. **It is a foundation.** Its risk-based ISMS maps well to HIPAA, DORA, HITRUST, SOC 2, and others, so it often becomes the first building block.
4. **It is specific to security.** CMMI, COBIT, and COSO solve adjacent problems. They are not wrong, just not the question being asked.
5. **It is visible.** Public certificate registers and logos make it easy to mention in marketing, procurement, and RFPs.

## The takeaway

These frameworks are not rivals. They sit at different layers:

- **Laws and regulations** (HIPAA, DORA, EU AI Act) and contractual standards (PCI DSS) tell you what you must do.
- **Governance and control frameworks** (COBIT, COSO) and audit practices (ITGRC, ITAC) tell leadership how to oversee and control.
- **Maturity models** (CMMI) tell you how well your processes run.
- **Certifiable security standards** (ISO 27001, HITRUST, TISAX) and audit reports (SOC 2 Type 2) let you prove to others that your security program works.

Underneath all of these sit technical catalogs and guides such as NIST SP 800-53 and 800-61, which give security teams detailed controls and playbooks but no certificate to show customers.

We hear about ISO 27001 most because it is the one that **proves security to strangers**, anywhere in the world. The right choice for your organization depends on your market, your regulators, and who is asking. Many mature companies end up with several of these working together, with ISO 27001 as the common core.
