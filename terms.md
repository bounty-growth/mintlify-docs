---
title: "Terms of Service"
description: "Draft Terms of Service for Bounty."
---

# Terms of Service

**Draft - legal review required.** These Terms of Service are a working draft for Bounty Growth / Bounty and must be reviewed by legal counsel before publication. Bracketed TODOs identify legal and product facts that must be confirmed before use.

Last updated: [TODO: confirm publication date]

## 1. Agreement To These Terms

These Terms of Service govern access to and use of Bounty, including the Bounty web app, CLI, agent workflows, documentation, APIs, integrations, AI features, and related services.

By accessing or using Bounty, you agree to these Terms. If you use Bounty on behalf of a company or other organization, you represent that you have authority to bind that organization, and "Customer" means that organization.

If Customer has a separate signed agreement or order form with Bounty that applies to the same service, that agreement controls over these Terms to the extent of any conflict. [TODO: confirm precedence language.]

## 2. Accounts And Credentials

Customer is responsible for:

- Ensuring that users have authority to access Customer's Bounty workspace.
- Maintaining accurate account and organization information.
- Protecting passwords, sessions, API keys, tokens, and credentials.
- Promptly notifying Bounty of suspected unauthorized access.
- Managing user access and removing users who should no longer have access.

Bounty CLI uses a normal Bounty user session and runs requests with the logged-in user's permissions. Users should not give agents database credentials, warehouse credentials, ad platform credentials, infrastructure secrets, or local environment files for normal Bounty CLI workflows.

## 3. Customer Responsibilities

Customer is responsible for Customer Data, Customer's users, and Customer's use of the service. Customer must:

- Have all rights, permissions, consents, notices, and legal bases needed to provide Customer Data to Bounty and connect third-party systems.
- Use Bounty only in compliance with applicable law, these Terms, and third-party provider terms.
- Configure connectors, permissions, data sources, fields, exports, and AI workflows appropriately for Customer's business.
- Review outputs, analyses, recommendations, and generated actions before relying on them.
- Ensure that Customer does not submit sensitive or regulated data unless authorized by the applicable agreement and Bounty's documented service capabilities. [TODO: confirm sensitive data policy.]

## 4. Customer Data

"Customer Data" means data, content, prompts, queries, files, credentials, configuration, outputs, and other information submitted to, connected to, generated through, or made available to Bounty by or on behalf of Customer.

Customer owns Customer Data. These Terms do not transfer ownership of Customer Data to Bounty.

Customer grants Bounty a limited license to process Customer Data only as needed to provide, secure, support, maintain, and improve the service; comply with law; and enforce these Terms. [TODO: confirm whether aggregated or deidentified usage data is used and how it is limited.]

## 5. AI Features And Outputs

Bounty may include AI chat, agents, generated actions, campaign analysis, and other AI-assisted features. AI outputs may be inaccurate, incomplete, outdated, or unsuitable for Customer's use case.

Customer is responsible for reviewing AI outputs before using them, including any recommended actions, analysis, code, data transformations, queries, summaries, or business decisions. Bounty does not provide legal, financial, tax, medical, or other professional advice.

[TODO: confirm model providers, whether prompts/outputs are retained, whether customer data is used for model training, and whether customers can configure AI data retention or opt-outs.]

## 6. Third-Party Integrations And Data Sources

Bounty may allow Customer to connect customer-authorized data sources and tools. Public docs currently describe connector examples including GA4, Meta Ads, Snowflake, Tinybird, and HubSpot.

When Customer connects a third-party system, Customer authorizes Bounty to access, process, and display data from that system according to Customer's configuration and permissions. Customer is responsible for its relationship with third-party providers, including provider terms, access permissions, data accuracy, credentials, rate limits, and revocation.

[TODO: confirm full supported integration list, including Google Ads, Customer.io, Apple Search Ads, and any destination/export integrations.]

## 7. Fees And Payment

Fees, subscription periods, payment terms, taxes, renewal terms, and usage limits will be stated in the applicable order form, checkout flow, invoice, pricing page, or other written agreement.

[TODO: confirm billing model, payment processor, taxes, renewal/non-renewal process, refunds, trials, and late payment terms.]

## 8. Fair Use And Acceptable Use

Customer must use Bounty consistently with normal business analytics and growth operations workflows.

Customer must not:

- Use Bounty for illegal, harmful, deceptive, abusive, or infringing activity.
- Attack, disrupt, overload, scan, probe, or test the vulnerability of Bounty systems without written authorization.
- Upload, transmit, or execute malware or harmful code.
- Attempt to bypass authentication, authorization, rate limits, usage limits, billing limits, or security controls.
- Reverse engineer, scrape, crawl, or extract the service except as allowed by law or written agreement.
- Share user credentials or permit access by unauthorized users.
- Use Bounty to send spam or unauthorized communications.
- Use the service in a way that harms Bounty, other customers, vendors, or third-party systems.

High-volume use of LLM features, sandboxed code execution, warehouse queries, syncs, API calls, exports, or email delivery may be throttled, delayed, limited, or disabled to protect the service, control costs, comply with provider limits, or prevent harm.

Bounty may contact Customer to reduce usage, upgrade to an appropriate plan, or agree custom limits. Bounty may suspend abusive or harmful use that risks the security, reliability, cost profile, or availability of the service or other customers.

## 9. Confidentiality

Each party may receive non-public information from the other party that is marked confidential or should reasonably be understood as confidential. The receiving party will use confidential information only to perform under these Terms and will protect it using reasonable care.

Confidential information does not include information that is publicly available without breach, already known without restriction, independently developed without use of confidential information, or lawfully received from a third party.

[TODO: confirm confidentiality exceptions, compelled disclosure process, and survival period.]

## 10. Intellectual Property

Bounty and its licensors own all rights in the service, software, documentation, designs, workflows, templates, models, and other Bounty technology. Customer receives only the rights expressly granted in these Terms.

Customer may provide feedback or suggestions. Bounty may use feedback without restriction or obligation. [TODO: confirm feedback terms.]

## 11. Service Changes And Availability

Bounty may update, modify, suspend, or discontinue parts of the service. Bounty will use reasonable efforts to avoid materially reducing core paid functionality during a subscription period. [TODO: confirm support commitments, SLA, uptime commitments, maintenance notice, and beta feature terms.]

## 12. Suspension And Termination

Bounty may suspend or terminate access if Customer breaches these Terms, fails to pay fees, creates security or legal risk, exceeds usage limits, or uses the service abusively.

Customer may stop using the service or terminate as stated in the applicable order form or subscription terms. [TODO: confirm termination process, account deletion, data export, and post-termination retention.]

## 13. Disclaimers

Except as expressly stated in a written agreement, the service is provided "as is" and "as available." Bounty disclaims warranties of merchantability, fitness for a particular purpose, non-infringement, and uninterrupted or error-free operation to the maximum extent permitted by law.

Bounty does not warrant that data from third-party integrations will be complete, accurate, timely, or available at all times.

## 14. Limitation Of Liability

[TODO: counsel to confirm liability cap, excluded damages, supercap, unlimited claims, and carveouts.]

Subject to the final agreed liability terms, neither party should be liable for indirect, incidental, special, consequential, exemplary, or punitive damages, or lost profits, revenues, goodwill, or data, to the extent permitted by law. [TODO: confirm final language.]

## 15. Indemnity

[TODO: counsel to confirm provider indemnity, customer indemnity, covered claims, defense process, settlement rights, and exclusions.]

## 16. Data Protection

The [Privacy Policy](/privacy) describes Bounty's privacy practices. The [Data Processing Addendum](/dpa) may apply when Bounty processes Customer Personal Data on behalf of Customer, but it is not effective until accepted through the applicable execution process. [TODO: confirm DPA execution mechanics.]

## 17. Governing Law And Disputes

These Terms are governed by [TODO: confirm governing law]. The parties consent to exclusive jurisdiction and venue in [TODO: confirm courts and venue].

[TODO: confirm arbitration, jury waiver, class waiver, injunctive relief, and notice requirements.]

## 18. Contact

Legal notices: [TODO: confirm legal contact email and mailing address]

Privacy requests: [TODO: confirm privacy contact email]

Security reports: [TODO: confirm security contact email or vulnerability disclosure process]
