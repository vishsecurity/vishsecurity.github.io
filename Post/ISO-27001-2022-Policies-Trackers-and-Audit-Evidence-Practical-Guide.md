# How to Create ISO 27001:2022 Policies, Trackers and Audit Evidence: A Practical Guide for GRC Consultants

## Introduction

One of the most common challenges in ISO/IEC 27001:2022 implementation is understanding how to convert a standard or regulatory requirement into a working organizational process.

A consultant may know that access rights must be managed, risks must be assessed, suppliers must be monitored and incidents must be recorded. However, knowing the requirement is only the first step. The real work is determining:

- What does the requirement mean for the organization?
- What policy or procedure is needed?
- What tracker or register should be created?
- Who is responsible for populating and maintaining it?
- What evidence demonstrates that the control operates?
- How will the auditor verify its effectiveness?

This blog explains a practical, repeatable method for creating ISO 27001:2022 policies, trackers and supporting evidence, using access control as a worked example.

## 1. Understand the Difference Between a Requirement, a Policy, a Tracker and Evidence

Before creating documents, distinguish between four related but different components.

### Requirement

A requirement establishes what the organization must achieve or demonstrate. It may originate from an ISO clause, an applicable Annex A control, a regulatory circular, a contractual obligation or an internal risk decision.

### Policy

A policy defines management's direction, principles and mandatory rules. It explains what the organization expects people to follow.

### Tracker or register

A tracker records the operational details needed to implement, monitor and manage a process. It may contain owners, dates, decisions, exceptions, deadlines and closure status.

### Evidence

Evidence demonstrates what actually happened. Examples include approved access requests, system exports, review records, change tickets, meeting minutes and screenshots collected with appropriate authorization.

Consider access management:

| Component   | Example                                                              |
| ----------- | -------------------------------------------------------------------- |
| Requirement | Access rights must be managed appropriately                          |
| Policy      | Access Control Policy                                                |
| Procedure   | User provisioning and access review procedure                        |
| Tracker     | User Access Review Tracker                                           |
| Evidence    | Access export, review decisions and completed access-removal tickets |
| Validation  | Check whether identified inappropriate access was actually removed   |

These components work together, but they are not interchangeable. A policy does not prove that a process was followed, and a tracker containing a status of “Completed” does not prove that the underlying action occurred.

## 2. Start With the Source Requirement

The first step is to identify the exact source of the requirement.

For an ISO 27001 project, the source may be:

- Clauses 4–10 of ISO/IEC 27001:2022.
- Annex A controls considered necessary through the risk treatment process.
- Applicable legal or regulatory requirements.
- Customer or contractual security requirements.
- Internal risk treatment decisions.

For a regulatory circular, record the regulator, circular reference, issue date, effective date, paragraph number and applicability to the organization.

Do not begin by downloading a generic policy template. First establish what the source requires and whether it applies to the organization's ISMS scope.

### Example: Access rights

ISO/IEC 27001:2022 Annex A control 5.18 concerns access rights. The exact control wording should be verified against a licensed copy of the standard.

A consultant should then determine:

1. Which systems and information are covered?
2. Who authorizes access?
3. How are permissions granted and changed?
4. How are access rights reviewed?
5. What happens when an employee leaves?
6. How are exceptions documented?
7. What evidence will demonstrate that the process operates?

These questions translate the source requirement into an implementation plan.

## 3. Convert the Requirement Into a Control Objective

A control objective describes the outcome the organization wants to achieve.

For access rights, a practical control objective could be:

**Ensure that access to organizational systems and information is authorized, appropriate to business responsibilities, periodically reviewed and revoked when no longer required.**

This objective gives the consultant a clear direction for designing the policy, procedure, tracker and validation tests.

A useful control specification includes:

| Field                      | Description                                              |
| -------------------------- | -------------------------------------------------------- |
| Requirement reference      | ISO clause, Annex A control or regulatory paragraph      |
| Requirement interpretation | What the requirement means in the organization's context |
| Control objective          | The intended security or compliance outcome              |
| Applicability              | Why the requirement applies or does not apply            |
| Control owner              | Person accountable for the control                       |
| Operating team             | Team responsible for execution                           |
| Frequency                  | When the activity must occur                             |
| Required records           | Documents and evidence to retain                         |
| Validation method          | How the consultant or auditor will test operation        |

The frequency and approval requirements should be defined based on the standard, applicable regulation, risk assessment and organizational decisions. Avoid presenting arbitrary timeframes as universal ISO requirements.

## 4. Create the Policy

A policy converts the control objective into approved organizational rules.

A typical policy structure includes:

1. Document control and approval.
2. Purpose.
3. Scope.
4. Definitions, where necessary.
5. Policy requirements.
6. Roles and responsibilities.
7. Exceptions and escalation.
8. Records and evidence.
9. Compliance monitoring.
10. Review and approval.

### Example: Access Control Policy

The policy might require that:

- Access must be approved before provisioning.
- Permissions must be appropriate to assigned responsibilities.
- Privileged access must be restricted and traceable.
- Authentication controls must be appropriate to risk.
- Access must be changed when responsibilities change.
- Access must be revoked when it is no longer required.
- Access rights must be reviewed at the organization's defined frequency.
- Exceptions must have documented justification, approval and review.
- Records must be retained in approved repositories.

These are illustrative policy provisions. They must be tailored to the organization's technology, risks, applicable obligations and actual operating processes.

### Validate before approval

A policy should not describe a process that the organization cannot perform or has not agreed to implement.

For example, if the policy requires quarterly access reviews, the consultant should confirm that system owners can obtain access listings, perform the reviews and complete remediation at that frequency.

The policy should be reviewed by the responsible stakeholders and approved by an authorized management representative. Its publication and communication should also be recorded.

## 5. Create the Tracker

Once the policy defines what must happen, the tracker records whether it happened.

For access control, the organization may need a user access inventory, an access review tracker or both. The design depends on the process and the systems involved.

A practical User Access Review Tracker could contain:

| Field             | Purpose                                          |
| ----------------- | ------------------------------------------------ |
| Review ID         | Unique reference for the review record           |
| Review period     | Period covered by the review                     |
| System name       | Application, cloud platform or service           |
| User ID           | Unique identifier for the account                |
| Assigned role     | Role or permission level                         |
| Business owner    | Person accountable for the business access       |
| Reviewer          | Person performing the review                     |
| Review date       | Date of the review                               |
| Decision          | Retain, modify or revoke                         |
| Exception details | Description of inappropriate or uncertain access |
| Action ID         | Reference to the remediation action              |
| Action owner      | Person responsible for resolving the issue       |
| Due date          | Agreed completion deadline                       |
| Closure evidence  | Record demonstrating the change                  |
| Verified by/date  | Person and date of closure validation            |
| Status            | Current review or remediation status             |

The tracker should support the organization's actual workflow rather than merely act as a list of names.

### Sample tracker records

The following records are fictional examples for demonstrating the design.

| Review ID | System               | User   | Decision | Action   | Status          |
| --------- | -------------------- | ------ | -------- | -------- | --------------- |
| UAR-001   | Cloud Console        | U-1001 | Retain   | None     | Reviewed        |
| UAR-002   | Business Application | U-1002 | Modify   | ACT-0041 | Open            |
| UAR-003   | Cloud Console        | U-1003 | Revoke   | ACT-0042 | Pending removal |

These sample records must not be presented as actual audit evidence. In a live ISMS, the tracker must be populated using authorized system data and real review decisions.

## 6. Populate the Tracker Using Real Information

Creating the spreadsheet is not the same as implementing the control. The next step is obtaining reliable information from the teams that operate the process.

For an access review:

**Step 1: Request the source data.** Obtain the current user and permission export from the system owner or administrator.

**Step 2: Confirm completeness.** Establish which systems, account types and privileged accounts are included in the review.

**Step 3: Assign the reviewer.** The appropriate business or system owner should determine whether the access remains justified.

**Step 4: Record the decision.** Each reviewed account should have a traceable decision, reviewer and date.

**Step 5: Create actions.** Inappropriate access should be assigned to a responsible person with a target completion date.

**Step 6: Verify the result.** Check the updated system record or approved change ticket to confirm that the access was actually modified or removed.

The GRC consultant coordinates this process, challenges incomplete records and validates evidence. The consultant should not approve access on behalf of an accountable business owner unless that responsibility has formally been assigned.

## 7. Define the Evidence Requirements

Evidence must be sufficient to demonstrate that the control was implemented and operated.

For access management, evidence may include:

- An access export showing the relevant accounts and permissions.
- Approved access requests.
- Review records identifying the reviewer and decisions.
- Provisioning or deprovisioning tickets.
- Records showing that exceptions were resolved.
- Relevant system records demonstrating the final access state.

Evidence should be authentic, relevant, complete and appropriate to the period being tested.

A screenshot alone may not be enough if it lacks context, a date, system identification or a link to the control being tested.

Evidence should be stored in an approved repository with appropriate access restrictions. Passwords, authentication tokens, private keys and other secrets should never be collected merely to demonstrate that a control exists.

## 8. Test Whether the Control Is Effective

The consultant should not stop after creating the policy and tracker. The next step is to test the operation of the control.

An access review test might ask:

| Test               | What to check                                                              |
| ------------------ | -------------------------------------------------------------------------- |
| Authorization      | Was access approved by the appropriate person?                             |
| Appropriateness    | Does the assigned role match the user's responsibilities?                  |
| Completeness       | Does the review cover the defined systems and accounts?                    |
| Frequency          | Was the review performed according to the organization's defined schedule? |
| Exception handling | Were inappropriate permissions recorded and assigned for action?           |
| Remediation        | Was access actually modified or revoked?                                   |
| Traceability       | Can the reviewer, decision, action and closure evidence be linked?         |

For example, if a review identifies an administrator account that is no longer required, the consultant should trace the record from the review decision to the remediation ticket and then verify the account's final state.

If the tracker says “Closed” but the access remains active, the issue is not resolved merely because the spreadsheet has been updated.

The consultant should document the exception, identify the responsible owner, agree on corrective action and retest the control after remediation.

## 9. Map the Artifacts to ISO 27001:2022

The policy, tracker and evidence should be mapped to the relevant requirements.

For the access control example, possible references include:

| ISO reference | Relevance                                        |
| ------------- | ------------------------------------------------ |
| Clause 7.5    | Control of documented information                |
| Clause 8.1    | Operational planning and control                 |
| Clause 9.1    | Monitoring, measurement, analysis and evaluation |
| Annex A 5.15  | Access control                                   |
| Annex A 5.16  | Identity management                              |
| Annex A 5.17  | Authentication information                       |
| Annex A 5.18  | Access rights                                    |
| Annex A 8.2   | Privileged access rights                         |
| Annex A 8.3   | Information access restriction                   |

This is an initial mapping, not a declaration that every listed control is automatically applicable. The organization must determine the necessary controls through its risk treatment process and document its decisions in the Statement of Applicability (SoA).

The broader implementation should also connect to:

- **Risk assessment:** What can go wrong, and how significant is the risk?
- **Risk treatment plan:** What actions will reduce the risk?
- **SoA:** Which controls are necessary, and why?
- **Control register:** Who operates each control and how?
- **Evidence register:** What records demonstrate operation?
- **Corrective-action register:** How are deficiencies resolved?

This creates traceability from risk and requirements to implementation and audit evidence.

## 10. Apply the Same Method to Other Artifacts

The approach can be reused across an ISO 27001 implementation.

| Requirement area         | Example policy or procedure                   | Example tracker or record             |
| ------------------------ | --------------------------------------------- | ------------------------------------- |
| Risk management          | Risk Assessment Methodology                   | Risk Register                         |
| Asset management         | Asset Management Policy                       | Asset Inventory                       |
| Access management        | Access Control Policy                         | User Access Review Tracker            |
| Incident management      | Incident Management Procedure                 | Incident Register                     |
| Supplier security        | Supplier Security Policy                      | Supplier Risk Register                |
| Vulnerability management | Vulnerability Management Procedure            | Vulnerability and Remediation Tracker |
| Business continuity      | Business Continuity Procedure                 | Test and Recovery Action Register     |
| Corrective action        | Nonconformity and Corrective Action Procedure | Corrective-Action Register            |

Not every area requires a separate policy and spreadsheet. Related requirements may be addressed through a single controlled document or system if the arrangement meets the applicable requirements and provides sufficient evidence.

The objective is not to create the largest possible document library. It is to establish an effective, maintainable management system.

## 11. Common Mistakes to Avoid

### Copying generic templates without understanding the requirement

A template may contain irrelevant controls or omit important organizational risks. Tailor it to the approved scope and actual operating environment.

### Treating every Annex A control as automatically mandatory

Use the risk assessment and treatment process to determine the necessary controls, document the rationale and maintain an accurate SoA.

### Creating trackers without assigning owners

A tracker without accountable owners and completion criteria will quickly become an inactive spreadsheet.

### Using sample data as real evidence

Illustrative records are useful for training and design, but operational evidence must come from actual activities. Never fabricate or backdate records.

### Closing actions without verification

A status update is not proof of remediation. Define the evidence required for closure and independently verify it where appropriate.

### Creating documents that contradict actual practices

The policy, procedure, tracker and technical implementation must agree. If the organization cannot follow the process as written, correct the process or revise the policy through proper approval.

## 12. A Practical Workflow for GRC Consultants

A repeatable workflow is:

1. Identify the source requirement.
2. Record its exact reference and applicability.
3. Interpret the requirement in the organization's context.
4. Define the control objective and accountable owner.
5. Design or update the policy and procedure.
6. Design the tracker or operational record.
7. Populate it using verified organizational information.
8. Identify and retain appropriate evidence.
9. Test samples to assess control operation.
10. Record gaps and assign corrective actions.
11. Retest after remediation.
12. Maintain the mapping to risks, controls and the SoA.

For a project starting from scratch, prioritize the ISMS scope, context, risk methodology, risk assessment, risk treatment plan and SoA before attempting to complete every supporting artifact. These foundational decisions determine which controls need to be implemented and how they should be evidenced.

## Conclusion

Creating an ISO 27001 policy is not simply a documentation exercise. It is the process of translating a requirement into an approved rule, an operational workflow, accountable responsibilities, traceable records and verifiable results.

For a GRC consultant, the real value lies in connecting these components so that management can understand compliance status, control owners know what to do, deficiencies are tracked to closure and auditors can verify how the ISMS operates.

The key principle is straightforward:

**A requirement defines what must be achieved. A policy defines the rules. A tracker records the activity. Evidence demonstrates what happened. Testing determines whether the control is effective.**

Use this method consistently, and your ISMS documentation becomes an operational management system rather than a collection of files prepared only for certification.
