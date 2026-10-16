# How to Prepare for an ISO/IEC 27001:2022 Stage 2 Certification Audit: A Practical Operational Guide

A step-by-step guide for organizations starting from scratch and targeting a March 2027 certification audit

Preparing for an ISO/IEC 27001:2022 certification audit is not simply a matter of writing information security policies, creating a risk register, and collecting screenshots. An organization must establish an Information Security Management System (ISMS), implement the controls it determines are necessary, demonstrate that the system operates in practice, and evaluate whether it is effective.

For an organization with 51–250 employees, a cloud-based environment, one in-scope physical site, and a single GRC consultant available for 30 hours per week, preparation must be carefully planned. The consultant coordinates the project, but management, IT, HR, Procurement, Facilities and business owners must participate in implementation and provide evidence.

This guide explains how to organize the project, who to contact, what meetings to conduct, how to perform a physical site survey, how to request and validate evidence, how to track resources, and how to determine whether the organization is ready for Stage 2.

Planning assumption: The target is March 2027, with work starting on 19 October 2026. Stage 1 is scheduled but has not yet been completed. The actual Stage 2 date must be confirmed with the certification body after considering Stage 1 outcomes and implementation readiness.

## 1. Understand what Stage 2 certification means

ISO/IEC 27001:2022 specifies requirements for establishing, implementing, maintaining and continually improving an ISMS. A certification audit evaluates whether the organization meets the applicable requirements and whether the ISMS is implemented and operating effectively.

The certification process generally includes two stages.

| Audit stage | Primary purpose                                                                  | Preparation focus                                                                            |
| ----------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| Stage 1     | Review ISMS documentation, scope, readiness and other relevant arrangements      | Scope, policies, risk methodology, risk assessment, SoA, implementation status and readiness |
| Stage 2     | Evaluate implementation and effectiveness of the ISMS in the actual organization | Interviews, records, observations, technical evidence, control operation and conformity      |

Stage 1 is not a substitute for implementation. An organization cannot rely on a well-written set of policies if the actual processes, responsibilities and controls do not work.

For example, an access control policy may state that access is reviewed quarterly. During Stage 2, the auditor may ask to see the latest review, the list of accounts reviewed, the reviewer’s approval, identified exceptions and evidence that inappropriate access was removed.

The auditor may also interview the person responsible for the process and compare the explanation with the documented procedure and records.

The practical objective is therefore to make the ISMS documented, implemented, evidenced, reviewed and improved.

## 2. Establish project governance before creating artifacts

The first task is to establish who has authority to make decisions and who is responsible for implementing controls.

A GRC consultant can coordinate the work, identify gaps, map requirements, validate evidence and report progress. The consultant should not independently approve management policies, accept business risks, or claim that technical controls have been implemented when the relevant technical owner has not verified them.

### Recommended project roles

| Role                            | Main responsibility                                                                                       |
| ------------------------------- | --------------------------------------------------------------------------------------------------------- |
| Executive sponsor               | Approves direction, resolves resource conflicts and makes management decisions                            |
| ISMS manager or designated lead | Coordinates ISMS operation and ownership                                                                  |
| GRC consultant                  | Maintains project plan, registers, evidence requests, validation, reporting and audit coordination        |
| IT/cloud security lead          | Implements and evidences technical security controls                                                      |
| Business/process owners         | Identify information risks and implement controls within their processes                                  |
| HR                              | Provides evidence for recruitment, onboarding, awareness, role changes and offboarding                    |
| Procurement/vendor owner        | Manages supplier assessments, contractual requirements and supplier reviews                               |
| Facilities/admin                | Supports physical access, visitor management and site security                                            |
| Independent internal auditor    | Audits the ISMS with appropriate competence and independence                                              |
| Certification body              | Conducts the certification audits and makes the certification recommendation/decision through its process |

If the GRC consultant designs and implements the ISMS, an independent competent person should perform the internal audit of that work. The organization must plan for this resource early rather than treating independence as a last-minute requirement.

### Create the project repository

Create a controlled project folder with a structure such as:

```
ISO27001_2022_Project/
├── 01_Project_Governance/
├── 02_ISMS_Artifacts/
├── 03_Evidence_Restricted/
├── 04_Site_Survey/
├── 05_Risks_and_Gaps/
├── 06_Internal_Audit/
├── 07_Management_Review/
├── 08_Certification_Audit/
└── 09_Reports_and_Meeting_Minutes/
```

Restrict access to sensitive evidence. Avoid storing passwords, secret keys, authentication tokens or unnecessary personal information in the audit repository. Where evidence includes employee data, production information or security configurations, use the organization's approved secure storage and redaction process.

At kickoff, agree the project scope, roles, deadlines, communication channel, evidence repository and escalation rules.

## 3. Create the ISMS artifacts in the correct order

One of the most common project mistakes is creating a large collection of documents before understanding the organization. Start with the business, its information, its systems and its risks. Then create the documentation needed to govern and demonstrate the resulting controls.

ISO/IEC 27001:2022 requirements are primarily contained in Clauses 4–10. Annex A provides a reference set of controls that the organization evaluates when determining the controls necessary to treat its information security risks. The organization should not automatically implement or exclude every control without considering its risks and requirements.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://www.services.bis.gov.in\&sz=32)

Bureau of Indian Standards

+1



### Artifact creation and population plan

| Artifact                                | What to include                                                                                | Owner                           | Target date            |
| --------------------------------------- | ---------------------------------------------------------------------------------------------- | ------------------------------- | ---------------------- |
| ISMS project charter                    | Objectives, scope assumptions, responsibilities, milestones and governance                     | GRC + sponsor                   | 25 Oct 2026            |
| Context and interested parties register | Internal/external issues, stakeholder requirements and relevant obligations                    | GRC + business owners           | 1 Nov                  |
| ISMS scope statement                    | Services, locations, organizational boundaries, systems and interfaces                         | Sponsor + GRC                   | 8 Nov                  |
| Information security policy             | Management commitments, direction and responsibilities                                         | Sponsor + ISMS lead             | 8 Nov                  |
| Information security objectives         | Measurable objectives, owners, targets and review frequency                                    | ISMS lead + management          | 8 Nov                  |
| Asset and information inventory         | Information assets, systems, owners, classification and dependencies                           | IT + business owners            | 15 Nov                 |
| Risk assessment methodology             | Risk criteria, likelihood, impact, acceptance and assessment rules                             | GRC drafts; management approves | 22 Nov                 |
| Risk register                           | Risks, causes, consequences, existing controls, ratings, owners and treatment                  | Risk owners + GRC               | 29 Nov                 |
| Risk treatment plan                     | Treatment option, planned controls, owner, resources and due date                              | Risk owners + management        | 6 Dec                  |
| Statement of Applicability (SoA)        | Necessary controls, inclusion rationale, implementation status and exclusion justifications    | GRC + control owners            | 6 Dec initial version  |
| Control and evidence register           | Control owner, implementation status, evidence required, validation result and gaps            | GRC + control owners            | 13 Dec initial version |
| Operational control records             | Access reviews, supplier assessments, incidents, backups, changes and other applicable records | Relevant control owners         | Dec–Jan                |
| Internal audit programme and report     | Scope, criteria, methods, independence, findings and results                                   | Independent auditor             | 31 Jan target          |
| Corrective-action register              | Nonconformity, cause, correction, corrective action and effectiveness verification             | Control owners + ISMS lead      | Feb onward             |
| Management review record                | Required inputs, decisions, resource needs and improvement actions                             | Top management + ISMS lead      | 7 Feb target           |
| Audit evidence index                    | Requirement/control, evidence reference, owner, review period and retrieval path               | GRC                             | 21–28 Feb              |

These are project deadlines, not deadlines prescribed by the standard. Some artifacts will need updating as the scope, risk assessment, implementation and audit findings evolve.

### How to populate an artifact correctly

Take the asset inventory as an example. Do not start by creating a spreadsheet containing generic asset names. Ask the cloud owner and business owners to identify the actual systems and information used to deliver the in-scope services.

For each asset or service, capture:

- Unique asset ID and name.
- Business or technical owner.
- Business purpose and information processed.
- Hosting location or cloud provider/service.
- Classification and confidentiality, integrity and availability requirements.
- Dependencies, integrations and supplier relationships.
- Relevant risks and controls.
- Last review date and changes requiring reassessment.

Then validate the inventory with owners. A list of cloud services exported from a console is useful technical evidence, but it does not by itself establish business ownership, information classification or risk.

### How to build the risk register

Use a repeatable risk assessment method rather than writing generic risks such as “cyberattack” or “data breach.”

A practical risk record should describe:

1. Asset or process: what needs protection.
2. Threat and vulnerability: what could happen and why.
3. Consequence: potential effect on confidentiality, integrity, availability, legal obligations, customers or operations.
4. Existing controls: controls that actually operate today.
5. Inherent or current risk: assessed using the organization's approved method.
6. Treatment decision: modify, avoid, share or retain the risk, as appropriate to the methodology.
7. Control and action mapping: what must change, who will do it and by when.
8. Residual risk: risk remaining after treatment.
9. Approval: risk owner and authorized acceptance authority.

For example:

| Field             | Example                                                                         |
| ----------------- | ------------------------------------------------------------------------------- |
| Risk ID           | RISK-001                                                                        |
| Scenario          | A former employee retains access to an in-scope cloud service after leaving     |
| Potential impact  | Unauthorized access to business information                                     |
| Existing controls | Identity provider, access approval process, account deactivation procedure      |
| Gap               | No consistent evidence that all relevant accounts are disabled on exit          |
| Treatment         | Improve and test the leaver process; reconcile identity and cloud accounts      |
| Owner             | IT/cloud lead, with HR supporting notifications                                 |
| Evidence          | Sampled leaver records, deactivation timestamps, account reconciliation results |
| Closure test      | Sample shows timely deactivation and any exceptions have been resolved          |

This is an illustrative risk scenario, not a claim that the organization has this weakness.

### The relationship between risk treatment and the SoA

The SoA is not simply a copied Annex A checklist. Clause 6.1.3 requires the organization to determine necessary controls, compare them with Annex A to avoid omissions, document the SoA and prepare a risk treatment plan. The SoA records the controls considered necessary, their inclusion rationale, implementation status and justifications for excluding Annex A controls.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://www.services.bis.gov.in\&sz=32)

Bureau of Indian Standards

+1



The practical sequence is:

Risk assessment → risk treatment decisions → necessary controls → Annex A comparison → SoA → implementation → evidence → effectiveness review.

If a control is listed as implemented, verify that it is operating and supported by evidence. If it is not implemented, do not mark it complete merely because a policy or action plan exists.

## 4. Organize evidence collection as a controlled process

Evidence collection should be planned before the first request is sent. Otherwise, the project becomes a series of unstructured emails and last-minute document searches.

### Step 1: Create an evidence request register

Each request needs a unique identifier, for example `EV-0001`, and should record:

- Requirement or control reference.
- Exact evidence requested.
- System, process and period covered.
- Evidence owner and backup owner.
- Request date and due date.
- Secure repository location.
- Date received.
- Validation result.
- Exceptions, re-requests and closure status.

### Step 2: Ask for specific evidence

A weak request says:

> Please share access management evidence.

A stronger request says:

> Please provide the current user and privileged-account listing for the in-scope cloud environment, the latest access review with reviewer approval and exceptions, and a sample of approved access requests. Include the report-generation date and period covered. Share the files through the approved restricted repository by the agreed due date.

The second request is easier to fulfil, validate and audit.

### Step 3: Validate the evidence

For every item, ask five questions:

1. Authenticity: Is it from the actual system or authorized process?
2. Completeness: Does it cover the requested systems, people and period?
3. Relevance: Does it demonstrate the specific control or requirement?
4. Timeliness: Is it current enough for the purpose?
5. Effectiveness: Does it show that the control operated and exceptions were addressed?

For example, a screenshot of an access-control configuration can show that a setting exists at the time of capture. It may not prove that the setting was consistently applied, monitored or reviewed during the period.

Use configuration exports, dated reports, sampled records, workflow approvals, logs, test results and interviews as appropriate. Evidence must be proportionate to the control and the risk.

### Step 4: Track exceptions, not just receipts

If an owner sends a file that is incomplete, outdated or inconsistent, mark it as Exception identified or Re-requested, not accepted.

Record the gap, identify its owner, agree a due date, and retest after remediation. Maintain a clear distinction between:

- Evidence requested.
- Evidence received.
- Evidence validated.
- Control operating effectively.
- Gap corrected and independently verified.

This distinction is essential for credible audit readiness.

## 5. How to conduct the physical site survey

A cloud-based organization still has physical information security risks. Employees may use laptops, print documents, discuss confidential matters, access office networks or handle visitor information. The site survey should examine the controls relevant to the approved ISMS scope and the organization's actual risks.

### Before the visit

Schedule the survey with Facilities, IT and the site owner. Confirm authorization, permitted areas, escort arrangements and whether photographs or records may be collected.

Review the existing physical-security policy, visitor process, office layout and relevant incident records before visiting. Prepare a checklist so observations can be compared against the organization's documented requirements.

### During the visit

| Area               | What to inspect                                                                    | Evidence to request                                       |
| ------------------ | ---------------------------------------------------------------------------------- | --------------------------------------------------------- |
| Reception          | Visitor registration, identification and escort arrangements                       | Redacted visitor-log sample, visitor procedure            |
| Entry points       | Door access, badge issuance and access revocation                                  | Access permissions, badge-management records              |
| Restricted rooms   | Server/network rooms, equipment cabinets and other restricted areas                | Authorized-access list, inspection records                |
| Work areas         | Screen locking, unattended devices, printing and confidential information handling | Observation records, relevant procedure                   |
| Document disposal  | Disposal of printed confidential material and storage of records                   | Disposal process, approved service records where relevant |
| Physical incidents | Reporting and investigation of access or facility incidents                        | Incident records, response process                        |
| Equipment          | Protection of equipment and local infrastructure where applicable                  | Asset records, maintenance and inspection records         |

Not every item applies to every site. For a cloud-only production environment, for example, the organization may have no on-premises production server room. The survey should record that fact and examine the relevant remaining risks rather than inventing a control requirement.

### Record the observations

Use one record for each material observation.

| Field              | Example                                                        |
| ------------------ | -------------------------------------------------------------- |
| Survey ID          | SUR-001                                                        |
| Area               | Reception                                                      |
| Observation        | Visitor procedure exists; a sample of records needs validation |
| Evidence reference | EV-0042                                                        |
| Potential impact   | Visitor access may not be consistently evidenced               |
| Owner              | Facilities lead                                                |
| Action             | Review sample records and confirm process operation            |
| Due date           | 20 Nov 2026                                                    |
| Retest             | Pending                                                        |

Do not immediately classify every observation as a nonconformity. Validate the facts, identify the applicable requirement or internal procedure, and determine whether there is an actual gap. Any confirmed finding should be recorded and managed through the corrective-action process.

## 6. Meeting calendar: who to meet, when and why

A GRC consultant working 30 hours a week cannot spend every day in meetings. Meetings must produce information, decisions, evidence or actions.

### Weekly recurring calendar

| Day             | Activity                                                       | Time budget        | Participants                                          |
| --------------- | -------------------------------------------------------------- | ------------------ | ----------------------------------------------------- |
| Monday          | Plan priorities and review overdue actions                     | 1 hour             | GRC consultant                                        |
| Monday          | Weekly ISMS working meeting                                    | 45 minutes         | ISMS lead, IT/cloud lead, relevant owners             |
| Tuesday         | Discovery or control walkthrough                               | 2 hours            | Process owner and relevant technical/functional owner |
| Wednesday       | Evidence validation and gap review                             | 2 hours            | GRC and control owner as needed                       |
| Thursday        | Risk/control workshop or remediation follow-up                 | 2 hours            | Relevant control owners                               |
| Friday          | Sponsor status report and decision review                      | 30 minutes         | Sponsor and ISMS lead                                 |
| Throughout week | Evidence review, drafting, follow-ups, registers and reporting | Remaining capacity | As required                                           |

This is a template. During the internal audit, increase audit coordination time; during the Stage 2 audit, reserve capacity for auditor requests and interviews.

### Discovery meeting agenda

Run a 45–60 minute discovery meeting for each major function.

Ask:

1. What business processes does this team operate?
2. What information does it create, receive, store or share?
3. Which systems, applications, cloud services and suppliers does it depend on?
4. Who can access those systems, and how is access approved and removed?
5. What security risks or incidents has the team experienced?
6. Which controls operate today, and what records demonstrate their operation?
7. What is missing, who owns it and when can it be resolved?

Record the answers, assets, risks, evidence requests, owners and follow-up actions in the master workbook.

### Control walkthrough agenda

For access management, ask the IT owner to demonstrate the real process:

- An employee requests access.
- An authorized manager approves it.
- The access administrator provisions it.
- The request and approval are retained.
- Access is reviewed periodically.
- Changes and leavers trigger appropriate changes or removal.
- Exceptions are identified, escalated and resolved.

The walkthrough should be corroborated with samples of real records. A demonstration alone may not establish that the process operated consistently over time.

## 7. Email and follow-up process

Use a consistent communication process so control owners understand exactly what is required.

### Initial kickoff email



Dear Team,

We are commencing the ISO/IEC 27001:2022 ISMS implementation and preparation for the initial certification audit targeted for March 2027.

The immediate objective is to establish the ISMS scope, identify information security risks, assign control ownership, determine the required evidence and create a realistic implementation plan.

Please confirm the nominated owner for your function and identify any existing policies, risk assessments, inventories, audit reports, supplier assessments, security incidents or control records relevant to the proposed scope.

We will schedule short discovery meetings to understand the actual processes, systems, information and security controls. Evidence requests and actions will be recorded in a central tracker with assigned owners and due dates.

Please flag resource constraints, unavailable evidence or implementation dependencies early so that these can be addressed by the ISMS lead and sponsor.

Regards,\
GRC / ISMS Project Coordinator

### Evidence request email



Dear [Owner],

Please provide the following evidence for the agreed ISMS scope:

- [Specific report, record or configuration]
- [Relevant review period or sample]
- [Approval, exception or follow-up records, where applicable]

Request ID: [EV-ID]\
Evidence owner: [Name]\
Due date: [Date]\
Approved repository: [Secure location]

Please include the system or process name, relevant period and report-generation date. Do not email passwords, tokens, secret keys or unrestricted production data.

If the evidence is unavailable, please confirm the reason, the alternative evidence available and the expected delivery date. Missing evidence will be recorded for assessment rather than treated as complete.

Regards,\
GRC / ISMS Project Coordinator

### Follow-up cadence

| Timing                                                                  | Action                                     |
| ----------------------------------------------------------------------- | ------------------------------------------ |
| Day 0                                                                   | Send request and create the tracker record |
| Day 2                                                                   | Confirm the owner has received the request |
| Day 5                                                                   | Follow up and resolve questions            |
| Due date                                                                | Record receipt or missed deadline          |
| 1 working day overdue                                                   | Contact owner and identify the blocker     |
| 3 working days overdue                                                  | Escalate to the ISMS lead                  |
| 5 working days overdue, or sooner if a critical milestone is threatened | Escalate to the sponsor                    |
| Within 1–2 working days after receipt                                   | Validate evidence or request correction    |
| After remediation                                                       | Retest and record closure evidence         |

These are suggested project service levels, not timelines mandated by ISO/IEC 27001. Critical risks and imminent audit milestones require immediate escalation.

## 8. Master spreadsheet: how to track everything

Maintain a single workbook as the operational source of truth. Use unique IDs so emails, meeting minutes, risk records, evidence and corrective actions can be linked.

### Recommended workbook tabs

| Tab                        | Purpose                                   | Essential columns                                                                                                                   |
| -------------------------- | ----------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| `00_Dashboard`             | Overall progress and management reporting | Reporting date, overdue actions, high risks, evidence status, upcoming milestones                                                   |
| `01_Master_Actions`        | All implementation tasks and follow-ups   | ACT-ID, task, owner, priority, start date, due date, estimated hours, status, dependency, next action, escalation, closure evidence |
| `02_Evidence_Requests`     | Evidence request and validation           | EV-ID, control, evidence description, owner, requested date, due date, received date, validation status, exception, repository      |
| `03_Requirements_Controls` | ISO clauses and control mapping           | Clause/control ID, applicability rationale, owner, implementation status, evidence ID, effectiveness result, gap ID                 |
| `04_Risks_Gaps`            | Risk and deficiency management            | Risk/GAP-ID, scenario, cause, impact, rating, existing controls, treatment, owner, due date, residual risk, approval                |
| `05_Meetings_Decisions`    | Decisions and meeting actions             | Meeting ID, attendees, decision, decision owner, action ID, due date, minutes location                                              |
| `06_Site_Surveys`          | Physical site observations                | Survey ID, location, observation, evidence, potential impact, owner, action, retest                                                 |
| `07_Resource_Time`         | Workload and time budget                  | Week, workstream, planned hours, actual hours, remaining capacity, variance, reason                                                 |
| `08_Audit_Readiness`       | Final evidence and readiness review       | Requirement/control, evidence sufficiency, sample reference, internal audit result, gap status, readiness decision                  |

### Example action tracker

| ACT-ID  | Task                            | Owner             | Due date | Est. hours    | Status      | Closure criteria                       |
| ------- | ------------------------------- | ----------------- | -------- | ------------- | ----------- | -------------------------------------- |
| ACT-001 | Approve ISMS scope              | Sponsor           | 8 Nov    | 2 GRC hours   | In progress | Scope reviewed and approved            |
| ACT-002 | Complete cloud inventory        | IT/cloud lead     | 15 Nov   | 6 owner hours | Not started | In-scope services and owners validated |
| ACT-003 | Complete risk workshops         | GRC + risk owners | 29 Nov   | 10 GRC hours  | Not started | Risks reviewed and owners confirmed    |
| ACT-004 | Validate access-review evidence | GRC + IT          | 20 Dec   | 5 GRC hours   | Not started | Sample tested and exceptions recorded  |

The hours above are planning estimates, not actual time spent. Record the control owner's hours separately from your own.

### How to calculate completion

Do not use the number of documents created as the only measure of progress.

Track at least:

- Percentage of actions completed by their due dates.
- Percentage of evidence requests validated and accepted.
- Number of high risks without approved treatment.
- Number of open gaps past due.
- Percentage of applicable controls with assigned owners.
- Percentage of corrective actions retested and verified.
- Completion of internal audit and management review.
- Number of unresolved critical dependencies.

A control should not be marked effective merely because a policy exists. A policy may establish the requirement; operational records, sampling, interviews and testing help demonstrate whether the requirement is actually followed.

## 9. Resource-loaded schedule: 30 hours per week

For a single GRC consultant, 30 hours per week is approximately 150 hours over five weeks. The workload must be divided between project management, meetings, artifacts, evidence validation, remediation and reporting.

The following allocation is a baseline for your own time.

| Period          | Main focus                                                 | Weekly allocation                                                               |
| --------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------------- |
| Weeks 1–4       | Kickoff, discovery, scope, context, inventory              | 10h meetings/discovery; 8h documentation; 6h tracking; 6h follow-ups            |
| Weeks 5–8       | Risk assessment, treatment plan, SoA and evidence register | 8h risk workshops; 8h risk/SoA documentation; 8h owner follow-ups; 6h reporting |
| Weeks 9–12      | Control walkthroughs, site survey and evidence validation  | 6h meetings; 12h evidence validation; 6h gap tracking; 6h reporting             |
| Weeks 13–16     | Remediation, internal audit and management review          | 10h validation/retesting; 8h audit coordination; 6h meetings; 6h reporting      |
| Weeks 17–19     | Corrective action, readiness and final evidence index      | 12h validation; 6h follow-ups; 6h readiness review; 6h contingency              |
| Weeks 20 onward | Stage 2 audit support or rescheduled readiness work        | 15h audit support; 6h evidence retrieval; 4h issue tracking; 5h contingency     |

Adjust the weekly split as the project progresses. Do not treat this allocation as proof that the organization has enough total implementation capacity: technical engineering, policy approvals, employee training, access reviews and remediation require time from the relevant owners.

### Example: access review workload

A reasonable initial estimate for one access-management review might be:

| Task                                 | Your time |
| ------------------------------------ | --------- |
| Prepare request and confirm scope    | 1 hour    |
| Walk through process with IT         | 1 hour    |
| Review evidence and sample records   | 2 hours   |
| Discuss exceptions and track actions | 1 hour    |
| Retest closure                       | 1–2 hours |
| Total                                | 6–7 hours |

This estimate excludes the time IT spends exporting records, performing the review, removing access and fixing deficiencies.

## 10. Full project timeline from October 2026 to March 2027

The detailed schedule below puts the operating tasks and milestones into one view. Dates are targets, subject to the actual Stage 1 and Stage 2 arrangements.

| Week | Dates        | Key deliverables                                           |
| ---- | ------------ | ---------------------------------------------------------- |
| 1    | 19–25 Oct    | Kickoff, roles, tracker and initial information requests   |
| 2    | 26 Oct–1 Nov | Context, interested parties and scope draft                |
| 3    | 2–8 Nov      | Scope approval, policy, objectives and governance          |
| 4    | 9–15 Nov     | Asset inventory, cloud discovery and physical site survey  |
| 5    | 16–22 Nov    | Risk methodology and criteria                              |
| 6    | 23–29 Nov    | Risk register and owner validation                         |
| 7    | 30 Nov–6 Dec | Risk treatment plan and initial SoA                        |
| 8    | 7–13 Dec     | Control mapping, evidence register and gap prioritization  |
| 9    | 14–20 Dec    | Access management and asset-control evidence               |
| 10   | 21–27 Dec    | Cloud security, logging, vulnerability and change evidence |
| 11   | 28 Dec–3 Jan | Backup, recovery, continuity and incident evidence         |
| 12   | 4–10 Jan     | HR, supplier, physical security and information handling   |
| 13   | 11–17 Jan    | Control testing, evidence sampling and gap assignment      |
| 14   | 18–24 Jan    | Remediation, risk review and security metrics              |
| 15   | 25–31 Jan    | Independent internal audit                                 |
| 16   | 1–7 Feb      | Corrective-action planning and management review           |
| 17   | 8–14 Feb     | Retesting and updated risk/SoA records                     |
| 18   | 15–21 Feb    | Stage 1 follow-up and readiness review                     |
| 19   | 22–28 Feb    | Evidence validation and audit logistics                    |
| 20   | 1–7 Mar      | Stage 2, if confirmed for this period                      |
| 21   | 8–14 Mar     | Continued audit or findings follow-up                      |
| 22   | 15–21 Mar    | Further audit days or corrective-action evidence           |
| 23   | 22–28 Mar    | Certification-body follow-up or unresolved remediation     |
| 24   | 29–31 Mar    | Closeout and handover                                      |

This schedule is aggressive for an organization starting from scratch. If significant technical remediation is required, owners are unavailable, or Stage 1 identifies substantial concerns, the responsible decision is to revise the date or add resources—not to declare readiness without sufficient evidence.

## 11. Dependencies and escalation rules

The project schedule depends on management approvals, technical implementation, evidence availability and independent audit resources. These dependencies should be visible in the tracker.

| Dependency                               | Owner                             | Required outcome                                      |
| ---------------------------------------- | --------------------------------- | ----------------------------------------------------- |
| ISMS scope approval                      | Executive sponsor                 | Approved scope and boundaries                         |
| Cloud architecture and service inventory | IT/cloud lead                     | Validated systems, dependencies and owners            |
| Risk assessment participation            | Business and asset owners         | Risks assessed and treatment decisions assigned       |
| Risk treatment and SoA                   | Management + GRC + control owners | Approved treatment plan and consistent SoA            |
| Evidence collection                      | Each control owner                | Evidence delivered and validated                      |
| Technical remediation                    | IT/cloud and relevant teams       | Controls implemented and tested                       |
| Independent internal audit               | Management                        | Competent, sufficiently independent auditor appointed |
| Corrective-action closure                | Control owners                    | Root cause addressed and effectiveness verified       |
| Stage 1 findings and Stage 2 date        | Certification body + ISMS lead    | Confirmed readiness and audit arrangements            |

### Escalation matrix

| Trigger                                                 | Escalation                                                                       |
| ------------------------------------------------------- | -------------------------------------------------------------------------------- |
| Evidence is one working day overdue                     | Contact the evidence owner                                                       |
| Evidence is three working days overdue                  | Escalate to the ISMS lead                                                        |
| Evidence is five working days overdue                   | Escalate to the sponsor with options                                             |
| Critical risk has no owner or treatment plan            | Escalate immediately to the sponsor                                              |
| Technical fix requires additional budget or engineering | Request a management resource decision                                           |
| Internal audit independence is compromised              | Appoint an independent auditor                                                   |
| A corrective action fails retesting                     | Reopen the action and investigate the cause                                      |
| Stage 1 findings threaten the Stage 2 date              | Agree a recovery plan with management and coordinate with the certification body |
| An active security incident occurs                      | Invoke the organization's incident-response process immediately                  |

Every escalation should state the problem, business or audit impact, decision required, accountable owner and latest acceptable decision date.

Do not wait for the normal follow-up cycle when a critical risk, security incident or certification milestone is threatened.

## 12. Internal audit and management review

These are important readiness milestones, not administrative formalities.

### Internal audit

Clause 9.2 requires an internal audit programme and audits that evaluate conformity with the organization's own ISMS requirements and the standard, as well as implementation and maintenance effectiveness. The audit programme should address scope, criteria, methods, responsibilities, reporting and impartiality.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://studylib.net\&sz=32)

Information Security Management System

+1



Prepare an audit plan that covers:

- ISMS Clauses 4–10.
- The scope, risk assessment, treatment plan and SoA.
- Applicable controls and the evidence of their operation.
- Relevant business processes, cloud services and physical-site arrangements.
- Findings, objective evidence, corrective actions and reporting.

The auditor should sample records, interview staff and verify actual processes. A document review alone is not a sufficient test of operating effectiveness.

### Corrective actions

For each confirmed nonconformity, record:

1. The requirement and objective evidence.
2. Immediate correction or containment, where needed.
3. Root-cause analysis.
4. Corrective action to address the cause.
5. Accountable owner and deadline.
6. Evidence of implementation.
7. Verification that the action worked.
8. Any required updates to risk assessments, procedures or controls.

Do not close a corrective action just because the owner says the fix is complete. Verify the result.

### Management review

Top management must review the ISMS at planned intervals and retain evidence of the review and its results. The review should address relevant changes, performance, audit outcomes, objectives, nonconformities, corrective actions, risk assessment results, risk treatment status and opportunities for improvement.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://www.theiteh.com\&sz=32)

Information Security Management System

+1



The meeting should produce decisions and actions—not just a presentation. Examples include approving resources, addressing overdue risk treatment, revising objectives and resolving issues that prevent effective implementation.

## 13. Final Stage 2 readiness checklist

Use this as a practical go/no-go review before the audit.

## Readiness self-assessment

### 0/14

Check an item only when there is objective evidence that it is complete.

ISMS scope is approved and matches actual services, systems, interfaces and site arrangements.

Organizational context, interested parties and relevant legal, regulatory and contractual obligations have been considered.

Information security policy, objectives, roles and responsibilities are approved and communicated.

Asset inventory and risk assessment have been validated by the relevant owners.

Risk treatment decisions, SoA and treatment plan are consistent and approved by authorized personnel.

Applicable controls have been implemented and evidence shows how they operate.

Evidence requests, exceptions, open gaps and risks have assigned owners and deadlines.

Physical site survey has been completed and material observations have been followed up.

Internal audit has been performed with appropriate competence and independence.

Internal audit findings have documented corrective actions and verification status.

Management review has been completed and decisions are recorded.

Relevant employees can explain and demonstrate their responsibilities and processes.

Stage 1 concerns have been addressed sufficiently for the certification body to proceed.

Audit logistics, evidence retrieval, interview availability and technical demonstrations are ready.

14 items remain unchecked.

Copy readiness checklist

This checklist is a project-management aid, not an official certification-body readiness determination. The certification body makes the certification decision through its own process.

## 14. The most important lesson for a new GRC consultant

Your role is not to generate as many documents as possible. Your role is to establish a controlled operating process in which:

- Management owns the ISMS and makes the necessary decisions.
- Control owners implement and operate the controls.
- Evidence is requested, validated, linked to requirements and retained securely.
- Risks and gaps have owners, deadlines and closure tests.
- Internal audit independently evaluates conformity and effectiveness.
- Management reviews results and directs improvement.
- The certification auditor can trace the relationship between the organization's scope, risks, treatment decisions, controls and evidence.

A cloud-based organization can use provider reports, configuration exports, access records, change logs, incident records and restore-test evidence where appropriate. However, relying on a cloud provider does not automatically transfer all security responsibilities away from the organization. The organization must understand its supplier responsibilities and demonstrate how relevant risks are controlled.

### Authoritative and further reading

- [Bureau of Indian Standards — ISO/IEC 27001:2022 standard document](https://www.services.bis.gov.in/tmp/LITD23420436_29122022_1.pdf?utm_source=chatgpt.com) — check the current official edition and applicable amendments.
- [ISO/IEC 27001 Auditing Practices Group — Statement of Applicability guidance](https://committee.iso.org/files/live/sites/jtc1sc27/files/resources/ISO-IECJTC1-SC27-WG1_N3298_Auditing%20Practices%20Note%20-%20SoA.pdf?utm_source=chatgpt.com) — explains the relationship between necessary controls, Annex A and the SoA.
- [ISO/IEC 27001 Stage 1 and Stage 2 audit guide](https://sterling-grc.com/standards/iso-27001/stage-1-and-stage-2/?utm_source=chatgpt.com) — practical context on audit readiness, control sampling and evidence.

Recommended immediate action: start with the kickoff, nominate control owners, confirm the scope and certification-body schedule, and create the master action/evidence tracker. Do not wait until all policies are drafted before beginning discovery and evidence collection.
