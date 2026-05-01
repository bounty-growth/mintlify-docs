# Bounty Docs

Public Mintlify documentation for Bounty's marketing operations CLI and AI agent skills.

## Local Preview

```bash
npm i -g mint
mint dev
```

## Validate

```bash
mint validate
mint broken-links
```

## Public Safety

Keep implementation details, private infrastructure names, customer data, and internal runbooks out of this repository.

Custom agent skills live in `.mintlify/skills/`. Do not symlink skills from private repositories into this repo; copy only audited, public-safe skill files.
