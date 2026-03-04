# nagisanzenin plugins

Claude Code plugin marketplace by nagisanzenin.

## Available Plugins

| Plugin | Description |
|--------|-------------|
| **product-manager** | AI Product Manager — interviews stakeholders, writes BRDs/PRDs, verifies engineering implementation |
| **skill-maker** | Creates new skills and plugins end-to-end: interviews, writes SKILL.md, packages, creates repo, adds to marketplace |
| **solution-architect** | Full architecture pipeline for SaaS: system design, tech stack, API contracts, data models, scaffolding (AWS/GCP/Azure) |
| **devops** | Full DevOps pipeline: Terraform IaC, CI/CD, Docker/K8s, monitoring, security for multi-cloud production deployments |
| **production-grade** | Meta-skill orchestrator: PM → Architect → DevOps pipeline for complete production-ready SaaS |

## Installation

```bash
# Add marketplace
/plugin marketplace add nagisanzenin/nagisanzenin-plugins

# Install a plugin
/plugin install product-manager@nagisanzenin
```

## Adding to your org

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "nagisanzenin": {
      "source": {
        "source": "github",
        "repo": "nagisanzenin/nagisanzenin-plugins"
      }
    }
  },
  "enabledPlugins": {
    "product-manager@nagisanzenin": true
  }
}
```

This auto-installs the plugin for everyone on the project.
