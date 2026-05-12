---
title: "Data Processing Addendum"
description: "Draft Data Processing Addendum for Bounty."
---

# Data Processing Addendum

**Draft - legal review required.** This Data Processing Addendum is a working draft for Bounty Growth / Bounty and must be reviewed by legal counsel before publication or signature. It is not an executed agreement unless accepted through the process approved by Bounty and Customer. [TODO: confirm DPA execution mechanics.]

Last updated: [TODO: confirm publication date]

## 1. Scope

This DPA applies when Bounty processes Customer Personal Data on behalf of Customer in connection with Bounty's services.

"Customer Personal Data" means personal data contained in Customer Data that Bounty processes on behalf of Customer under the applicable agreement.

If there is a conflict between this DPA and the applicable agreement, [TODO: confirm order of precedence].

## 2. Roles

Customer is the Controller or Processor of Customer Personal Data, depending on Customer's relationship with the relevant data subjects and data sources.

Bounty is the Processor or Subprocessor of Customer Personal Data when it processes Customer Personal Data on behalf of Customer.

Each party will comply with data protection laws that apply to its role. [TODO: confirm covered laws and definitions.]

## 3. Processing Instructions

Bounty will process Customer Personal Data only:

- To provide, secure, support, maintain, and improve the service.
- As instructed by Customer through the agreement, product configuration, support requests, and authorized use of the service.
- As required by applicable law.

Bounty will notify Customer if Bounty believes an instruction violates applicable data protection law, unless prohibited by law. [TODO: confirm notice process.]

## 4. Confidentiality

Bounty will ensure that personnel authorized to process Customer Personal Data are bound by confidentiality obligations or are subject to appropriate statutory confidentiality duties.

[TODO: confirm personnel confidentiality controls and contractor access terms.]

## 5. Security Measures

Bounty will implement and maintain appropriate technical and organizational measures designed to protect Customer Personal Data against accidental or unlawful destruction, loss, alteration, unauthorized disclosure, or unauthorized access.

Current public docs state that Bounty CLI and agent workflows use authenticated user sessions and logged-in user permissions, and that normal CLI workflows do not require database credentials, warehouse credentials, ad platform credentials, infrastructure secrets, or local environment files.

[TODO: confirm full app security measures, including encryption, access controls, backups, logging, monitoring, vulnerability management, incident response, and vendor management.]

Additional draft measures are listed in Annex 2.

## 6. Subprocessors

Customer authorizes Bounty to use subprocessors to provide the service, subject to this DPA. The current draft list is available at [Subprocessors](/subprocessors).

Bounty will impose written data protection obligations on subprocessors that are appropriate for the services they provide.

Bounty remains responsible for subprocessors' processing of Customer Personal Data to the extent required by applicable data protection law and the applicable agreement. [TODO: confirm liability language.]

[TODO: confirm subprocessor approval process, objection process, and change notification period, such as 10 business days.]

## 7. Assistance With Data Subject Requests

Bounty will provide reasonable assistance to Customer for data subject requests relating to Customer Personal Data, taking into account the nature of processing and the information available to Bounty.

If Bounty receives a request directly from a data subject relating to Customer Personal Data, Bounty may direct the requester to Customer unless required by law to respond differently. [TODO: confirm request handling process and timelines.]

## 8. Security Incident Notice

Bounty will notify Customer after becoming aware of a Security Incident affecting Customer Personal Data.

"Security Incident" means a confirmed breach of security leading to accidental or unlawful destruction, loss, alteration, unauthorized disclosure of, or unauthorized access to Customer Personal Data.

[TODO: confirm breach notice timing, notice contents, security contact, escalation process, and exclusions for unsuccessful attempts or routine security events.]

## 9. Deletion Or Return

At termination or expiration of the service, Bounty will delete or return Customer Personal Data as required by the applicable agreement and product functionality, unless retention is required by law.

[TODO: confirm deletion/export process, backup retention, log retention, sandbox artifact deletion, warehouse deletion, and support data retention.]

## 10. Audit And Documentation

Bounty will make available information reasonably necessary to demonstrate compliance with this DPA, subject to confidentiality, security, and operational limits.

[TODO: confirm audit rights, documentation package, questionnaire process, frequency limits, customer audit mechanics, third-party audit reports, and fees.]

## 11. International Transfers

Bounty and its subprocessors may process Customer Personal Data outside Customer's country or region. [TODO: confirm processing locations.]

Where required, the parties will use an appropriate transfer mechanism. [TODO: confirm whether Standard Contractual Clauses, UK Addendum, Data Privacy Framework, or other safeguards apply.]

## 12. CCPA/CPRA Service Provider Terms

Where the CCPA/CPRA applies, Bounty will process Customer Personal Data as a service provider or contractor for Customer and will not sell or share Customer Personal Data, retain, use, or disclose it for purposes other than providing the service, or combine it with personal information from other sources except as permitted by law.

[TODO: confirm CCPA/CPRA applicability, service provider/contractor language, certification language, and whether any exceptions are needed.]

## 13. Liability

[TODO: confirm liability cap and whether DPA claims share the agreement cap, have a separate cap, or are uncapped.]

## Annex 1: Processing Details

### Subject Matter

Bounty's processing of Customer Personal Data to provide a B2B SaaS analytics and growth operations product, including connected data sources, metrics, performance analysis, actions, agents, chat, CLI workflows, and support.

### Nature And Purpose Of Processing

Bounty may collect, receive, host, store, query, transform, analyze, display, transmit, log, delete, and otherwise process Customer Personal Data to:

- Authenticate users and enforce workspace permissions.
- Connect to customer-authorized data sources.
- Organize connectors, connections, tables, data sources, fields, and projections.
- Support analysis, metrics, driver trees, campaign and ad views, actions, agents, and chat.
- Provide CLI and agent workflows using logged-in user permissions.
- Monitor, secure, troubleshoot, and improve the service.

[TODO: confirm whether syncs, warehouses, exports, sandbox execution, and AI prompts/outputs should be listed in more detail.]

### Duration

For the term of the applicable agreement, plus any retention period required by law, the agreement, backup practices, security needs, or deletion/export process.

[TODO: confirm exact retention and deletion timelines.]

### Categories Of Data Subjects

Customer Personal Data may relate to:

- Customer administrators and authorized users.
- Customer employees, contractors, and business contacts.
- End users, prospects, leads, customers, website visitors, app users, and other individuals represented in customer-authorized data sources.
- Individuals appearing in campaign, ad, analytics, CRM, warehouse, support, or event data connected by Customer.

[TODO: confirm categories based on supported integrations and customer use cases.]

### Categories Of Personal Data

Customer Personal Data may include:

- Identifiers, such as names, email addresses, user IDs, account IDs, device IDs, advertising IDs, and customer IDs.
- Business contact and account data.
- Marketing, advertising, campaign, ad, creative, event, conversion, and attribution data.
- Product usage, website, app, event, and analytics data.
- CRM, lifecycle, deal, and customer interaction data.
- Warehouse table data, schemas, fields, and query results.
- Prompts, queries, outputs, notes, generated actions, analysis results, and support communications.
- Technical logs, request metadata, IP addresses, browser/device data, and error data.

[TODO: confirm whether credentials, tokens, files, recordings, exports, and sandbox artifacts are processed and should be listed.]

### Sensitive Or Special Category Data

The service is not intended for sensitive personal data, special category data, protected health information, payment card data, government identifiers, children's data, or other highly regulated data unless expressly authorized in writing.

[TODO: confirm sensitive data policy, technical controls, and whether any customers or integrations may submit special category data.]

## Annex 2: Technical And Organizational Measures

The following measures are documented or proposed for confirmation:

- Authentication and permissions: CLI requests use the logged-in user's Bounty permissions.
- Credential minimization for agent workflows: normal CLI workflows do not require agents to receive database credentials, warehouse credentials, ad platform credentials, infrastructure secrets, or local environment files.
- Session management: Bounty CLI stores a local user session, and users can clear it with logout.
- Backend URL safety: Bounty CLI accepts secure remote backend URLs and local development URLs, and rejects insecure non-local HTTP URLs.
- Least-privilege guidance: agents are instructed to verify identity, use parseable evidence, state date ranges, and avoid requesting infrastructure secrets.
- Encryption in transit: [TODO: confirm for app, APIs, integrations, warehouses, vendors, and CLI.]
- Encryption at rest: [TODO: confirm for application database, storage, warehouse, logs, backups, vendors, and sandbox artifacts.]
- Access controls: [TODO: confirm internal access controls, MFA/SSO, role-based access, production access approval, and employee offboarding.]
- Logging and monitoring: [TODO: confirm product logging, audit logs, error monitoring, security monitoring, retention, and review process.]
- Vulnerability management: [TODO: confirm dependency scanning, code review, penetration testing, security testing, and remediation timelines.]
- Data deletion and retention: [TODO: confirm customer deletion/export workflows, backup retention, log retention, and vendor deletion obligations.]
- Incident response: [TODO: confirm incident response plan, security contact, escalation process, and customer notification timing.]
- Vendor management: Bounty maintains a draft vendor inventory organized by category and risk tier. Tier 1 vendors that process customer data or support critical product operations are targeted for due diligence and annual review; lower-risk vendors are targeted for review on onboarding, renewal, material change, incident, or security concern. [TODO: confirm completed reviews, control owner, contracts, evidence location, subprocessor process, and review cadence.]
