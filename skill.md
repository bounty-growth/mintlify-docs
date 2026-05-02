---
name: bounty
description: |
  Bounty CLI gives AI agents a safe, authenticated marketing operations CLI for
  campaign performance, ads, creatives, generated actions, and agent workflows
  in the Bounty app.
license: Proprietary
compatibility: Requires Node.js 20 or later for the CLI. Works with AI coding agents that can load skill files.
metadata:
  product: Bounty
  package: bounty-cli
---

# Bounty CLI

`bounty-cli` helps marketing teams and AI agents inspect Bounty paid performance, creative fatigue, campaign details, generated actions, and agent workflows from the terminal.

## Install

Install the CLI skills and authenticate with browser login:

```bash
npx -y bounty-cli@latest init --all --browser
```

After install, restart the AI agent so it discovers the new skills.

## Verify

```bash
bounty-cli whoami
bounty-cli campaigns list --json
```

If the CLI is not authenticated:

```bash
bounty-cli login
```

## Choose A Skill

- Use `bounty-cli` for broad authenticated CLI workflows.
- Use `bounty-campaigns` for campaign lists, filters, and details.
- Use `bounty-ads` for ad-level inspection.
- Use `bounty-creatives` for creative analytics and fatigue.
- Use `bounty-actions` for generated action review.
- Use `bounty-agents` for agent definitions and context.
- Use `bounty-campaign-analysis` for prioritized findings on one campaign.

## Rules

- Use `--json` when output will be parsed, cited, or passed to another tool.
- Start with list commands, then use show or analyze commands for detail.
- Use explicit `--start-date` and `--end-date` values for performance questions.
- Do not ask for database, warehouse, ad platform, or infrastructure credentials.
