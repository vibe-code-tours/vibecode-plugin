---
name: Ship a Project
description: Use when finishing a small project — write a clear README, make the repo public and runnable, and get it online.
version: 1.0.0
---

# Ship a Project

"Done" means someone else can find it, understand it, and run it.

## 1. README (the front door)
A good README answers, in order:
- **What is it?** One line.
- **Why?** The problem it solves, in plain words.
- **Run it** — exact copy-paste steps (`git clone ...`, install, start). Test them on a clean machine.
- A screenshot or short demo if it has a UI.

## 2. Make it real
- Repo **public** so people (and the checker) can see it.
- Commit often with clear messages. A repo with one giant commit looks fake.
- No secrets in the repo — keys go in `.env` (gitignored), document the names in README.

## 3. Get it online (optional but strong)
- Static site / frontend → **GitHub Pages**, **Vercel**, or **Netlify** (free).
- Small app/API → **Render** or **Railway** (free tiers).
- Put the live link at the top of the README.

## 4. Ask for stars ⭐
Share the link with teammates, ask them to look and star it. A project nobody saw isn't shipped.
