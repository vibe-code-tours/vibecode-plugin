---
name: PR Review
description: Use when reviewing a pull request or your own diff before pushing — checklist for correctness, security, clarity.
version: 1.0.0
---

# PR Review

Review your own diff before asking anyone else to.

## Checklist
- **Correctness** — does it do what the PR says? Any obvious bug or off-by-one?
- **Edge cases** — empty input, null, error path, large input.
- **Security** — no hardcoded secrets, user input validated, no injection.
- **Clarity** — names say what they do, functions small, no dead code.
- **Tests** — new behavior has a test; the test would fail without the change.
- **Scope** — nothing unrelated snuck in.

## How to give feedback
- Be specific: quote the line, say why, suggest the fix.
- Separate "must fix" (bugs, security) from "nice to have" (style).
