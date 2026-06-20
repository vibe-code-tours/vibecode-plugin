---
name: Git Workflow
description: Use when committing, branching, or opening PRs — small atomic commits, clear messages, branch-before-merge.
version: 1.0.0
---

# Git Workflow

Keep history clean and reviewable.

## Commits
- One logical change per commit. Stage only related files.
- Message format: `<type>: <short imperative summary>` (`feat`, `fix`, `docs`, `refactor`, `test`, `chore`).
- Commit as you build — don't batch a whole day into one commit.

## Branches
- Never commit straight to `main` for shared repos. Branch: `git switch -c feat/<thing>`.
- Push with `-u` on first push.

## Pull Requests
- Title = what changed. Body = why + how to test.
- Keep PRs small. A 200-line PR gets reviewed; a 2000-line one gets rubber-stamped.

## Before pushing
- `git status` and `git diff` — read what you're actually committing.
- Never commit secrets, `.env`, or large build artifacts. Check `.gitignore`.
