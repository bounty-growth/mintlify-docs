---
title: "Vendor Management"
description: "Draft vendor and third-party risk management process for Bounty."
---

# Vendor Management

**Draft - security and legal review required.** This page is a working draft for Bounty Growth / Bounty and must be reviewed before publication or use in customer security questionnaires.

Last updated: [TODO: confirm publication date]

## Purpose

Bounty uses a risk-based vendor management process for third-party tools, infrastructure providers, subprocessors, developer tools, customer-authorized integrations, and corporate operations vendors.

The goal is to understand which vendors may access customer data, personal data, production systems, source code, credentials, internal information, or other sensitive information, and to review those vendors at a level that matches their risk.

This page is broader than the [Subprocessors](/subprocessors) page. The subprocessor list focuses on vendors that may process Customer Personal Data or Customer Data as part of delivering the Bounty service. This vendor management page also includes internal enterprise apps, developer tools, production access tools, customer-authorized source systems, and corporate operations vendors.

## Current Status

This is a draft control description. Bounty has started maintaining a vendor inventory and risk tiers. [TODO: confirm formal approval date, control owner, review evidence location, and first completed Tier 1 review cycle.]

Bounty should not state that all vendors are assessed annually until the annual review process has been implemented and review evidence exists.

## Risk Tiers

| Tier | Description | Review expectation |
| --- | --- | --- |
| Tier 1 | Vendors that host, store, process, transmit, or can access customer data, production systems, sensitive internal information, credentials, CI/CD secrets, source data, or other high-impact systems. | Due diligence before onboarding where practical, executive/security owner approval, and annual review target. [TODO: confirm owner and evidence requirements.] |
| Tier 2 | Vendors that may receive limited customer context, internal documentation, product planning data, code snippets, telemetry, error context, or employee information, but do not broadly host core customer data or production systems. | Review before onboarding and on renewal, material scope change, incident, or security concern. [TODO: confirm review cadence.] |
| Tier 3 | Vendors used for low-risk corporate operations with no expected customer data, production access, sensitive internal data, or material operational dependency. | Lightweight review as needed. [TODO: define Tier 3 criteria and examples.] |

## Due Diligence Process

For Tier 1 vendors, Bounty's target due diligence process is to review and record:

- Business purpose and product function.
- Data categories processed, including whether customer data or personal data is involved.
- Whether the vendor is mandatory, optional, customer-configured, or internal-only.
- Vendor security, privacy, trust, and subprocessor documentation.
- DPA, privacy terms, security terms, and confidentiality terms where applicable.
- Data location or hosting region where available.
- Encryption, access control, incident notification, deletion, retention, and support access information where available.
- OAuth scopes, API permissions, production access, CI/CD access, or credential access where applicable.
- Internal owner and approval decision.
- Next review date and review evidence.

For Tier 2 vendors, Bounty's target process is a lighter review focused on the vendor's purpose, data access, contractual terms, security/privacy documentation, and any material changes.

For customer-authorized source systems, the customer controls whether to connect the integration. Bounty still tracks these systems because Bounty may access, sync, query, or process data from them when authorized by a customer.

## Review Cadence

Bounty uses a risk-based cadence:

- Tier 1 vendors: targeted for annual review and review on material change.
- Tier 2 vendors: reviewed on onboarding, renewal, material change, incident, or security concern.
- Tier 3 vendors: reviewed as needed based on risk and use.

[TODO: confirm whether "annual review" is calendar-year, rolling 12-month, contract-renewal based, or another cadence.]

## Customer Questionnaire Position

Until the first review cycle is completed, the careful answer is:

> We maintain a risk-based vendor inventory and are implementing a formal vendor review cadence. Vendors that process customer data or support critical product operations are prioritized for due diligence and targeted annual review. Lower-risk vendors are reviewed on onboarding, renewal, material change, incident, or security concern.

After Tier 1 review evidence exists, the stronger answer can be:

> We maintain a risk-based vendor management process. Vendors that process customer data or support critical product operations are reviewed before onboarding and periodically thereafter. Tier 1 vendors are reviewed at least annually or upon material change. Lower-risk vendors are reviewed on renewal, material change, incident, or security concern.

## Enterprise Apps

Internal SaaS tools employees use to run the business.

| Vendor / tool | Category and tier | Use and data access | Review status |
| --- | --- | --- | --- |
| Google Workspace | Enterprise app / productivity suite (Tier 1) | Email, calendar, docs, employee identity, and internal collaboration. May contain sensitive internal information and some customer-related information. | [TODO: collect admin settings, security documentation, DPA/privacy terms, access controls, retention settings, and next review date.] |
| Notion | Enterprise app / knowledge base (Tier 2) | Internal documentation and planning. May include some customer, product, and security information. | [TODO: collect security documentation, access controls, workspace settings, and next review date.] |
| Linear | Enterprise app / product delivery (Tier 2) | Issue tracking and product planning. May include customer names, support context, and product/security work items. | [TODO: collect security documentation, access controls, workspace settings, and next review date.] |

## Product Infrastructure And Subprocessors

Vendors that host, store, process, or transmit product/customer data as part of delivering the Bounty service.

| Vendor / tool | Category and tier | Use and data access | Review status |
| --- | --- | --- | --- |
| Supabase | Product infrastructure / subprocessor (Tier 1) | Auth, Postgres database, service role access, storage, and auth data. May store account, workspace, customer, and application data. | [TODO: collect trust/security docs, DPA/subprocessor terms, project region, encryption details, backup/retention details, access controls, and next review date.] |
| Airbyte Cloud | Product data integration / subprocessor (Tier 1) | Handles OAuth/source setup and syncs customer-authorized ad, analytics, CRM, and other source data. | [TODO: collect trust/security docs, DPA/subprocessor terms, region/data residency, connector credential handling, retention, access controls, and next review date.] |
| ClickHouse | Product data warehouse (Tier 1) | Stores and queries analytics/source data for product analysis workflows. | [TODO: collect trust/security docs, DPA/subprocessor terms, cloud region, encryption details, retention, access controls, and next review date.] |
| OpenAI API Platform | AI processing vendor (Tier 1) | In-product LLM requests. Prompts and context can include customer metrics, analysis context, and generated outputs. | [TODO: collect API data usage terms, retention settings, security docs, DPA terms, model/data processing settings, and next review date.] |
| E2B | Code sandbox / AI analysis infrastructure (Tier 1) | Sandboxed code execution for analysis workflows. Customer CSVs or other data files may be uploaded into sandboxes for Python analysis. | [TODO: collect security docs, DPA/privacy terms, sandbox isolation details, data retention/deletion behavior, region, and next review date.] |
| PostHog | Product analytics / session replay (Tier 1 or Tier 2) | Product analytics, user identification, and session recording if enabled. May process user names, email addresses, product events, and replay data. | [TODO: confirm whether session replay is enabled, masking/redaction settings, data location, retention, DPA terms, opt-out controls, final tier, and next review date.] |
| Resend | Email delivery (Tier 2) | Transactional or report email delivery. Receives recipient email addresses and email content. | [TODO: collect security/privacy docs, DPA terms, message content handling, retention, and next review date.] |
| Codex | AI coding assistant (Tier 2) | Developer tool for code generation and review. May receive code context, snippets, and developer-provided context. | [TODO: confirm account configuration, data retention/training settings, approved-use policy, and whether customer data may be submitted.] |
| Claude Code | AI coding assistant (Tier 2) | Developer tool for code generation and review. May receive code context, snippets, and developer-provided context. | [TODO: confirm account configuration, data retention/training settings, approved-use policy, and whether customer data may be submitted.] |

## Developer And Production Access Tools

Tools used to build, deploy, monitor, or access production systems.

| Vendor / tool | Category and tier | Use and data access | Review status |
| --- | --- | --- | --- |
| Vercel and Vercel Workflows | Product infrastructure / deployment (Tier 1) | Hosts and executes the Bounty app and workflows. May process app requests, deployment artifacts, logs, environment variables, and workflow data. | [TODO: collect trust/security docs, DPA/subprocessor terms, region/runtime details, secrets handling, incident terms, and next review date.] |
| GitHub and GitHub Actions | Developer platform / CI/CD (Tier 1) | Source code, pull requests, CI/CD workflows, CI secrets, and production migration workflows. | [TODO: collect security docs, account access controls, branch protection, secrets handling, audit logs, SSO/MFA settings, and next review date.] |
| Sentry | Error monitoring / observability (Tier 2, or Tier 1 if error events include customer data) | Exception monitoring, request context, source maps, and diagnostic data. Could receive customer data if errors include request payloads or identifiers. | [TODO: confirm scrubbing settings, event payloads, retention, DPA terms, final tier, and next review date.] |

## Data Source And Integration Partners

Customer-authorized source systems and integration partners that Bounty connects to on behalf of customers.

| Vendor / tool | Category and tier | Use and data access | Review status |
| --- | --- | --- | --- |
| Meta / Facebook Ads | Customer-authorized source system | Advertising source data synced into a customer warehouse, Bounty warehouse, or Bounty analytics store as configured. | [TODO: confirm data flow, OAuth scopes, retention, and vendor documentation link.] |
| Google Ads | Customer-authorized source system | Advertising source data synced into a customer warehouse, Bounty warehouse, or Bounty analytics store as configured. | [TODO: confirm data flow, OAuth scopes, retention, and vendor documentation link.] |
| GA4 | Customer-authorized source system | Web analytics source data synced into a customer warehouse, Bounty warehouse, or Bounty analytics store as configured. | [TODO: confirm data flow, OAuth scopes, retention, and vendor documentation link.] |
| HubSpot | Customer-authorized source system | CRM source data synced into a customer warehouse, Bounty warehouse, or Bounty analytics store as configured. | [TODO: confirm data flow, OAuth scopes, retention, and vendor documentation link.] |
| Customer.io | Customer-authorized source system | Lifecycle messaging platform source data synced into a customer warehouse, Bounty warehouse, or Bounty analytics store as configured. | [TODO: confirm support status, data flow, API scopes, retention, and vendor documentation link.] |
| Apple Search Ads | Customer-authorized source system | Advertising source data synced into a customer warehouse, Bounty warehouse, or Bounty analytics store as configured. | [TODO: confirm support status, data flow, API scopes, retention, and vendor documentation link.] |
| Snowflake | Customer data source / direct-query warehouse (Tier 1 when configured) | Customer-configured direct warehouse queries and selected warehouse tables. | [TODO: confirm connection model, credential handling, query logging, data retention, region, and vendor documentation link.] |
| Tinybird | Customer/source data integration (Tier 1 when configured) | Customer-configured Tinybird tables or APIs used as source data for Bounty analysis workflows. | [TODO: confirm connection model, data flow, credential handling, retention, region, and vendor documentation link.] |

## Corporate Operations Vendors

Vendors that process employee, finance, legal, payroll, or administrative data.

| Vendor / tool | Category and tier | Use and data access | Review status |
| --- | --- | --- | --- |
| [TODO: add vendor] | Corporate operations vendor | [TODO: describe employee, finance, legal, payroll, or administrative data processed] | [TODO: collect review evidence if Tier 1 or Tier 2.] |

## Open Questions

- [TODO: confirm whether this page should be public, private, or customer-confidential.]
- [TODO: confirm exact vendor owner, approver, and review evidence location.]
- [TODO: complete Tier 1 vendor due diligence and record review dates.]
- [TODO: confirm whether Codex and Claude Code are approved for customer data, code only, or restricted contexts.]
- [TODO: confirm whether PostHog session replay is enabled and whether default masking is sufficient.]
- [TODO: confirm whether Sentry receives customer data in event payloads.]
- [TODO: confirm whether all listed source systems are currently supported and publicly nameable.]
