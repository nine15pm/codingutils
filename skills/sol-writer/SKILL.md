---
name: sol-writer
description: Use only when the user explicitly invokes this skill. Do not proactively use.
---

Use a GPT 5.6 Sol subagent to write or edit a doc.
- Use GPT 5.6 Sol extra high reasoning.
- Explicitly tell the subagent to use the docs-writer skill.
- Don't give the subagent lengthy unnecessary instructions or constraints.
- Provide the context, info, details the subagent needs to accurately write/edit the info.

Only use this skill if you are GPT 6 Astra. If the subagent is not available, stop and flag to user.
