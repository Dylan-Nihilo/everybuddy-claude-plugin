---
name: setup
description: Set up EveryBuddy companion in Claude Code — installs the CLI, hatches a companion, and configures the status bar.
allowedTools:
  - Bash
---

Run these commands in sequence:

1. First check if buddy is installed:
   `which buddy`

2. If NOT found, install it:
   `npm install -g everybuddy`

3. Then run the setup:
   `buddy install claude-code`

Show the full output to the user. After success, tell the user to restart Claude Code to see their companion in the status bar.
