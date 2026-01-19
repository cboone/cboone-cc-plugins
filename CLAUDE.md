# Claude Code Plugins

## Project Overview

This repository contains plugins (hooks and skills) for Claude Code.

## Structure

```text
cboone-cc-plugins/
├── .claude-plugin/
│   └── marketplace.json            # Plugin registry for this repository
└── plugins/
    ├── notify/                     # Notification hooks plugin
    │   ├── .claude-plugin/
    │   │   └── plugin.json
    │   ├── hooks/
    │   │   └── hooks.json
    │   └── scripts/
    │           └── notify
    └── writing-shell-scripts/      # Bash style guide skill
        ├── .claude-plugin/
        │   └── plugin.json
        ├── SKILL.md
        └── references/
            └── BASH.md
```

## Development

When adding new plugins:

1. Create the plugin directory under `plugins/`
2. Add a `.claude-plugin/plugin.json` with metadata
3. Register the plugin in `.claude-plugin/marketplace.json`
4. Update README.md with the new plugin description

## License

MIT License - see LICENSE file for details.
