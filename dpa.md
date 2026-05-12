---
title: "Data Processing Addendum"
description: "Data Processing Addendum for Bounty."
---

# Data Processing Addendum

Last updated: May 12, 2026

This Data Processing Addendum ("DPA") applies when Bounty processes Customer Personal Data on behalf of Customer in connection with Bounty's services and the DPA is accepted by the parties or incorporated into the applicable agreement.

## 1. Scope

"Customer Personal Data" means personal data contained in Customer Data that Bounty processes on behalf of Customer under the applicable agreement.

If there is a conflict between this DPA and the applicable agreement, the applicable agreement controls except where this DPA expressly provides more specific data processing terms required by applicable data protection law.

## 2. Roles

Customer is the Controller or Processor of Customer Personal Data, depending on Customer's relationship with the relevant data subjects and data sources.

Bounty is the Processor or Subprocessor of Customer Personal Data when it processes Customer Personal Data on behalf of Customer.

Each party will comply with data protection laws that apply to its role.

## 3. Processing Instructions

Bounty will process Customer Personal Data only:

- To provide, secure, support, maintain, and improve the service.
- As instructed by Customer through the agreement, product configuration, support requests, and authorized use of the service.
- As required by applicable law.

Bounty will notify Customer if Bounty believes an instruction violates applicable data protection law, unless prohibited by law.

## 4. Confidentiality

Bounty will ensure that personnel authorized to process Customer Personal Data are bound by confidentiality obligations or are subject to appropriate statutory confidentiality duties.

## 5. Security Measures

Bounty will implement and maintain appropriate technical and organizational measures designed to protect Customer Personal Data against accidental or unlawful destruction, loss, alteration, unauthorized disclosure, or unauthorized access.

Additional measures are listed in Annex 2 and summarized in [Security Controls](/security-controls).

## 6. Subprocessors

Customer authorizes Bounty to use subprocessors to provide the service, subject to this DPA. The subprocessor list is available at [Subprocessors](/subprocessors).

Bounty will impose written data protection obligations on subprocessors that are appropriate for the services they provide.

Bounty remains responsible for subprocessors' processing of Customer Personal Data to the extent required by applicable data protection law and the applicable agreement.

Customers with contractual notice or objection rights for new subprocessors receive those rights as described in their agreement with Bounty.

## 7. Assistance With Data Subject Requests

Bounty will provide reasonable assistance to Customer for data subject requests relating to Customer Personal Data, taking into account the nature of processing and the information available to Bounty.

If Bounty receives a request directly from a data subject relating to Customer Personal Data, Bounty may direct the requester to Customer unless required by law to respond differently.

## 8. Security Incident Notice

Bounty will notify Customer after becoming aware of a Security Incident affecting Customer Personal Data.

"Security Incident" means a confirmed breach of security leading to accidental or unlawful destruction, loss, alteration, unauthorized disclosure of, or unauthorized access to Customer Personal Data.

## 9. Deletion Or Return

At termination or expiration of the service, Bounty will delete or return Customer Personal Data as required by the applicable agreement and product functionality, unless retention is required by law.

## 10. Audit And Documentation

Bounty will make available information reasonably necessary to demonstrate compliance with this DPA, subject to confidentiality, security, and operational limits.

## 11. International Transfers

Bounty and its subprocessors may process Customer Personal Data outside Customer's country or region. Where required, the parties will use an appropriate transfer mechanism.

## 12. CCPA/CPRA Service Provider Terms

Where the CCPA/CPRA applies, Bounty will process Customer Personal Data as a service provider or contractor for Customer and will not sell or share Customer Personal Data, retain, use, or disclose it for purposes other than providing the service, or combine it with personal information from other sources except as permitted by law.

## 13. Liability

Liability for claims arising under this DPA is governed by the liability terms in the applicable agreement, unless prohibited by applicable law.

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
- Support syncs, warehouses, exports, sandbox execution, AI prompts, AI outputs, and customer support workflows where used by Customer.

### Duration

For the term of the applicable agreement, plus any retention period required by law, the agreement, backup practices, security needs, or deletion/export process.

### Categories Of Data Subjects

Customer Personal Data may relate to:

- Customer administrators and authorized users.
- Customer employees, contractors, and business contacts.
- End users, prospects, leads, customers, website visitors, app users, and other individuals represented in customer-authorized data sources.
- Individuals appearing in campaign, ad, analytics, CRM, warehouse, support, or event data connected by Customer.

### Categories Of Personal Data

Customer Personal Data may include:

- Identifiers, such as names, email addresses, user IDs, account IDs, device IDs, advertising IDs, and customer IDs.
- Business contact and account data.
- Marketing, advertising, campaign, ad, creative, event, conversion, and attribution data.
- Product usage, website, app, event, and analytics data.
- CRM, lifecycle, deal, and customer interaction data.
- Warehouse table data, schemas, fields, and query results.
- Prompts, queries, outputs, notes, generated actions, analysis results, and support communications.
- Credentials, tokens, files, recordings, exports, sandbox artifacts, and other Customer Data submitted to or generated through the service.
- Technical logs, request metadata, IP addresses, browser/device data, and error data.

### Sensitive Or Special Category Data

The service is not intended for sensitive personal data, special category data, protected health information, payment card data, government identifiers, children's data, or other highly regulated data unless expressly authorized in writing.

## Annex 2: Technical And Organizational Measures

Bounty maintains technical and organizational measures appropriate to the nature of the service, including:

- Authentication and permissions: CLI requests use the logged-in user's Bounty permissions.
- Credential minimization for agent workflows: normal CLI workflows do not require agents to receive database credentials, warehouse credentials, ad platform credentials, infrastructure secrets, or local environment files.
- Session management: Bounty CLI stores a local user session, and users can clear it with logout.
- Backend URL safety: Bounty CLI accepts secure remote backend URLs and local development URLs, and rejects insecure non-local HTTP URLs.
- Least-privilege guidance: agents are instructed to verify identity, use parseable evidence, state date ranges, and avoid requesting infrastructure secrets.
- Encryption in transit: Bounty uses HTTPS/TLS and provider-managed transport protections for app, API, integration, vendor, and CLI communications where applicable.
- Encryption at rest: Bounty relies on infrastructure-provider encryption for application databases, storage, warehouses, logs, backups, and other hosted systems where applicable.
- Access controls: internal access is limited based on business need and protected by authentication, authorization, and MFA where supported.
- Logging and monitoring: Bounty uses product, infrastructure, and error monitoring to troubleshoot, secure, and operate the service.
- Vulnerability management: security fixes are triaged and remediated through Bounty's code review, CI, deployment, and engineering tracking workflows.
- Data deletion and retention: Customer Data is retained and deleted according to the applicable agreement, product functionality, legal requirements, and operational needs.
- Incident response: Bounty investigates security events, escalates confirmed incidents, and notifies affected customers as required by the applicable agreement and law.
- Vendor management: Bounty maintains a risk-based vendor management process for vendors that process customer data or support critical product operations.
