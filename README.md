<div align="center">
  <img src="assets/banner.svg" alt="claude-marketplace — Skills, workflows, and tools for Claude Code." width="800"/>
</div>

<div align="center">

A Claude Code plugin marketplace with skills for git workflows, code quality, safety, and more.

[![PR Validation](https://github.com/jzills/Claude-Marketplace/actions/workflows/pr.yml/badge.svg)](https://github.com/jzills/Claude-Marketplace/actions/workflows/pr.yml)
[![CodeQL](https://github.com/jzills/Claude-Marketplace/actions/workflows/codeql.yml/badge.svg)](https://github.com/jzills/Claude-Marketplace/actions/workflows/codeql.yml)
![Plugins](https://img.shields.io/badge/plugins-7-D97757?style=flat-square&labelColor=21262d)

</div>

## Getting started

Add this marketplace to Claude Code:

```shell
/plugin marketplace add jzills/claude-marketplace
```

Then install any plugin you need — see the full list below.

## Plugins

### Git & Workflow

| Plugin | Description | Install |
|--------|-------------|---------|
| `conventional-commits` | Enforces Conventional Commits format and branch naming when creating branches or committing | `/plugin install conventional-commits@jzills` |
| `github-pr` | Creates GitHub pull requests using the gh CLI with auto-generated titles and descriptions | `/plugin install github-pr@jzills` |

### Testing

| Plugin | Description | Install |
|--------|-------------|---------|
| `dotnet-unit-tests` | Writes production-quality NUnit + Moq unit tests for C# / .NET code | `/plugin install dotnet-unit-tests@jzills` |
| `pep8-python` | Enforces PEP 8 style conventions for Python code | `/plugin install pep8-python@jzills` |

### Safety & Auditing

| Plugin | Description | Install |
|--------|-------------|---------|
| `shimmering-forest` | CVSS v3.1-inspired risk auditor that scores every tool call and blocks or warns based on configurable thresholds | `/plugin install shimmering-forest@jzills` |

### Skill Management

| Plugin | Description | Install |
|--------|-------------|---------|
| `skill-changelog` | Maintains a versioned CHANGELOG.md inside any skill directory being created or modified | `/plugin install skill-changelog@jzills` |
| `auto-rewind` | Detects test failures and guides a `/rewind` to a clean checkpoint instead of fixing forward | `/plugin install auto-rewind@jzills` |

## Maintenance

**Update all plugins:**

```shell
/plugin marketplace update jzills
```

**Validate plugin structure:**

```shell
claude plugin validate .
```
