# Install — Generic (Any Agent/Framework)

> **Recommended**: Run `./install.sh` from the repo root for automated installation. Supports Claude Code, Gemini CLI, Codex CLI, Cursor, OpenCode, and OpenClaw.
> The manual steps below are for reference or troubleshooting.

## Universal principle

Constraint as Catalyst is a cognitive base — it changes how the agent relates to limitations, not what tools it uses. Installation means injecting `cognitive-protocol.md` into the agent's always-on instructions (system prompt, rules file, or configuration).

## Platform mapping

| Platform | Where to inject | File to use |
|---|---|---|
| Claude Code | `~/.claude/constraint-as-catalyst.md` + ref in `CLAUDE.md` | `cognitive-protocol.md` |
| Codex | Prepend to `AGENTS.md` | `cognitive-protocol.md` |
| Gemini | `system_instruction` field | `cognitive-protocol.md` |
| Cursor | Prepend to `.cursorrules` | `cognitive-protocol.md` |
| ChatGPT | Custom Instructions -> system prompt | `cognitive-protocol.md` |
| LangChain | System message in chain | `cognitive-protocol.md` |
| AutoGPT / CrewAI | Agent system prompt | `cognitive-protocol.md` |
| Any other | Find the "always-on instructions" config and inject there | `cognitive-protocol.md` |

## Step by step

1. Locate your agent's system prompt or always-on rules file
2. Copy the contents of `cognitive-protocol.md` (~30 lines)
3. Paste it into the system prompt, BEFORE any domain-specific instructions
4. If using First Principles, place it first, then Constraint as Catalyst

## File selection guide

| Need | File | Size |
|---|---|---|
| Minimal install (core rules only) | `cognitive-protocol.md` | ~30 lines |
| Full reference framework | + `SKILL.md` | ~200 lines |
| Anti-pattern detection | + `anti-patterns.md` | ~120 lines |
| Teaching examples | + `examples.md` | ~120 lines |

For most agents, `cognitive-protocol.md` alone is sufficient. The additional files are reference material for when the agent needs deeper guidance.

## Troubleshooting

- **Agent ignores the rules**: Move `cognitive-protocol.md` content to the beginning of the system prompt, not the end. Most models weight earlier instructions more heavily.
- **Agent over-applies constraints**: Check intensity calibration in `SKILL.md`. Routine tasks should get low intensity (silent self-check only). Not every task needs impossible deadlines.
- **Agent deletes too aggressively**: Ensure the anti-pattern for over-deletion is loaded. The deletion test requires empirical verification, not just logical justification.
- **Context window pressure**: `cognitive-protocol.md` is ~30 lines. If that's too much, something else in your prompt needs trimming first.
