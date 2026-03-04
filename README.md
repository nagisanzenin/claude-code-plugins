# nagisanzenin plugins

Claude Code plugin marketplace by nagisanzenin.

## Available Plugins

| Plugin | Description |
|--------|-------------|
| **product-manager** | AI Product Manager — interviews stakeholders, writes BRDs/PRDs, verifies engineering implementation |

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
