---
title: "Vendor Management"
description: "Vendor and third-party risk management process for Bounty."
---

Last updated: July 16, 2026

Bounty uses a risk-based vendor management process for third-party tools, infrastructure providers, subprocessors, developer tools, customer-authorized integrations, and corporate operations vendors.

The process is designed to identify vendors that may access customer data, personal data, production systems, source code, credentials, internal information, or other sensitive information, and to review each vendor at a level that matches its risk.

This page is broader than the [Subprocessors](/subprocessors) page. The subprocessor list focuses on vendors that may process Customer Personal Data or Customer Data as part of delivering Bounty. This vendor management process also covers internal enterprise applications, developer tools, production access tools, customer-authorized source systems, and corporate operations vendors.

## Risk Tiers

| Tier | Description | Review expectation |
| --- | --- | --- |
| Tier 1 | Vendors that host, store, process, transmit, or can access customer data, production systems, sensitive internal information, credentials, CI/CD secrets, source data, or other high-impact systems. | Reviewed before onboarding where practical, approved by an appropriate owner, and reviewed at least annually or upon material change. |
| Tier 2 | Vendors that may receive limited customer context, internal documentation, product planning data, code snippets, telemetry, error context, or employee information, but do not broadly host core customer data or production systems. | Reviewed before onboarding and on renewal, material scope change, incident, or security concern. |
| Tier 3 | Vendors used for low-risk corporate operations with no expected customer data, production access, sensitive internal data, or material operational dependency. | Reviewed as needed based on risk and use. |

## Due Diligence

For Tier 1 vendors, Bounty reviews and records relevant information such as:

- Business purpose and product function.
- Data categories processed, including whether customer data or personal data is involved.
- Whether the vendor is mandatory, optional, customer-configured, or internal-only.
- Vendor security, privacy, trust, and subprocessor documentation.
- Data processing, privacy, security, confidentiality, and other contractual terms where applicable.
- Data location or hosting region where available.
- Encryption, access control, incident notification, deletion, retention, and support access information where available.
- OAuth scopes, API permissions, production access, CI/CD access, or credential access where applicable.
- Internal owner, approval decision, review date, and next review date.

For Tier 2 vendors, Bounty uses a lighter review focused on the vendor's purpose, data access, contractual terms, security and privacy documentation, and material changes.

For Tier 3 vendors, Bounty applies lightweight review appropriate to the vendor's expected access, operational dependency, and data sensitivity.

## Customer-Authorized Integrations

Some integrations connect to systems that a customer configures or authorizes, such as advertising platforms, analytics tools, CRM systems, lifecycle messaging tools, or customer-managed warehouses.

For these integrations, the customer controls whether to connect the source system and is responsible for the customer's relationship with that provider. Bounty tracks customer-authorized integrations because Bounty may access, sync, query, transform, or process data from those systems when authorized by a customer.

## Review Cadence

Bounty uses a risk-based review cadence:

- Tier 1 vendors are reviewed before onboarding where practical, at least annually, and upon material change.
- Tier 2 vendors are reviewed on onboarding, renewal, material change, incident, or security concern.
- Tier 3 vendors are reviewed as needed based on risk and use.

Material changes may include a new data category, new access path, new integration scope, change in hosting or processing location, change in security posture, acquisition, incident, or other change that affects vendor risk.

## Subprocessors

Vendors that may process Customer Personal Data or Customer Data as part of delivering Bounty are listed on the [Subprocessors](/subprocessors) page.

The vendor management process supports the subprocessor review process by identifying vendor purpose, data access, processing role, security posture, contractual terms, and review cadence.

## Review Records

Bounty maintains vendor review records internally. These records may include vendor documentation, security and privacy materials, contractual terms, approval decisions, review dates, data categories, internal owners, and remediation items.
