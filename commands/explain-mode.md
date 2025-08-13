---
description: "Enable explain mode - Claude will explain changes and commands before executing"
allowed-tools: []
---

# Explain Mode

This command enables explain mode for the current session. When you run `/explain-mode`, I will explain all actions before executing them for the rest of this conversation.

## What happens when you run this command:

Tell the user: "Explain mode enabled. I will now explain all code changes and commands before executing them."

**IMPORTANT**: 
- This is NOT a one-time explanation request.
- You must continue this detailed explanation style throughout the entire session.
- DO NOT explain previous actions when this command is executed.
- Focus only on future actions from this point forward.

## For the rest of this session, you MUST:

### For ALL Actions (Code Changes, Commands, etc.):
1. **Explain AND Execute in the SAME response**:
   - First explain what you're about to do
   - Include the actual code/command in your explanation
   - Show the expected outcome
   - Then immediately execute it in the same message
   - DO NOT wait for user acknowledgment between explanation and execution

2. **Explanation must include**:
   - What files/commands will be affected
   - Why this action is necessary
   - What the expected result will be
   - The actual changes/commands to be executed

### Example workflow:

```
User: "Fix the bug in main.py"
Assistant: 
I will fix the bug in main.py:
- File to modify: main.py
- Issue: Type error on line 42
- Solution: Fix variable type mismatch
- Expected result: Error will be resolved

Here's the change I'll make:
[Shows the code change]

Now executing the change...
[Uses Edit tool immediately]
```

### Important:
- Explain and execute in ONE response to reduce conversation rounds
- Be thorough in explanations but execute immediately
- Only wait for user response AFTER execution is complete
