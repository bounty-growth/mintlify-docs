---
title: "Subprocessors"
description: "Draft subprocessor list for Bounty."
---

# Subprocessors

**Draft - legal review required.** This page is a working draft for Bounty and must be reviewed by legal counsel before publication. It starts with likely vendors identified for confirmation. Do not treat this as a final or complete subprocessor list until each TODO has been resolved.

Last updated: [TODO: confirm publication date]

## About This Page

Bounty may use third-party vendors and subprocessors to provide, host, secure, monitor, analyze, and support the service. This page lists vendors that may process Customer Personal Data or other Customer Data.

For Bounty's broader draft vendor inventory and risk-based review process, see [Vendor Management](/vendor-management). [TODO: confirm whether vendor management details should be public, private, or customer-confidential.]

[TODO: confirm whether this page is incorporated into customer agreements, the DPA, or both.]

[TODO: confirm change notification period, such as 10 business days, and customer objection process.]

Customers can contact [TODO: confirm privacy contact email] or [TODO: confirm security contact email] with questions.

## Core Or Likely Product Vendors

| Subprocessor | Purpose | Product function | Categories of data processed | Location / region | Mandatory or optional | Vendor trust / privacy page |
| --- | --- | --- | --- | --- | --- | --- |
| Supabase | [TODO: confirm] Authentication, database, and storage | User authentication, application database, file/object storage | Account data, authentication identifiers, workspace data, Customer Data, files/objects, logs [TODO: confirm] | [TODO: confirm Supabase project region(s) and processing locations] | [TODO: confirm mandatory/core] | [Supabase security docs](https://supabase.com/docs/guides/security) |
| Vercel | [TODO: confirm] Hosting and processing for the Next.js app and workflows | Web app hosting, deployments, routing, serverless/edge processing | User requests, IP/device data, app data in transit, logs, environment variables/secrets [TODO: confirm] | [TODO: confirm deployment regions and Vercel processing locations] | [TODO: confirm mandatory/core] | [Vercel Security](https://vercel.com/security) |
| Airbyte | [TODO: confirm] Source and data integrations | Customer-authorized connector syncs and integration data movement | Source credentials/tokens, schema metadata, synced records, sync logs, configuration metadata [TODO: confirm] | [TODO: confirm Airbyte Cloud region/data residency] | [TODO: confirm whether mandatory for integrations or optional/configuration-specific] | [Airbyte Cloud security](https://support.airbyte.com/hc/en-us/articles/15947202218907-Securing-Airbyte-Cloud) |
| OpenAI | [TODO: confirm] LLM features | AI chat, agents, analysis, summarization, generated actions, prompt/output processing | Prompts, Customer Data included in prompts, outputs, usage metadata [TODO: confirm] | [TODO: confirm API processing/storage region and retention settings] | [TODO: confirm mandatory for AI features] | [OpenAI security and privacy](https://openai.com/security-and-privacy/) |
| E2B | [TODO: confirm] Sandboxed Python/code execution | Isolated code execution for analysis or workflow tasks | Code, inputs, customer-provided data, generated files, logs, execution outputs [TODO: confirm] | [TODO: confirm E2B processing region] | [TODO: confirm mandatory for sandbox/code features] | [E2B Privacy Policy](https://e2b.dev/privacy) |
| ClickHouse | [TODO: confirm] Analytics warehouse | Storage and querying of analytics/customer data | Customer source data, transformed analytics data, query results, schemas, metadata, logs [TODO: confirm] | [TODO: confirm ClickHouse Cloud region(s)] | [TODO: confirm mandatory/core analytics warehouse] | [ClickHouse Trust Center](https://trust.clickhouse.com/) |
| PostHog | [TODO: confirm] Product analytics and session recording | Product usage analytics, events, funnels, session replay if enabled | User identifiers, product events, device/session metadata, page interactions, recordings if enabled [TODO: confirm masking/redaction] | [TODO: confirm PostHog project region, EU/US hosting, and recording storage] | [TODO: confirm mandatory or optional analytics/session recording] | [PostHog Trust Center](https://trust.posthog.com/) |
| Sentry | [TODO: confirm] Error monitoring | Error capture, diagnostics, stack traces, logs, performance context | Error events, stack traces, request context, user identifiers if configured, source maps, logs [TODO: confirm scrubbing] | [TODO: confirm Sentry processing region/account configuration] | [TODO: confirm mandatory/core monitoring] | [Sentry Security](https://sentry.io/security/) |
| Resend | [TODO: confirm] Email delivery | Transactional email delivery and email-related notifications | Recipient email addresses, names, message content, delivery metadata, bounce/open/click data if enabled [TODO: confirm] | [TODO: confirm Resend processing region] | [TODO: confirm mandatory for email delivery] | [Resend Security](https://resend.com/security) |

## Customer-Configured / Optional Integrations

These vendors may process Customer Data only when Customer configures or authorizes the relevant integration. [TODO: confirm whether any are also used as core infrastructure.]

| Subprocessor / integration | Purpose | Product function | Categories of data processed | Location / region | Mandatory or optional | Vendor trust / privacy page |
| --- | --- | --- | --- | --- | --- | --- |
| Snowflake | Customer-configured warehouse integration | Connect to selected warehouse tables and make curated data sources available in Bounty | Warehouse credentials/tokens [TODO: confirm], schemas, table names, selected warehouse records, query results, metadata | [TODO: confirm customer Snowflake region and Bounty access path] | Optional / customer-configured | [Snowflake Privacy Notice](https://www.snowflake.com/en/legal/privacy/privacy-policy/) |
| Tinybird | Customer-configured analytics integration | Connect to available Tinybird tables and make curated data sources available in Bounty | API tokens [TODO: confirm], schemas, table names, records, query results, metadata | [TODO: confirm customer Tinybird region and Bounty access path] | Optional / customer-configured | [Tinybird Security](https://guides.tinybird.co/security) |
| GA4 | Customer-configured analytics source | Connect GA4 data for analysis and data sources | Analytics events, dimensions, metrics, identifiers, conversion data, metadata [TODO: confirm] | [TODO: confirm Google/GA4 processing locations and Bounty access path] | Optional / customer-configured | [TODO: add vendor trust/privacy page] |
| Meta Ads | Customer-configured advertising source | Connect campaign, ad set, ad, and daily performance tables | Campaign/ad performance data, account identifiers, audience/reporting metadata, conversion data [TODO: confirm] | [TODO: confirm Meta processing locations and Bounty access path] | Optional / customer-configured | [TODO: add vendor trust/privacy page] |
| HubSpot | Customer-configured CRM/source integration | Connect CRM or lifecycle data for analysis and data sources | Contact/company/deal data, lifecycle fields, interaction metadata, identifiers [TODO: confirm] | [TODO: confirm HubSpot processing locations and Bounty access path] | Optional / customer-configured | [TODO: add vendor trust/privacy page] |
| Google Ads | [TODO: confirm support] Customer-configured advertising source | Campaign and performance data | Advertising account, campaign, keyword/ad, conversion, and reporting data [TODO: confirm] | [TODO: confirm] | Optional / customer-configured if supported | [TODO: add vendor trust/privacy page] |
| Customer.io | [TODO: confirm support] Customer-configured lifecycle/customer engagement source | Lifecycle, messaging, or customer event data | Contact profiles, event data, message metadata, segments [TODO: confirm] | [TODO: confirm] | Optional / customer-configured if supported | [TODO: add vendor trust/privacy page] |
| Apple Search Ads | [TODO: confirm support] Customer-configured advertising source | Campaign and app advertising performance data | Campaign/ad group/keyword performance, attribution data, account identifiers [TODO: confirm] | [TODO: confirm] | Optional / customer-configured if supported | [TODO: add vendor trust/privacy page] |

## Updates

We may update this page as vendors, subprocessors, and integrations change.

[TODO: confirm whether Bounty will provide advance notice of new subprocessors, the notice period, customer objection rights, and how customers subscribe to updates.]
