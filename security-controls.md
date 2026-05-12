---
title: "Security Controls"
description: "Draft security control summary for Bounty."
---

# Security Controls

Last updated: May 12, 2026

**Draft - legal review required.** This Security Controls page is a working draft for Bounty and has not yet been reviewed by legal counsel. It is provided as a non-binding indication of Bounty's intended security practices only. It is not a security certification, audit report, or contractual commitment unless and until it is reviewed, approved, and accepted through an authorized agreement process.

Bounty maintains security controls designed to protect customer data, personal data, product systems, credentials, source code, and internal information. These controls are reviewed as the service, vendors, integrations, and operating environment change.

## Security Contact

Security issues can be reported to [arran@bountygrowth.com](mailto:arran@bountygrowth.com).

## Authentication And Access

Bounty uses Supabase Auth for product authentication and authorization. The product login flow supports password-based login and magic-link authentication. Google OAuth may be enabled where configured.

Okta SSO can be supported on request through Supabase Auth's SAML 2.0 SSO support. SSO requires customer-specific configuration and testing.

Customer access is scoped through application authorization and database-level tenant isolation. Customer users are authorized only for their organization's data and permitted product workflows.

## Enterprise MFA

Bounty requires MFA for key production and administrative systems. Administrative access is limited to authorized personnel based on business need.

## Password-Based Login

Where password-based login is used:

- Passwords of at least 64 characters are supported.
- Supabase Auth supports passwords up to 72 characters due to bcrypt limits.
- Password requirements do not dictate character choices. Bounty does not require specific numbers, symbols, uppercase letters, or lowercase letters.
- Bounty does not use security questions.
- Password reset is performed through an email-based recovery link.
- Password reset requires access to the user's email recovery link before a new password can be set.
- Password storage is handled by Supabase Auth, which uses bcrypt, a salted CPU-hard one-way password hash.

Bounty can disable password and email login for a customer when required by the customer's authentication configuration.

## Data Protection

Primary product application data is stored in Supabase Postgres and protected with encryption in transit and at rest by the underlying infrastructure provider.

Bounty generally relies on infrastructure-provider encryption rather than applying separate application-level encryption before inserting product data. Data is encrypted in transit and at rest by infrastructure providers such as Supabase where applicable.

Generated charts, reports, action artifacts, and related product files may be stored in Supabase Storage or other product infrastructure as needed to provide the service.

## Backups

Primary product application data is stored in Supabase Postgres. Supabase provides managed automatic database backups for hosted projects.

Backup and restore access is restricted to authorized administrators through Supabase access controls. Bounty does not store database backups in public repositories.

Customer source data may also be recoverable by re-syncing from the original source where applicable.

## Vulnerability Reporting And Patch Management

Security fixes are handled through Bounty's standard code change and deployment process, including:

- Private vulnerability reporting.
- Pull request review.
- CI validation.
- Production deployment through Vercel and GitHub workflows.
- Database security fixes represented as checked-in Supabase migrations.

Bounty triages security issues based on severity, exploitability, affected systems, and customer impact. Remediation is tracked through the same engineering workflow used for product and infrastructure changes.

## Security Testing

Bounty uses code review, automated checks, dependency review, infrastructure controls, monitoring, and focused security review to identify and remediate security issues. Third-party assessments may be performed based on customer commitments, product maturity, and risk.

## Vendor And Subprocessor Review

Bounty uses a risk-based vendor management process. Vendors that process customer data or support critical product operations are reviewed before onboarding where practical and periodically thereafter.

See:

- [Vendor Management](/vendor-management)
- [Subprocessors](/subprocessors)

## Legal And Privacy Documentation

Legal, privacy, and data protection resources are available here:

- [Legal](/legal)
- [Privacy Policy](/privacy)
- [Terms of Service](/terms)
- [Data Processing Addendum](/dpa)
- [Subprocessors](/subprocessors)
