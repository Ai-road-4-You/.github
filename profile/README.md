<div align="center">

# 🛣️ Ai-road-4-You

**Shared Platform · CI/CD · Governance · Templates**

*Central enablement org for [iAiFy](https://github.com/enterprises/iAiFy) enterprise*

[![Location](https://img.shields.io/badge/📍-Stockholm,_Sweden-blue)]()
[![Repos](https://img.shields.io/badge/repos-5-green)]()
[![Enterprise](https://img.shields.io/badge/enterprise-iAiFy-purple)]()

</div>

---

## What We Build

Ai-road-4-You is the backbone of the iAiFy enterprise. Everything that's shared across organizations lives here — CI/CD workflows, governance policies, repository templates, and cross-org automation.

### 🏗️ Projects

| Project | Description | Status |
|---------|-------------|--------|
| **[enterprise-ci-cd](https://github.com/Ai-road-4-You/enterprise-ci-cd)** | 16 shared CI/CD workflows + 4 reusable actions for all iAiFy repos | ✅ Active |
| **[github-actions](https://github.com/Ai-road-4-You/github-actions)** | 13 composite GitHub Actions — deploy, test, lint, security scan | ✅ Active |
| **[governance](https://github.com/Ai-road-4-You/governance)** | Enterprise governance standards, policies, and compliance templates | ✅ Active |
| **[repo-templates](https://github.com/Ai-road-4-You/repo-templates)** | Repository bootstrap templates for new iAiFy projects | ✅ Active |
| **[fork-sync](https://github.com/Ai-road-4-You/fork-sync)** | Automated upstream sync for all managed forks across the enterprise | ✅ Active |

### What This Org Provides

```
Ai-road-4-You/
│
├── enterprise-ci-cd/         → Shared workflows consumed by all orgs
│   ├── 16 reusable workflows
│   ├── 4 composite actions
│   └── Deployment templates
│
├── github-actions/           → Composite actions library
│   ├── deploy/
│   ├── test/
│   ├── lint/
│   └── security-scan/
│
├── governance/               → Enterprise policies
│   ├── Branch protection rules
│   ├── Security policies
│   ├── PR templates
│   └── Compliance standards
│
├── repo-templates/           → New repo scaffolding
│   ├── CLAUDE.md
│   ├── copilot-instructions.md
│   ├── AGENTS.md
│   ├── dependabot.yml
│   └── GitHub Actions workflows
│
└── fork-sync/                → Upstream sync automation
    └── Cron-based fork updates
```

### Enterprise Governance

| Policy | Coverage |
|--------|----------|
| **Branch protection** | All 72 repos — PR required, no force push, no deletion |
| **Secret scanning** | Enabled on all repos with push protection |
| **Dependabot** | Security updates + version updates on all repos |
| **CodeQL** | Code scanning on 39 repos with supported languages |
| **Custom agents** | 16 Copilot coding agents deployed to all repos |
| **CODEOWNERS** | Defined on all repos |
| **Tag protection** | v* tags protected on this org |

### How Orgs Consume Shared Resources

```yaml
# Any repo in any iAiFy org can reference shared workflows:
jobs:
  lint:
    uses: Ai-road-4-You/enterprise-ci-cd/.github/workflows/lint.yml@main

  deploy:
    uses: Ai-road-4-You/enterprise-ci-cd/.github/workflows/deploy.yml@main
```

## The iAiFy Enterprise

| Organization | Purpose | Repos |
|-------------|---------|-------|
| **[AiFeatures](https://github.com/AiFeatures)** | AI engineering, agent platforms, LLM tooling | 45 |
| **[HomeAutonom](https://github.com/HomeAutonom)** | Smart home automation, IoT, network infrastructure | 4 |
| **[AiProducting](https://github.com/AiProducting)** | Production apps, infrastructure, financial tools | 18 |
| **[Ai-road-4-You](https://github.com/Ai-road-4-You)** | Shared platform, CI/CD, governance *(this org)* | 5 |

---

<div align="center">
<sub>The road for all 🛣️ Stockholm · <a href="https://github.com/enterprises/iAiFy">iAiFy Enterprise</a></sub>
</div>
