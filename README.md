# Claude Code N8N Skills

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Validate](https://github.com/produtoramaxvision/claude-code-n8n-skills/actions/workflows/validate.yml/badge.svg)](https://github.com/produtoramaxvision/claude-code-n8n-skills/actions/workflows/validate.yml)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)
[![Upstream: czlonkowski/n8n-skills](https://img.shields.io/badge/upstream-czlonkowski%2Fn8n--skills%20v1.6.0-green)](https://github.com/czlonkowski/n8n-skills)

> 7 expert skills for building flawless n8n workflows in Claude Code.

Self-hosted Claude Code plugin packaging the excellent [czlonkowski/n8n-skills](https://github.com/czlonkowski/n8n-skills) by Romuald Członkowski, with the full professional repository scaffolding needed for reliable consumption in production environments.

---

## Skills Included

| Skill | Purpose |
|---|---|
| `n8n-code-javascript` | Write JavaScript in n8n Code nodes (data access, helpers, DateTime, error prevention) |
| `n8n-code-python` | Write Python in n8n Code nodes (standard library, patterns, errors) |
| `n8n-expression-syntax` | Validate `{{ }}` expression syntax, `$json`/`$node` access, webhook body structure |
| `n8n-mcp-tools-expert` | Use n8n-mcp MCP tools effectively (search, validate, templates, workflows) |
| `n8n-node-configuration` | Configure nodes correctly (operation patterns, dependencies) |
| `n8n-validation-expert` | Interpret validation errors and fix them (error catalog, false positives) |
| `n8n-workflow-patterns` | Proven architectural patterns (webhooks, APIs, DBs, AI agents, scheduled tasks) |

---

## Installation

### Option 1: via Marketplace (recommended)

In Claude Code, run:

```
/plugin marketplace add produtoramaxvision/claude-code-n8n-skills
/plugin install n8n-skills@maxvision-skills
```

### Option 2: Manual clone (user scope)

```bash
git clone https://github.com/produtoramaxvision/claude-code-n8n-skills.git \
  ~/.claude/plugins/claude-code-n8n-skills
```

Then restart Claude Code. The 7 skills appear automatically.

---

## Usage

Skills activate automatically when you mention n8n-related tasks. Explicit triggers:

- "Write JavaScript for an n8n Code node that..." → `n8n-code-javascript`
- "Validate this n8n expression..." → `n8n-expression-syntax`
- "Build an n8n workflow that..." → `n8n-workflow-patterns`

No manual skill invocation required — Claude Code loads skill metadata on startup and triggers skills based on task description matching.

---

## Requirements

- Claude Code ≥ 2.0 (for plugin support)
- Optional: [n8n-mcp](https://github.com/czlonkowski/n8n-mcp) MCP server for the `n8n-mcp-tools-expert` skill to be fully actionable

---

## Attribution

This plugin is a derivative work of [czlonkowski/n8n-skills](https://github.com/czlonkowski/n8n-skills) by **Romuald Członkowski**, licensed under MIT.

All skill content under `skills/` is verbatim from upstream v1.6.0. Modifications by MaxVision are limited to plugin packaging and repository scaffolding. See [NOTICE](NOTICE) for full attribution and [LICENSE](LICENSE) for the dual-copyright MIT terms.

---

## Contributing

Pull requests welcome for:

- Packaging improvements (CI, docs, metadata)
- Bug reports for plugin loading issues

**Skill content changes should be proposed upstream at [czlonkowski/n8n-skills](https://github.com/czlonkowski/n8n-skills).** This repo resyncs periodically from upstream via the sync mechanism documented in the workspace (not in this public repo).

See [CONTRIBUTING.md](CONTRIBUTING.md) for commit conventions and PR guidelines.

---

## Security

Report vulnerabilities privately via the process in [SECURITY.md](SECURITY.md). **Do not open public issues for security concerns.**

---

## License

Dual-copyright MIT License. See [LICENSE](LICENSE).

- Original work © Romuald Członkowski
- Plugin packaging and modifications © 2026 Produtora MaxVision
