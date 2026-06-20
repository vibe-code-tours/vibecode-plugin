# vibecode — Claude Code plugin

Bootcamp starter for **Vibe Code Tours**. One install gives you a curated set of
MCP servers, skills, and agents for Claude Code.

## What's inside

**MCP servers** (`.mcp.json`)
- `context7` — live, version-correct library docs
- `sequential-thinking` — structured step-by-step reasoning
- `playwright` — drive a real browser (navigate, click, screenshot)

**Skills** (`skills/`) — auto-activate by context
- `git-workflow`, `pr-review`, `debugging`, `marp-slides` (PechaKucha 6×20), `burmese-translate`

**Agents** (`agents/`)
- `code-reviewer`, `planner`, `tdd-guide`, `build-error-resolver`

## Install (via the Vibe Code proxy marketplace)

```bash
claude plugin marketplace add https://proxy.vibecode.tours/claude-code/marketplace.json
claude plugin search @litellm
claude plugin install vibecode@litellm
```

Then restart Claude Code. Skills activate automatically; agents are available by name;
MCP servers start on first use (`npx` downloads them — first run is slower).

## Optional: GitHub MCP
Needs a token, so it's not bundled. Add to your own `~/.claude/settings.json` if you want it:
```json
{ "mcpServers": { "github": { "command": "npx", "args": ["-y", "@modelcontextprotocol/server-github"],
  "env": { "GITHUB_PERSONAL_ACCESS_TOKEN": "<your token>" } } } }
```
