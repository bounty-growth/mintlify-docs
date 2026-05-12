---
title: "Subprocessors"
description: "Draft subprocessor list for Bounty."
---

# Subprocessors

Last updated: May 12, 2026

**Draft - legal review required.** This Subprocessors page is a working draft for Bounty and has not yet been reviewed by legal counsel. It is provided as a non-binding indication of Bounty's intended subprocessor disclosures only. It is not a final subprocessor list or contractual notice unless and until it is reviewed, approved, and accepted through an authorized agreement process.

Bounty uses third-party vendors and subprocessors to provide, host, secure, monitor, analyze, and support the service. This page identifies vendors that may process Customer Personal Data or other Customer Data, depending on the customer's service configuration and authorized integrations.

For Bounty's broader vendor review process, see [Vendor Management](/vendor-management).

Customers can contact [arran@bountygrowth.com](mailto:arran@bountygrowth.com) with questions about subprocessors.

## Core Product Vendors

| Subprocessor | Purpose | Product function | Categories of data processed | Location / region | Use |
| --- | --- | --- | --- | --- | --- |
| Supabase | Authentication, database, and storage | User authentication, application database, file/object storage | Account data, authentication identifiers, workspace data, Customer Data, files/objects, and logs | Determined by Bounty's Supabase project configuration and Supabase processing locations | Core service |
| Vercel | Hosting and processing for the Bounty app and workflows | Web app hosting, deployments, routing, serverless/edge processing | User requests, IP/device data, app data in transit, logs, environment variables, and secrets | Determined by Bounty's deployment configuration and Vercel processing locations | Core service |
| Airbyte | Source and data integrations | Customer-authorized connector syncs and integration data movement | Source credentials/tokens, schema metadata, synced records, sync logs, and configuration metadata | Determined by Bounty's Airbyte configuration and Airbyte processing locations | Integration-dependent |
| OpenAI | AI features | AI chat, agents, analysis, summarization, generated actions, prompt/output processing | Prompts, Customer Data included in prompts, outputs, and usage metadata | Determined by OpenAI API processing locations and Bounty's account settings | AI features |
| E2B | Sandboxed code execution | Isolated code execution for analysis or workflow tasks | Code, inputs, customer-provided data, generated files, logs, and execution outputs | Determined by E2B processing locations and Bounty's account settings | Analysis features |
| ClickHouse | Analytics warehouse | Storage and querying of analytics/customer data | Customer source data, transformed analytics data, query results, schemas, metadata, and logs | Determined by Bounty's ClickHouse Cloud configuration and ClickHouse processing locations | Analytics features |
| PostHog | Product analytics and session recording | Product usage analytics, events, funnels, and session replay where enabled | User identifiers, product events, device/session metadata, page interactions, and recordings where enabled | Determined by Bounty's PostHog project configuration and PostHog processing locations | Product analytics |
| Sentry | Error monitoring | Error capture, diagnostics, stack traces, logs, and performance context | Error events, stack traces, request context, user identifiers if configured, source maps, and logs | Determined by Bounty's Sentry project configuration and Sentry processing locations | Monitoring |
| Resend | Email delivery | Transactional email delivery and email-related notifications | Recipient email addresses, names, message content, delivery metadata, and bounce/open/click data where enabled | Determined by Resend processing locations and Bounty's account settings | Email delivery |

## Customer-Configured Integrations

These vendors may process Customer Data only when a customer configures or authorizes the relevant integration.

| Subprocessor / integration | Purpose | Product function | Categories of data processed | Location / region | Use |
| --- | --- | --- | --- | --- | --- |
| Snowflake | Customer-configured warehouse integration | Connect to selected warehouse tables and make curated data sources available in Bounty | Warehouse credentials/tokens, schemas, table names, selected warehouse records, query results, and metadata | Determined by the customer's Snowflake account, warehouse region, and Bounty access path | Optional / customer-configured |
| Tinybird | Customer-configured analytics integration | Connect to available Tinybird tables and make curated data sources available in Bounty | API tokens, schemas, table names, records, query results, and metadata | Determined by the customer's Tinybird account and Bounty access path | Optional / customer-configured |
| GA4 | Customer-configured analytics source | Connect GA4 data for analysis and data sources | Analytics events, dimensions, metrics, identifiers, conversion data, and metadata | Determined by Google processing locations and the customer's GA4 configuration | Optional / customer-configured |
| Meta Ads | Customer-configured advertising source | Connect campaign, ad set, ad, and daily performance tables | Campaign/ad performance data, account identifiers, audience/reporting metadata, and conversion data | Determined by Meta processing locations and the customer's account configuration | Optional / customer-configured |
| HubSpot | Customer-configured CRM/source integration | Connect CRM or lifecycle data for analysis and data sources | Contact/company/deal data, lifecycle fields, interaction metadata, and identifiers | Determined by HubSpot processing locations and the customer's account configuration | Optional / customer-configured |
| Google Ads | Customer-configured advertising source | Connect campaign and performance data | Advertising account, campaign, keyword/ad, conversion, and reporting data | Determined by Google processing locations and the customer's account configuration | Optional / customer-configured |
| Customer.io | Customer-configured lifecycle/customer engagement source | Connect lifecycle, messaging, or customer event data | Contact profiles, event data, message metadata, and segments | Determined by Customer.io processing locations and the customer's account configuration | Optional / customer-configured |
| Apple Search Ads | Customer-configured advertising source | Connect campaign and app advertising performance data | Campaign/ad group/keyword performance, attribution data, and account identifiers | Determined by Apple processing locations and the customer's account configuration | Optional / customer-configured |

## Updates

Bounty may update this page as vendors, subprocessors, integrations, and processing activities change. Customers with contractual notice or objection rights receive those rights as described in their agreement with Bounty.
