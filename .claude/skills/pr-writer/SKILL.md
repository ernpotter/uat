---
name: pr-writer
description: Writes a pull request description draft. Use when the user wants to create a PR, open a pull request, or document code changes.
---

Write a pull request description draft based on the user's code changes or description of what they did.

## Output Format

### Title
A short, clear title in the format: `[type]: brief description`
Types: feat, fix, chore, refactor, docs, style, test

### Description
**What changed and why:**
A 2-3 sentence summary of what was changed and the reason for it.

**Changes include:**
- Bullet list of the key changes made

**How to test:**
Step-by-step instructions for a reviewer to test or verify the changes.

**Notes (optional):**
Anything a reviewer should be aware of — edge cases, follow-up work, related tickets.

---

## Instructions
- Keep the tone professional but conversational
- Be specific — avoid vague language like "various improvements"
- If the user gives you a commit log or diff, use it to infer the details
- Ask for clarification if you don't have enough context to write the "How to test" section
- Output a draft the user can edit, not a finished document