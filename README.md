# vibecode — Claude Code plugin

Bootcamp starter for **Vibe Code Tours**. One install gives you a curated set of
MCP servers, skills, and agents for Claude Code.

## What's inside

**MCP servers** (`.mcp.json`) — kept lean on purpose (each is a process spawned per session)
- `context7` — live, version-correct library docs
- `sequential-thinking` — structured step-by-step reasoning
- `playwright` — drive a real browser (navigate, click, screenshot)
- `memory` — a simple knowledge graph that persists across the session

**Skills** (`skills/`) — auto-activate by context
- `ui-ux-pro-max` — design intelligence: 67 styles, 96 palettes, 57 font pairings, 99 UX rules (CLI-searchable)
- `frontend-design` — distinctive, accessible web UI that avoids the AI-template look
- `api-design` — REST naming, status codes, error envelopes, pagination
- `git-workflow` — small atomic commits, branch-before-merge, clean PRs
- `pr-review` — review your own diff before pushing
- `debugging` — reproduce, isolate, fix the root cause
- `marp-slides` — PechaKucha 6x20 pitch decks
- `ship-project` — write a README, make it runnable, get it online
- `burmese-translate` — bilingual EN + မြန်မာ content

**Agents** (`agents/`) — helpers for building **your own** project
- `code-explainer` — explains code & error messages in plain language
- `code-reviewer`, `security-reviewer` — catch bugs & risks before you commit
- `frontend-designer` — build accessible, good-looking web UI
- `planner`, `tdd-guide`, `build-error-resolver`, `pitch-coach`

## Install (via the Vibe Code proxy marketplace)

```bash
claude plugin marketplace add https://proxy.vibecode.tours/claude-code/marketplace.json
claude plugin search @litellm
claude plugin install vibecode@litellm
```

Then restart Claude Code. Skills activate automatically; agents are available by name;
MCP servers start on first use (npx downloads them — first run is slower).

`ui-ux-pro-max` uses a small Python CLI — needs `python3` on your machine.

## Optional: GitHub MCP
Needs a token, so it's not bundled. Add to your own `~/.claude/settings.json` if you want it:
```json
{ "mcpServers": { "github": { "command": "npx", "args": ["-y", "@modelcontextprotocol/server-github"],
  "env": { "GITHUB_PERSONAL_ACCESS_TOKEN": "<your token>" } } } }
```
