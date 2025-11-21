# Claude Code Configuration

This directory contains custom configurations for Claude Code.

## Overview

Claude Code is an interactive CLI tool by Anthropic that assists with software engineering tasks. This directory can be used to customize project-specific settings, memory, and other configurations.

## Current Configuration

### settings.json
- Custom permissions for allowed/denied commands
- Restricted operations: git commit/push, rm, terragrunt apply/destroy

### Custom Commands
- `/explain-mode` - Enables detailed explanations before executing code changes or commands

## Learn More

- [Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code)
- [Settings Reference](https://docs.anthropic.com/en/docs/claude-code/settings)
- [Slash Commands](https://docs.anthropic.com/en/docs/claude-code/slash-commands)
