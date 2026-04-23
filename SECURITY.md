# Security Policy

## Reporting a Vulnerability

**Do NOT open a public GitHub issue for security vulnerabilities.**

Instead, email: **produtoramaxvision@gmail.com** with the subject line:
`[SECURITY] claude-code-n8n-skills: <short description>`

Include:

- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Suggested fix (if any)

We will acknowledge receipt within **48 hours** and provide a timeline for a fix.

## Scope

This repository contains only markdown documentation and JSON manifests — no executable plugin code. Security concerns would typically fall into:

- Malicious content injected into a skill file that could influence Claude's behavior in harmful ways
- Supply-chain risks in CI/CD workflows
- Credential/PII exposure in committed files

For vulnerabilities in the underlying skill content (the educational MD files), please also consider reporting to the upstream project: [czlonkowski/n8n-skills](https://github.com/czlonkowski/n8n-skills/security).

## Supported Versions

| Version | Security fixes |
|---------|----------------|
| 0.x     | Latest minor only |

## Disclosure Policy

We follow coordinated disclosure with a **90-day** window. Public announcement happens after a patch is released.
