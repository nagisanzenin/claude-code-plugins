# nagisanzenin plugins

Claude Code plugin marketplace by nagisanzenin -- 13 production-grade AI workflow skills.

## Available Plugins

| Plugin | Version | Description |
|--------|---------|-------------|
| **production-grade** | 2.0.0 | Fully autonomous SaaS pipeline: 13 bundled skills, one install, complete pipeline |
| **product-manager** | 1.0.0 | AI Product Manager -- stakeholder interviews, BRDs/PRDs, implementation verification |
| **solution-architect** | 1.0.0 | Full architecture pipeline: system design, tech stack, API contracts, scaffolding (AWS/GCP/Azure) |
| **software-engineer** | 1.0.0 | Production-grade services: clean architecture, payment integration, autonomous debugging |
| **frontend-engineer** | 1.0.0 | Complete frontend pipeline: design system, components, pages, accessibility (Next.js/Vue/Svelte) |
| **qa-engineer** | 1.0.0 | Comprehensive testing: unit, integration, contract, e2e, performance, self-healing protocols |
| **security-engineer** | 1.0.0 | Application security: STRIDE threat modeling, OWASP audit, pen test, compliance |
| **code-reviewer** | 1.0.0 | Architecture conformance, code quality, security, performance review, auto-fix |
| **devops** | 1.0.0 | Full DevOps: Terraform IaC, CI/CD, Docker/K8s, monitoring, security scanning |
| **sre** | 1.0.0 | Site reliability: production readiness, chaos engineering, capacity planning, incident management |
| **data-scientist** | 1.0.0 | AI/ML/LLM optimization: prompt engineering, token optimization, A/B testing |
| **technical-writer** | 1.0.0 | Complete docs: API reference, dev guides, operational docs, Docusaurus scaffold |
| **skill-maker** | 1.0.0 | Creates new skills/plugins end-to-end: interviews, writes SKILL.md, packages, publishes |

## Quick Start

### Option A: Install Everything (Recommended)

```bash
/plugin marketplace add nagisanzenin/claude-code-plugins
/plugin install production-grade@nagisanzenin
```

This single install gives you all 13 skills bundled together.

### Option B: Install Individual Skills

```bash
/plugin marketplace add nagisanzenin/claude-code-plugins
/plugin install software-engineer@nagisanzenin
/plugin install qa-engineer@nagisanzenin
# ... etc
```

## Adding to Your Org

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "nagisanzenin": {
      "source": {
        "source": "github",
        "repo": "nagisanzenin/claude-code-plugins"
      }
    }
  },
  "enabledPlugins": {
    "production-grade@nagisanzenin": true
  }
}
```

This auto-installs the plugin for everyone on the project.
