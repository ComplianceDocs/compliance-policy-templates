# Change Management Policy

> **Framework:** SOC 2 (AICPA Trust Services Criteria) — TSC CC8.1 (Change Management)
>
> Free template from [ComplianceDocs](https://compliancedocshq.com/resources/templates/free-change-management-policy-template) — editable Word version (.docx) in [templates/](templates/free-change-management-policy-template.docx). Replace every [bracketed placeholder]. No template makes an organization certified or compliant on its own.

This policy establishes the requirements for requesting, approving, testing, implementing, and documenting changes to [Organization Name]'s information systems and infrastructure. It is designed to support the organization's SOC 2 program by addressing the AICPA Trust Services Criteria for change management, principally CC8.1. Customize all bracketed placeholders before adoption.

## 1. Purpose

The purpose of this policy is to ensure that changes to [Organization Name]'s production systems, applications, infrastructure, and supporting configurations are authorized, designed, developed, tested, approved, and implemented in a controlled manner. This policy supports the organization's alignment with the AICPA Trust Services Criteria (2017, with 2022 points of focus), specifically CC8.1: "The entity authorizes, designs, develops or acquires, configures, documents, tests, approves, and implements changes to infrastructure, data, software, and procedures to meet its objectives." Related criteria addressed in part by this policy include CC6.8 (controls over unauthorized or malicious software) and CC3.4 (identification and assessment of changes that could significantly impact the system of internal control).

## 2. Scope

This policy applies to all changes to production infrastructure, application code, databases, network configurations, security tooling, and third-party integrations that support [System Name] or otherwise fall within the boundaries of [Organization Name]'s SOC 2 system description. It applies to all employees, contractors, and third parties who develop, approve, or deploy such changes. Changes confined to isolated development or sandbox environments with no pathway to production data or services are out of scope, except where noted in Section 4 (Standard Changes).

## 3. Change Categories

All in-scope changes must be classified into one of the following categories prior to implementation. Classification determines the required level of review and approval.

- Standard Changes: Low-risk, repeatable changes that follow a pre-approved, documented procedure (e.g., routine certificate renewal, adding a user to a pre-defined group via an approved workflow). Standard change procedures must be approved in advance by [Role/Title, e.g., Head of Engineering] and reviewed at least annually. Individual executions do not require separate approval but must be logged.
- Normal Changes: All planned changes that are not pre-approved as standard. Normal changes require the full request, approval, testing, and deployment workflow described in Section 4.
- Emergency Changes: Changes required to restore service, remediate an active security vulnerability under exploitation, or prevent imminent harm, where following the normal workflow would cause unacceptable delay. Emergency changes follow the expedited process in Section 6.

## 4. Change Workflow: Request, Approval, Testing, Deployment, Rollback

Normal changes must follow the workflow below. Each step must produce a record in [Change Management System, e.g., ticketing system or version control platform].

- Request: The requester documents the change description, business or technical justification, systems affected, risk assessment, planned implementation window, and rollback plan in [Change Management System].
- Approval: A person other than the author must review and approve the change before deployment to production. Approval authority is defined as follows: routine normal changes — [Role/Title]; changes affecting security controls, authentication, encryption, or data handling — [Role/Title, e.g., Security Officer]; changes with anticipated customer-facing downtime — [Role/Title, e.g., VP of Engineering]. Approvals must be recorded in the system of record.
- Testing: Changes must be tested in a non-production environment before deployment, commensurate with risk. At minimum, application code changes require peer code review and passing automated test results; infrastructure changes require validation in a staging environment or a documented rationale where no equivalent environment exists. Test evidence must be linked to the change record.
- Deployment: Only authorized personnel with production deployment access, as defined in the [Access Control Policy], may implement changes. Deployments must occur through [Deployment Tooling/Pipeline] wherever technically feasible.
- Rollback: Every normal change must include a rollback or remediation plan before approval. If a deployed change causes a service degradation or control failure, the implementer must execute the rollback plan or escalate to [Role/Title] for a decision within the incident management process.
- Verification: After deployment, the implementer or a designated reviewer must confirm the change operated as intended and record the outcome (success, rolled back, or partially implemented) in the change record.

## 5. Segregation of Duties

To reduce the risk of unauthorized or erroneous changes, [Organization Name] enforces segregation of duties within the change process: the author of a change may not be the sole approver of that change, and approval must be performed by a qualified individual with knowledge of the affected system. Where team size makes full segregation impracticable, [Organization Name] applies compensating controls, which must include independent post-implementation review of the change by [Role/Title] and logging of all production deployments with periodic review of those logs. Direct modification of production systems outside the approved deployment process is prohibited except as provided under Section 6.

## 6. Emergency Changes

Emergency changes may be implemented before full documentation is complete, but are not exempt from control. The following requirements apply:

- Verbal or written authorization from [Role/Title, e.g., Engineering Manager or Security Officer] must be obtained before implementation; if no authorizer is reachable and delay would cause material harm, the implementer may proceed and must notify [Role/Title] as soon as practicable.
- A retrospective change record must be created within [X business days, e.g., 2 business days], documenting the justification, actions taken, testing or validation performed, approver, and outcome.
- All emergency changes must receive a retrospective review by [Role/Title] to confirm the emergency classification was appropriate and to identify any needed follow-up remediation.
- Recurring use of the emergency process for foreseeable changes must be flagged in the periodic review described in Section 8.

## 7. Documentation and Evidence Requirements

For each in-scope change, the following records must be retained in [Change Management System] for a minimum of [Retention Period, e.g., one year, or as required by the Data Retention Policy]:

- The change request, including description, justification, and risk assessment
- Identity of the requester, approver(s), and implementer, with timestamps
- Evidence of testing or peer review (e.g., linked pull request reviews, test results, staging validation notes)
- The rollback plan and, where executed, the rollback outcome
- Deployment logs or pipeline records showing what was deployed, when, and by whom
- For emergency changes, the retrospective record and review outcome

## 8. Roles and Responsibilities

[Role/Title, e.g., Chief Technology Officer] owns this policy and is accountable for its enforcement. [Role/Title, e.g., Engineering Managers] are responsible for ensuring their teams follow the workflow in Section 4 and for approving changes within their authority. [Role/Title, e.g., Security Officer] is responsible for reviewing changes affecting security controls and for the emergency change retrospective process. All personnel in scope are responsible for classifying and documenting their changes in accordance with this policy.

## 9. Enforcement, Exceptions, and Review

Violations of this policy may result in disciplinary action up to and including termination, consistent with [Organization Name]'s [Sanctions/HR Policy]. Exceptions to this policy must be documented, risk-assessed, and approved in writing by [Role/Title]; exceptions must include an expiration date and be tracked to closure.

This policy must be reviewed at least annually, and additionally upon significant changes to [Organization Name]'s systems, organizational structure, or applicable requirements. The policy owner must record the review date, reviewer, and any resulting revisions in the version history below.

Version History: [Version] | [Date] | [Author] | [Summary of Changes] | [Approved By]

## How to customize

1. Replace every [bracketed placeholder] — organization name, role titles, system names, tooling, and retention periods — with your actual values; search the document for "[" to confirm none remain.
2. Confirm the approval authorities in Section 4 match your real org chart; in small teams, adopt the compensating controls in Section 5 rather than inventing roles that do not exist.
3. Name your actual change management system of record (e.g., Jira, Linear, GitHub) and verify it can produce the evidence listed in Section 7.
4. Decide which changes qualify as pre-approved Standard Changes and document those procedures separately before relying on that category.
5. Have the policy owner formally approve the document, record the approval in the version history, and set a calendar reminder for the annual review.
6. Cross-reference your Access Control, Incident Response, and Data Retention policies so the references in Sections 4, 6, and 7 point to documents you actually maintain.
