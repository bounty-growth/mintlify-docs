---
title: "Security Controls"
description: "Draft security control summary for Bounty."
---

# Security Controls

**Draft - security and legal review required.** This page is a working draft for Bounty Growth / Bounty and must be reviewed before publication or use in customer security questionnaires.

Last updated: [TODO: confirm publication date]

## Current Status

Bounty is formalizing its security and privacy documentation for customer review. Some controls described below are implemented today, while others are in progress and will be confirmed before this page is used as final customer-facing security collateral.

Open items before final publication:

- Complete the enterprise application MFA audit.
- Confirm the final vendor management review cadence.
- Confirm the public subprocessor list and DPA with legal counsel.
- Finalize the written patch management policy, including severity-based remediation targets.
- Confirm whether broader security collateral should remain public or be shared under NDA.

## Security Contact

Security issues can be reported to [arran@bountygrowth.com](mailto:arran@bountygrowth.com).

[TODO: confirm whether a dedicated security email, disclosure policy, or vulnerability intake process will replace this contact.]

## Authentication And Access

Bounty uses Supabase Auth for product authentication and authorization. The current product login flow supports password-based login and magic-link authentication. Google OAuth may be enabled where configured.

Okta SSO can be supported on request through Supabase Auth's SAML 2.0 SSO support. Okta SSO is not enabled by default in the current login flow and requires customer-specific configuration and testing.

Customer access is scoped through application authorization and database-level tenant isolation. Customer users should only access their organization's data.

## Enterprise MFA

Bounty requires MFA for key production and administrative systems and is completing a full enterprise application MFA audit.

Before this page is used as final customer-facing collateral, Bounty expects to confirm MFA enforcement across enterprise applications and remediate any gaps identified.

## Password-Based Login

Where password-based login is used:

- Passwords of at least 64 characters are supported.
- Supabase Auth currently supports passwords up to 72 characters due to bcrypt limits.
- Password requirements do not dictate character choices. Bounty does not require specific numbers, symbols, uppercase letters, or lowercase letters.
- Bounty does not use security questions.
- Password reset is performed through an email-based recovery link.
- Password reset requires access to the user's email recovery link before a new password can be set.
- Password storage is handled by Supabase Auth, which uses bcrypt, a salted CPU-hard one-way password hash.

Bounty can disable password and email login for a customer if required. [TODO: confirm operational process and lead time.]

## Data Protection

Primary product application data is stored in Supabase Postgres and protected with encryption in transit and at rest by the underlying infrastructure provider.

Bounty does not generally apply application-level encryption before inserting product data. Data is encrypted in transit and at rest by infrastructure providers such as Supabase where applicable.

Some generated charts and action artifacts are stored in Supabase Storage. [TODO: confirm whether artifact buckets remain public, move to private buckets, or are served through authenticated/signed access before final publication.]

## Backups

Primary product application data is stored in Supabase Postgres. Supabase provides managed automatic database backups for hosted projects.

Backup and restore access is restricted to authorized administrators through Supabase access controls. Bounty does not store database backups in public repositories.

Customer source data may also be recoverable by re-syncing from the original source where applicable.

[TODO: do not claim point-in-time recovery or restore drill completion until verified.]

## Vulnerability Reporting And Patch Management

Security fixes are handled through Bounty's standard code change and deployment process, including:

- Private vulnerability reporting.
- Pull request review.
- CI validation.
- Production deployment through Vercel and GitHub workflows.
- Database security fixes represented as checked-in Supabase migrations.

Bounty is formalizing the written patch management policy, including severity-based remediation targets, before final submission of this collateral.

## Third-Party Penetration Testing

Bounty does not currently conduct third-party penetration tests on a recurring cadence.

Bounty plans to begin annual third-party penetration testing of the product/service starting **November 1, 2026**. Findings will be tracked and remediated according to severity.

## Vendor And Subprocessor Review

Bounty uses and is formalizing a risk-based vendor management process. Vendors that process customer data or support critical product operations are prioritized for diligence.

See:

- [Vendor Management](/vendor-management)
- [Subprocessors](/subprocessors)

[TODO: confirm final annual review cadence before stating that all vendors or all subprocessors are reviewed annually.]

## Legal And Privacy Documentation

Draft legal and privacy documents are available for review:

- [Legal](/legal)
- [Privacy Policy](/privacy)
- [Terms of Service](/terms)
- [Data Processing Addendum](/dpa)
- [Subprocessors](/subprocessors)

These drafts require legal review before they are treated as final, binding, or incorporated into customer agreements.
