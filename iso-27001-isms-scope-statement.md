# ISMS Scope Statement — [Organization Name]

> **Framework:** ISO/IEC 27001:2022 — Clause 4.3 (Determining the scope of the ISMS)
>
> Free template from [ComplianceDocs](https://compliancedocshq.com/resources/templates/free-iso-27001-isms-scope-statement-template) — editable Word version (.docx) in [templates/](templates/free-iso-27001-isms-scope-statement-template.docx). Replace every [bracketed placeholder]. No template makes an organization certified or compliant on its own.

This document defines and records the scope of the Information Security Management System (ISMS) operated by [Organization Name], as required by ISO/IEC 27001:2022 Clause 4.3. It identifies the organizational units, locations, systems, services, and information within the ISMS boundary, records exclusions with justification, and documents the interfaces and dependencies that the scope determination took into account.

## 1. Purpose

ISO/IEC 27001:2022 Clause 4.3 requires the organization to determine the boundaries and applicability of the ISMS to establish its scope, and to make the scope available as documented information. This Scope Statement fulfills that requirement for [Organization Name].

In determining this scope, [Organization Name] has considered: (a) the external and internal issues identified under Clause 4.1; (b) the requirements of interested parties identified under Clause 4.2; and (c) the interfaces and dependencies between activities performed by [Organization Name] and those performed by other organizations, as Clause 4.3 directs.

This document is maintained as documented information in accordance with ISO/IEC 27001:2022 Clause 7.5 and is reviewed as part of management review under Clause 9.3.

## 2. Organizational Context Summary (Clauses 4.1 and 4.2)

[Organization Name] is a [brief description of business, e.g., "provider of cloud-hosted payroll software to mid-market employers"] headquartered at [Headquarters Address]. The external and internal issues relevant to the ISMS — including [e.g., regulatory obligations, customer contractual security requirements, reliance on cloud infrastructure, and workforce distribution] — are recorded in [Context of the Organization Register / document reference], maintained under Clause 4.1.

Interested parties relevant to the ISMS and their applicable requirements — including [e.g., customers, regulators, employees, suppliers, and shareholders] — are recorded in [Interested Parties Register / document reference], maintained under Clause 4.2. The scope defined in Section 3 was determined by reference to both registers.

## 3. Scope of the ISMS

The ISMS of [Organization Name] applies to the protection of information within the following boundary. The formal scope statement, suitable for use on the certificate of conformity, is:

"The management of information security in the provision of [products/services description] by [Organization Name], delivered from [Location(s)], in accordance with the Statement of Applicability version [X.X] dated [Date]."

The following elements are within the ISMS boundary:

- Locations: [Headquarters Address]; [Office/Data Center 2 — Address]; remote work environments of in-scope personnel to the extent governed by [Remote Working Policy reference].
- Business services and processes: [Service Name 1 — e.g., SaaS platform operation]; [Service Name 2 — e.g., customer support]; supporting processes including [e.g., software development, HR onboarding/offboarding, supplier management, incident management].
- Information systems: [System Name — production environment]; [System Name — corporate IT / identity provider]; [System Name — code repository and CI/CD]; [System Name — ticketing/CRM]; endpoints issued to in-scope personnel.
- Information assets: customer data processed by the in-scope services; personnel data of in-scope staff; source code, configuration, and operational documentation; records required by the ISMS. Assets are inventoried in [Asset Inventory reference].
- Organizational units and teams: [Engineering]; [IT/Security]; [Operations]; [People/HR]; [Executive management]; and contractors performing in-scope roles under written agreements.
- Networks: [corporate network / VPN name]; production cloud environments in [Cloud Provider, region(s)].

## 4. Exclusions and Justification

The following are excluded from the ISMS scope. Each exclusion is recorded with its justification and an assessment confirming that the exclusion does not affect [Organization Name]'s ability or responsibility to ensure information security within the scope, nor the security requirements determined from Clauses 4.1 and 4.2. Note that this section addresses scope boundaries; the applicability of Annex A controls is justified separately in the Statement of Applicability under Clause 6.1.3 d).

Exclusion pattern (repeat per exclusion): [Excluded unit/system/location] — Justification: [e.g., "operates under separate management, shares no infrastructure, networks, personnel, or information with in-scope services"] — Boundary control: [e.g., "network segmentation and access restrictions documented in [reference]"] — Assessed by: [Role/Title] on [Date].

- [Business Unit Name] — separate legal entity with independent management and no shared systems; boundary enforced by [control reference].
- [Legacy System Name] — scheduled for decommission by [Date]; holds no in-scope information; isolated per [reference].
- [Location Name] — performs [non-relevant activity] only; no access to in-scope information or systems.

## 5. Interfaces and Dependencies

As required by ISO/IEC 27001:2022 Clause 4.3 c), the following interfaces and dependencies between activities performed by [Organization Name] and those performed by other organizations were considered in determining the scope. Security requirements for these relationships are addressed through supplier management processes and written agreements, and the associated risks are treated within the risk assessment process under Clause 6.1.2.

- [Cloud Provider Name] — hosting of production infrastructure; responsibilities allocated per the provider's shared responsibility model and [agreement reference].
- [Managed Service Provider Name] — [e.g., 24/7 monitoring]; governed by [contract/SLA reference].
- [Software Vendor Name] — [e.g., identity provider, email, payroll processor]; data flows documented in [data flow diagram / record of processing reference].
- [Customer interface] — customer-managed configuration and user administration within the platform; responsibility boundaries stated in [terms of service / customer agreement reference].

## 6. Roles and Responsibilities

The [Role/Title, e.g., Information Security Manager] is responsible for maintaining this Scope Statement, proposing changes when the organization, its services, locations, or dependencies change, and presenting the scope for review at management review (Clause 9.3). Top management, represented by [Role/Title], is responsible for approving this Scope Statement and any changes to it, consistent with its leadership and commitment obligations under Clause 5.1. All personnel performing in-scope roles are responsible for complying with ISMS policies applicable to the activities described in Section 3.

## 7. Review and Maintenance

This Scope Statement is reviewed at least [annually] and upon significant change, including: acquisition or divestiture; addition or closure of locations; introduction or retirement of in-scope systems or services; material changes to interested-party requirements identified under Clause 4.2; or changes to the interfaces and dependencies in Section 5. Changes are approved per Section 8 and version-controlled in accordance with Clause 7.5.3. The Statement of Applicability and risk assessment are reviewed for consistency whenever this scope changes.

## 8. Approval

This Scope Statement is approved by top management of [Organization Name].

Approved by: [Name], [Role/Title] — Signature: ______________________ — Date: [Date]

Document owner: [Name], [Role/Title] | Document ID: [DOC-ID] | Version: [X.X] | Effective date: [Date] | Next review date: [Date]

Revision history: Version [X.X] — [Date] — [Summary of change] — [Author] — [Approver].

## How to customize

1. Replace every [bracketed placeholder] with your organization's actual names, locations, systems, and document references — search the document for "[" to find them all.
2. Complete your Clause 4.1 context register and Clause 4.2 interested-parties register first, then reference their document IDs in Section 2 so the scope traceably derives from them.
3. List every physical location, system, service, and team that touches in-scope information in Section 3 — auditors will test the boundary, so be specific rather than broad.
4. For each exclusion in Section 4, apply the justification pattern fully: state why it is excluded, how the boundary is enforced, and who assessed it and when.
5. Align the scope statement wording in Section 3 with your Statement of Applicability version and date — certification bodies print this sentence on the certificate.
6. Have top management sign the approval block, assign a document ID and version, and set the next review date before distributing.
