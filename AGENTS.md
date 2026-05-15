# Repository Instructions

## Public Docs Privacy

Never mention customer-specific, organization-specific, account-specific, or prospect-specific names in public documentation examples. Use generic examples such as "a GA4 connection", "a Snowflake connection", "a retail brand", or "an example workspace" instead.

Do not reuse private names from prompts, tickets, databases, logs, screenshots, branches, commits, or local test data in docs unless the user explicitly says the material is for private/internal documentation and asks for those names to appear.

## Mintlify Page Headers

Mintlify renders each page's frontmatter `title` and `description` as the page header. Do not repeat the page title as a top-level heading or opening subsection in the MDX body, especially under `/legal`.

Never paste agent discovery boilerplate into page content, including headings or text such as "Documentation Index", "Fetch the complete documentation index", or references instructing agents to use `llms.txt`. That material is context for agents, not public documentation copy.

When adding or reviewing MDX pages, check the first visible body content after frontmatter. It should begin with the actual page copy or a real subsection, not another copy of the title and not agent-only index instructions.
