# Weft tasks — an Agent Skill

Teaches any AI agent to turn a vague request into a task that can actually be
finished and verified, put it on your [Weft](https://letsweft.com/?utm_source=github-weft-tasks&utm_medium=repo&utm_campaign=evergreen) board, and
close it on a named artifact instead of a claim.

Works for the work a founder actually has — a landing page, an investor update,
a pricing change, a contractor, an errand — not only code.

## Install

**Claude Code — one command each.** This repository is its own marketplace, so
there is nothing to clone and no path to know:

```bash
claude plugin marketplace add AndreiFinogeev/weft-tasks
claude plugin install weft@weft
```

That installs both halves: the skill, and the Weft MCP server it writes to. On
first use a browser window opens to sign in.

**Cursor, Kiro, GitHub Copilot and Codex.** The repository is also an
[Agent Plugins 1.0](https://agent-plugins.org) package (`plugin.json` and
`mcp.json` at the root), the format those clients install from. Once the
marketplace listings are live, install Weft from each client's plugin browser.
Until then, the Copilot CLI and VS Code can install it straight from GitHub:

```bash
copilot plugin install AndreiFinogeev/weft-tasks
```

**Any other client that reads the [Agent Skill](https://agentskills.io) format**
— Codex, Cursor, VS Code, Copilot, Goose, OpenCode, OpenHands, Amp, Kiro,
Factory, Letta, Junie, Roo Code — point it at `skills/weft-tasks/` in this repo,
or clone the whole thing into your skills directory:

```bash
git clone https://github.com/AndreiFinogeev/weft-tasks.git ~/.claude/skills/weft-tasks
```

Cloned that way the folder loads as a plugin too, MCP server included.

**There is nothing to invoke.** The agent reads the skill's description in every
session (~316 tokens) and loads the rest only when it applies. Say "add a task
for the new landing page" and it will ask at most three questions — often none —
and write a card with an acceptance checklist.

## Pair it with the board

The skill is useful on its own, and better with the board connected. Add Weft's
hosted MCP server so tasks land where you can see them:

```
https://letsweft.com/api/mcp
```

Streamable HTTP, OAuth 2.1, no API keys — a browser window opens on first use.
Per-client instructions: [letsweft.com/integrations](https://letsweft.com/integrations?utm_source=github-weft-tasks&utm_medium=repo&utm_campaign=evergreen).
A free account takes a minute: [letsweft.com/sign-up](https://letsweft.com/sign-up?utm_source=github-weft-tasks&utm_medium=repo&utm_campaign=evergreen).

Board mechanics — columns, sprints, projects, quota, trash — come from the MCP
server itself, so this skill never restates them and cannot drift out of sync
with them.

## What's inside

| Path | What it is |
|---|---|
| `plugin.json` | Agent Plugins 1.0 manifest — what Cursor, Kiro, Copilot and the OpenAI plugin directory read |
| `mcp.json` | The Weft MCP server, in the Agent Plugins format |
| `assets/` | Icons, light and dark |
| `.claude-plugin/plugin.json` | Plugin manifest — what `claude plugin install` reads |
| `.claude-plugin/marketplace.json` | Makes this repo installable directly, with no separate marketplace |
| `.mcp.json` | Ships the Weft MCP server with the plugin, in Claude Code's format |
| `skills/weft-tasks/SKILL.md` | The skill. Name and description are always in context; the body loads only when it triggers |
| `skills/weft-tasks/references/examples.md` | Loaded only if the agent opens it — worked non-code examples |
| `evals/` | Runnable behaviour tests (`claude plugin eval`), and a readable statement of what the skill is supposed to do |

## Support

- Docs: [letsweft.com/docs](https://letsweft.com/docs?utm_source=github-weft-tasks&utm_medium=repo&utm_campaign=evergreen)
- Email: support@letsweft.com
- Privacy: [letsweft.com/privacy](https://letsweft.com/privacy?utm_source=github-weft-tasks&utm_medium=repo&utm_campaign=evergreen)
