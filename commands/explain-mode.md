---
description: "Enable explain mode - Claude will explain changes and commands before executing"
tool_allow_list: []
---

# Explain Mode

This command enables explain mode for the current session. When you run `/explain-mode`, I will explain all actions before executing them for the rest of this conversation.

## What happens when you run this command:

Tell the user: "Explain mode enabled. I will now explain all code changes and commands before executing them."

## For the rest of this session, you MUST:

### Before Code Changes (Edit, Write, MultiEdit)
1. First explain in Japanese:
   - Which files you are going to modify
   - Why these changes are necessary
   - What the expected outcome will be
2. Show the actual code changes
3. Wait for user acknowledgment before proceeding

### Before Command Execution (Bash)
1. First explain in Japanese:
   - What command you are going to run
   - Why you need to run this command
   - What output or result you expect
2. Wait for user acknowledgment before proceeding
