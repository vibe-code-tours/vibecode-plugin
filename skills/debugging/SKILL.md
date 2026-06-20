---
name: Debugging
description: Use when a bug appears, a test fails, or behavior is wrong — reproduce, isolate, fix the root cause not the symptom.
version: 1.0.0
---

# Debugging

Don't guess. Find the root cause.

## Steps
1. **Reproduce** — get a reliable, minimal way to trigger the bug. If you can't reproduce it, you can't fix it.
2. **Read the error** — the actual message + stack trace, not what you assume it says. Quote it exactly.
3. **Isolate** — narrow down: which file, which function, which line. Add logging or use a debugger.
4. **Form one hypothesis** — "I think X because Y". Test it. If wrong, discard and form the next.
5. **Fix the root cause** — not the symptom. A `try/catch` that hides the error is not a fix.
6. **Verify** — the repro now passes, and you didn't break anything nearby.

## Anti-patterns
- Changing random things hoping it works.
- Swallowing errors silently.
- "It works on my machine" — check environment differences.
