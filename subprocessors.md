---
title: "Subprocessors"
description: "Subprocessor list for Bounty."
---

Last updated: August 26, 2026

Bounty uses third-party vendors and subprocessors to provide, host, secure, monitor, analyze, and support the service. This page identifies vendors that may process Customer Personal Data or other Customer Data, depending on the customer's service configuration and authorized integrations.

For Bounty's broader vendor review process, see [Vendor Management](/vendor-management).

Customers can contact [arran@bountygrowth.com](mailto:arran@bountygrowth.com) with questions about subprocessors.

The **Countries where data may be processed** columns declare where Customer Data may be stored, accessed remotely, or otherwise processed, including confirmed downstream processing. They do not identify a processor's registered address or country of registration, and do not represent an exhaustive list of each provider's global operations.

## Core Product Vendors

| Subprocessor | Purpose | Product function | Categories of data processed | Countries where data may be processed | Use |
| --- | --- | --- | --- | --- | --- |
| Supabase Inc. | Authentication, database, and storage | User authentication, application database, file/object storage | Account data, authentication identifiers, workspace data, Customer Data, files/objects, and logs | United States of America (Bounty's primary project data store); Supabase subprocessors may process data in the United States of America and Singapore | Core service |
| Vercel, Inc. | Hosting and processing for the Bounty app and workflows | Web app hosting, deployments, routing, serverless/edge processing | User requests, IP/device data, app data in transit, logs, environment variables, and secrets | United States of America (primary); other locations may apply based on Bounty's deployment configuration and Vercel subprocessors | Core service |
| Trigger.dev (API Hero Ltd) | Background job orchestration and managed task execution | Scheduled and asynchronous notebook, dataset, attribution, integration sync, and workflow tasks | Task payloads and tags, organization/dataset/notebook/model/run identifiers, Customer Data accessed or transformed during execution, task outputs, logs, errors, and execution metadata | United Kingdom and United States of America; Trigger.dev subprocessors may also process data in the European Union | Core background processing |
| Airbyte | Source and data integrations | Customer-authorized connector syncs and integration data movement | Source credentials/tokens, schema metadata, synced records, sync logs, and configuration metadata | Determined by Bounty's Airbyte configuration and Airbyte processing locations | Integration-dependent |
| OpenAI | AI inference | Customer-visible chat, agents, analysis, summarization, and generated actions | Prompts, de-identified Customer Data included in prompts, outputs, and usage metadata | OpenAI OpCo, LLC: United States of America. OpenAI service subprocessors may process Customer Data in Australia, Brazil, Canada, Finland, France, Germany, India, Indonesia, Ireland, Italy, Japan, Malaysia, Mexico, Netherlands, Norway, Philippines, Poland, Singapore, South Africa, South Korea, Spain, Sweden, Switzerland, United Arab Emirates, United Kingdom, and the United States of America | AI features; submitted customer data is not used to train OpenAI's general models |
| Anthropic | AI inference | Customer-visible analysis, agent, and language-model workflows where enabled | Prompts, de-identified Customer Data included in prompts, outputs, and usage metadata | Determined by Anthropic API processing locations and Bounty's account settings | AI features; submitted customer data is not used to train Anthropic's general models |
| E2B | Sandboxed code execution | Isolated code execution for analysis or workflow tasks | Code, inputs, customer-provided data, generated files, logs, and execution outputs | Determined by E2B processing locations and Bounty's account settings | Analysis features |
| ClickHouse | Analytics warehouse | Storage and querying of analytics/customer data | Customer source data, transformed analytics data, query results, schemas, metadata, and logs | Determined by Bounty's ClickHouse Cloud configuration and ClickHouse processing locations | Analytics features |
| PostHog | Product analytics and session recording | Product usage analytics, events, funnels, and session replay where enabled | User identifiers, product events, device/session metadata, page interactions, and recordings where enabled | Determined by Bounty's PostHog project configuration and PostHog processing locations | Product analytics |
| Sentry | Error monitoring | Error capture, diagnostics, stack traces, logs, and performance context | Error events, stack traces, request context, user identifiers if configured, source maps, and logs | Determined by Bounty's Sentry project configuration and Sentry processing locations | Monitoring |
| Resend | Email delivery | Transactional email delivery and email-related notifications | Recipient email addresses, names, message content, delivery metadata, and bounce/open/click data where enabled | Determined by Resend processing locations and Bounty's account settings | Email delivery |

## Customer-Configured Integrations

These vendors may process Customer Data only when a customer configures or authorizes the relevant integration.

| Subprocessor / integration | Purpose | Product function | Categories of data processed | Countries where data may be processed | Use |
| --- | --- | --- | --- | --- | --- |
| Snowflake | Customer-configured warehouse integration | Connect to selected warehouse tables and make curated data sources available in Bounty | Warehouse credentials/tokens, schemas, table names, selected warehouse records, query results, and metadata | Determined by the customer's Snowflake account, warehouse region, and Bounty access path | Optional / customer-configured |
| Tinybird | Customer-configured analytics integration | Connect to available Tinybird tables and make curated data sources available in Bounty | API tokens, schemas, table names, records, query results, and metadata | Determined by the customer's Tinybird account and Bounty access path | Optional / customer-configured |
| GA4 | Customer-configured analytics source | Authorize GA4, select properties, and support activated customer data workflows | Property metadata and, when activated, analytics dimensions, metrics, identifiers, conversion data, and reporting data | Determined by Google processing locations and the customer's GA4 configuration | Optional / customer-configured |
| Meta Ads | Customer-configured advertising source | Connect campaign, ad set, ad, and daily performance tables | Campaign/ad performance data, account identifiers, audience/reporting metadata, and conversion data | Determined by Meta processing locations and the customer's account configuration | Optional / customer-configured |
| HubSpot | Customer-configured CRM/source integration | Connect CRM or lifecycle data for analysis and data sources | Contact/company/deal data, lifecycle fields, interaction metadata, and identifiers | Determined by HubSpot processing locations and the customer's account configuration | Optional / customer-configured |
| Google Ads | Customer-configured advertising source | Authorize Google Ads, select advertiser accounts, and support activated customer data workflows | Account metadata and, when activated, campaign, keyword/ad, conversion, and reporting data | Determined by Google processing locations and the customer's account configuration | Optional / customer-configured |
| Google Search Console | Customer-configured search analytics source | Authorize read-only Search Console access, select domain or URL-prefix properties, and synchronize finalized daily search performance | Property identifiers, query and canonical page dimensions, clicks, impressions, click-through rate, and average position | Determined by Google processing locations and the customer's Search Console configuration | Optional / customer-configured |
| Customer.io | Customer-configured lifecycle/customer engagement source | Connect lifecycle, messaging, or customer event data | Contact profiles, event data, message metadata, and segments | Determined by Customer.io processing locations and the customer's account configuration | Optional / customer-configured |
| Apple Search Ads | Customer-configured advertising source | Connect campaign and app advertising performance data | Campaign/ad group/keyword performance, attribution data, and account identifiers | Determined by Apple processing locations and the customer's account configuration | Optional / customer-configured |

## Updates

Bounty may update this page as vendors, subprocessors, integrations, and processing activities change. Customers with contractual notice or objection rights receive those rights as described in their agreement with Bounty.

Google-derived data sent to an AI subprocessor is de-identified and used only to return the customer-requested feature. Bounty may use Google-derived data for an organization-specific model or model artifact, but never for generalized, foundational, pooled, or cross-customer training.
