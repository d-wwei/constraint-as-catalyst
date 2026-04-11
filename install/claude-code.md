# Install — Claude Code

## Quick install

```bash
# 1. Copy cognitive protocol to Claude's config
cp cognitive-protocol.md ~/.claude/constraint-as-catalyst.md

# 2. Add reference in CLAUDE.md
echo '@~/.claude/constraint-as-catalyst.md' >> ~/.claude/CLAUDE.md
```

## What gets loaded where

| File | Destination | Purpose |
|---|---|---|
| `cognitive-protocol.md` | `~/.claude/constraint-as-catalyst.md` | Always-on core rules (~30 lines) |
| `SKILL.md` | `~/.claude/skills/constraint-as-catalyst/SKILL.md` | Full reference (loaded on demand) |
| `anti-patterns.md` | `~/.claude/skills/constraint-as-catalyst/anti-patterns.md` | Detailed anti-pattern guide |
| `examples.md` | `~/.claude/skills/constraint-as-catalyst/examples.md` | Before/after reference |

## Full install (with skill files)

```bash
# 1. Core rules
cp cognitive-protocol.md ~/.claude/constraint-as-catalyst.md

# 2. Skill files
mkdir -p ~/.claude/skills/constraint-as-catalyst
cp SKILL.md ~/.claude/skills/constraint-as-catalyst/
cp anti-patterns.md ~/.claude/skills/constraint-as-catalyst/
cp examples.md ~/.claude/skills/constraint-as-catalyst/

# 3. Register in CLAUDE.md
echo '@~/.claude/constraint-as-catalyst.md' >> ~/.claude/CLAUDE.md
```

## Verify

Ask Claude Code: "What are the constraint-as-catalyst cognitive rules you're following?" It should list the four sections from `cognitive-protocol.md`: weaponize constraints, delete before optimize, find the real bottleneck, focus through negation, plus the output self-check.

## Stacking with other cognitive bases

If First Principles (`~/.claude/first-principles.md`) is already loaded, no changes needed. Both protocols load independently. First Principles audits whether the constraint is real or conventional; Constraint as Catalyst then weaponizes the verified constraint. No conflicts.

## Uninstall

```bash
rm ~/.claude/constraint-as-catalyst.md
rm -rf ~/.claude/skills/constraint-as-catalyst
# Remove the @~/.claude/constraint-as-catalyst.md line from ~/.claude/CLAUDE.md
```
