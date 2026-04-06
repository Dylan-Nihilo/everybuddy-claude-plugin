# EveryBuddy — Claude Code Plugin

> Your gacha-hatched terminal companion lives in the Claude Code status bar.

EveryBuddy draws a unique companion from a deterministic gacha system, gives it an AI-written personality, and renders its ASCII sprite in the Claude Code status bar alongside session info (model, context %, git branch, cost).

This plugin provides the Claude Code integration. The core CLI is at [Dylan-Nihilo/EveryBuddy](https://github.com/Dylan-Nihilo/EveryBuddy).

## Install

In Claude Code:

```
/plugin marketplace add Dylan-Nihilo/everybuddy-claude-plugin
/plugin install everybuddy
```

Then run setup (one time only):

```
/everybuddy:setup
```

This will:
1. Install the `everybuddy` npm package globally (if not already installed)
2. Hatch a companion using your system username as the deterministic seed
3. Write the `statusLine` config to `~/.claude/settings.json`

Restart Claude Code — your companion will appear in the status bar.

## What You Get

```
   .----.        Branch Bath · capybara
  ( .  . )       [Opus] 42% | main | $0.23
  (______)   
  /\/\/\/\   
```

- **ASCII sprite** of your unique companion rendered in the status bar
- **Session info**: model name, context window usage %, git branch, accumulated cost
- **Frame animation**: sprite frame changes on each assistant message turn

## Uninstall

Remove the `statusLine` entry from `~/.claude/settings.json`, then:

```
/plugin uninstall everybuddy
```

## Requirements

- Node.js 18+
- npm (used by `/everybuddy:setup` to install the CLI)

## Related

- [EveryBuddy CLI](https://github.com/Dylan-Nihilo/EveryBuddy) — the core package (npm: `everybuddy`). Also supports tmux sidecar follow mode with AI-driven speech bubble reactions.
- [everybuddy.cn](https://everybuddy.cn) — Showcase and species gallery.
