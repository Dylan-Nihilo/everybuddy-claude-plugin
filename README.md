# EveryBuddy — Claude Code Plugin

Your gacha-hatched terminal companion lives in the Claude Code status bar.

## Install

In Claude Code:

```
/plugin marketplace add Dylan-Nihilo/everybuddy-claude-plugin
/plugin install everybuddy
```

Then run the setup:

```
/everybuddy:setup
```

This will:
1. Install the `everybuddy` npm package globally (if needed)
2. Hatch a companion for you (deterministic from your username)
3. Configure Claude Code's status bar

Restart Claude Code and your companion will appear.

## What You Get

- ASCII sprite of your companion in the status bar
- Session info: model, context usage %, git branch, cost
- Frame changes on each assistant message

## Requirements

- Node.js 18+
- npm (for installing the everybuddy CLI)
