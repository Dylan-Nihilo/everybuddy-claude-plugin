<p align="center">
  <strong>EveryBuddy — Claude Code Plugin</strong>
</p>

<p align="center">
  Your gacha-hatched terminal companion lives in the Claude Code status bar.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Claude_Code-Plugin-7C3AED?logo=anthropic&logoColor=white" alt="Claude Code Plugin" />
  <img src="https://img.shields.io/badge/npm-everybuddy-CB3837?logo=npm&logoColor=white" alt="npm" />
  <img src="https://img.shields.io/badge/Node.js-≥18-339933?logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/License-MIT-blue" alt="License" />
</p>

<p align="center">
  <a href="#install">Install</a> ·
  <a href="#what-you-get">What You Get</a> ·
  <a href="#uninstall">Uninstall</a> ·
  <a href="#related">Related</a>
</p>

---

EveryBuddy draws a unique companion from a deterministic gacha system, gives it an AI-written personality, and renders its ASCII sprite in the Claude Code status bar alongside session info.

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

| Feature | Description |
|---------|-------------|
| ASCII sprite | Your unique companion rendered in the status bar |
| Session info | Model name, context window %, git branch, cost |
| Frame animation | Sprite frame changes on each assistant message |
| Auto-hatch | Deterministic draw from your username — no setup choices needed |

## Uninstall

Remove the `statusLine` entry from `~/.claude/settings.json`, then:

```
/plugin uninstall everybuddy
```

## Requirements

- **Node.js** >= 18
- **npm** (used by `/everybuddy:setup` to install the CLI)

## Related

- [EveryBuddy CLI](https://github.com/Dylan-Nihilo/EveryBuddy) — Core package (`npm: everybuddy`). Also supports tmux sidecar follow mode with AI-driven speech bubble reactions.
- [everybuddy.cn](https://everybuddy.cn) — Showcase and species gallery.

## License

MIT
