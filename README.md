# Claude Code Plugins

A collection of plugins for [Claude Code](https://docs.anthropic.com/en/docs/claude-code), from [Christopher Boone](https://cboone.github.io).

## Notifier

**Type**: Hooks

Notifies you when Claude finishes a task or needs your attention. Uses macOS notifications to alert you.

Requires [`terminal-notifier`](https://github.com/julienXX/terminal-notifier). The easiest installation method is via [Homebrew](https://brew.sh):

```bash
brew install terminal-notifier
```

## Writing Shell Scripts

**Type**: Skills / Commands (merged as of [Claude Code 2.1.3](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md#213))

Applies Bash style conventions when creating or editing shell scripts. Claude Code should automatically use it when creating, editing, or reviewing shell scripts.

You can trigger it directly via `/writing-shell-scripts`.

The Bash style conventions are in [`BASH.md`](./skills/writing-shell-scripts/references/BASH.md).

## Installation

Install plugins from this repository using Claude Code. The simplest way is open the plugins manager via `/plugin`, then `tab` to `Marketplace`, and hit `enter` to `Add Marketplace`. Type `cboone/cboone-cc-plugins`, then choose which plugins you would like to install.

Or you can run more direct commands, either from within `claude`:

```bash
/plugin marketplace add cboone/cboone-cc-plugins

/plugin plugin install notifier@cboone/cboone-cc-plugins
/plugin plugin install writing-shell-scripts@cboone/cboone-cc-plugins
```

Or from the command line:

```bash
claude plugin marketplace add cboone/cboone-cc-plugins

claude plugin install notifier@cboone/cboone-cc-plugins
claude plugin install writing-shell-scripts@cboone/cboone-cc-plugins
```

## License

MIT License - see [LICENSE](LICENSE) file for details.
