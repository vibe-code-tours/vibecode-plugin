---
name: Marp Slides (PechaKucha 6x20)
description: Use when building a short project pitch deck — Marp markdown, exactly 6 slides, 20 seconds each, auto-advance.
version: 1.0.0
---

# Marp Slides — PechaKucha 6×20

A tight 2-minute pitch: **6 slides, 20 seconds each**.

## Frontmatter (required)
```markdown
---
marp: true
auto-advance: 20
---
```

## Rules
- Exactly **6 slides**. Separate each with `---` on its own line, with a **blank line before it**.
- One idea per slide. Few words, one visual. The slide supports you talking — it's not the script.
- Suggested arc: 1) Problem 2) Who it's for 3) What you built 4) How (AI/tools used) 5) Demo/result 6) What's next.

## Example
```markdown
---
marp: true
auto-advance: 20
---

# My Project
The one-line pitch.

---

# The Problem
Who hurts, and how much.

---

# ...four more slides...
```

Keep the file in your repo (e.g. `slides/pitch.md`) and reference it by repo-relative path.
