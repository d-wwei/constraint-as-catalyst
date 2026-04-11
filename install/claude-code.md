# Install — Claude Code

## Quick install

```bash
# 1. Inject core rules into CLAUDE.md (direct content injection — works on all versions)
cat cognitive-protocol.md >> ~/.claude/CLAUDE.md
```

## What gets loaded where

| File | Destination | Purpose |
|---|---|---|
| `cognitive-protocol.md` | `~/.claude/CLAUDE.md` (appended) | Always-on core rules (~30 lines) |
| `SKILL.md` | `~/.claude/skills/constraint-as-catalyst/SKILL.md` | Full reference (loaded on demand) |
| `anti-patterns.md` | `~/.claude/skills/constraint-as-catalyst/anti-patterns.md` | Detailed anti-pattern guide |
| `examples.md` | `~/.claude/skills/constraint-as-catalyst/examples.md` | Before/after reference |

## Full install (with skill files)

```bash
# 1. Core rules (inject directly into CLAUDE.md)
cat cognitive-protocol.md >> ~/.claude/CLAUDE.md

# 2. Skill files
mkdir -p ~/.claude/skills/constraint-as-catalyst
cp SKILL.md ~/.claude/skills/constraint-as-catalyst/
cp anti-patterns.md ~/.claude/skills/constraint-as-catalyst/
cp examples.md ~/.claude/skills/constraint-as-catalyst/

# 3. (Core rules already injected in step 1)
```

## Verify

Ask Claude Code: "What are the constraint-as-catalyst cognitive rules you're following?" It should list the four sections from `cognitive-protocol.md`: weaponize constraints, delete before optimize, find the real bottleneck, focus through negation, plus the output self-check.

## Stacking with other cognitive bases

If First Principles (`~/.claude/first-principles.md`) is already loaded, no changes needed. Both protocols load independently. First Principles audits whether the constraint is real or conventional; Constraint as Catalyst then weaponizes the verified constraint. No conflicts.

## Uninstall

```bash
# Remove the Constraint as Catalyst section from ~/.claude/CLAUDE.md (search for "# Constraint as Catalyst — Cognitive Protocol" header)
rm -rf ~/.claude/skills/constraint-as-catalyst
```
