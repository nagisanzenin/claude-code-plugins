# nagisanzenin plugins

Claude Code plugin marketplace by nagisanzenin.

## Production Grade Plugin

**One install. 14 AI agents. Idea to production-ready SaaS.**

| Plugin | Version | What's Included |
|--------|---------|-----------------|
| **production-grade** | 3.3.0 | Polymath co-pilot, PM, Architect, Backend, Frontend, QA, Security, Code Review, DevOps, SRE, Data Scientist, Technical Writer, Skill Maker, Orchestrator |

## Install

```bash
/plugin marketplace add nagisanzenin/claude-code-plugins
/plugin install production-grade@nagisanzenin
```

Then say: *"Build a production-grade SaaS for [your idea]"* — or *"Help me think about [your idea]"* if you want the co-pilot first.

## Add to Your Project

Add to `.claude/settings.json` to auto-install for everyone on the project:

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

See [production-grade-plugin](https://github.com/nagisanzenin/claude-code-production-grade-plugin) for full documentation.
