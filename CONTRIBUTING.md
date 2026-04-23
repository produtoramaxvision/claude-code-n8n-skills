# Contributing

Thanks for your interest in contributing!

## Scope of This Repository

**In scope:**
- Plugin packaging improvements (`.claude-plugin/` manifests)
- CI / tooling / repository hygiene
- Documentation fixes
- Bug reports about plugin installation or discovery

**Out of scope (upstream):**
- Changes to skill content under `skills/`. These are imported verbatim from [czlonkowski/n8n-skills](https://github.com/czlonkowski/n8n-skills). Open issues/PRs there instead.

## Commit Convention

We follow [Conventional Commits 1.0](https://www.conventionalcommits.org/):

```
<type>(<scope>): <description>
```

**Types:** `feat`, `fix`, `docs`, `chore`, `ci`, `refactor`, `test`, `perf`.

**Examples:**

```
feat(marketplace): add maxvision-skills marketplace.json
fix(ci): correct markdownlint glob pattern
docs(readme): fix broken link to upstream repo
chore(upstream): sync skills to czlonkowski/n8n-skills v1.7.0
```

## Semver

- `feat` → MINOR bump (`0.1.0` → `0.2.0`)
- `fix` → PATCH bump (`0.1.0` → `0.1.1`)
- `BREAKING CHANGE:` footer → MAJOR bump (`0.9.0` → `1.0.0`)

## Pull Request Process

1. Fork and create a feature branch off `main`: `git checkout -b feat/short-description`
2. Make your changes.
3. Ensure CI passes locally (see `.github/workflows/validate.yml` for the jobs).
4. Update `CHANGELOG.md` under an `## [Unreleased]` section.
5. Open a PR with a clear description. Link any related issue.

## Code of Conduct

All contributors are expected to follow the [Contributor Covenant](CODE_OF_CONDUCT.md).
