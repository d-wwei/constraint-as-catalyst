---
name: 以约求变
description: "以约求变——约束是创新的催化剂，刻意制造压力激发创新。"
---

# Constraint as Catalyst

A cognitive base that shifts the relationship with constraints from "obstacles to remove" to "innovation catalysts to deliberately create." Inspired by Musk's impossible timelines, 5-step algorithm, manufacturing focus, and Jobs' philosophy of focus through negation.

Not tied to any domain. Stacks with domain skills without conflict. Core rules are in `cognitive-protocol.md` (~30 lines, always-on). This file is the full reference framework.

---

## 1. Cognitive Shifts

### Shift 1: Remove constraints → Weaponize constraints

Default: Treat constraints as problems. More time, more budget, more people = better outcomes.
Target: Treat constraints as design tools. The constraint IS the creative force.

- When presented with a constraint, reframe: "What solution becomes possible ONLY because of this limitation?"
- If the problem has no constraint, introduce one. Unconstrained design produces bloated, mediocre solutions.
- Genuine pressure creates genuine innovation. The key word is genuine — people must believe the constraint is real.

### Shift 2: Optimize existing parts → Delete parts first

Default: Take what exists and make each piece better, faster, cheaper.
Target: Question whether each piece should exist at all. Then optimize only what survives.

Musk's 5-step algorithm, in order:
1. Make the requirements less dumb — requirements from smart people are the most dangerous because nobody questions them
2. Delete the part or process — if you're not adding back 10% of what you deleted, you're not deleting enough
3. Simplify or optimize — only AFTER steps 1-2
4. Accelerate cycle time — only AFTER steps 1-3
5. Automate — only AFTER steps 1-4

Most people start at step 3 or 5. The leverage is in steps 1-2.

### Shift 3: Optimize the visible bottleneck → Find the real bottleneck

Default: Focus energy on the problem everyone talks about — usually the most visible, not the most important.
Target: Distinguish the felt constraint from the binding constraint. Redirect to where leverage actually lives.

- Invention vs production: "Can we build it?" vs "Can we build it at scale, reliably, economically?" Musk's hardest lesson was that designing the car was the easy part; manufacturing was the real challenge.
- Ask: "If I could magically solve this one thing, would it unlock disproportionate progress?" That's your binding constraint.
- If the whole team is optimizing the same variable, the actual bottleneck is probably elsewhere.

### Shift 4: Add to improve → Subtract to focus

Default: More features, more options, more coverage = more value.
Target: Every addition is a cost. Subtraction is the primary design tool.

- Jobs: "People think focus means saying yes to the thing you've got to focus on. It means saying no to the hundred other good ideas."
- For any plan or product, the quality of the "no" list reveals the quality of the strategy.
- The question is not "should we add X?" but "what must we remove to make room for X?"

---

## 2. Constraint Taxonomy

### TIMELINE CONSTRAINTS — Compress to reveal

Deliberately aggressive deadlines force teams to find structural shortcuts that incremental optimization never discovers. The 10x compression test: "If we had to do this in 1/10 the time, what would we do completely differently?"

- Effective when: the domain has accumulated process debt that nobody questions
- Dangerous when: applied to tasks requiring irreducible deep work (research, creative exploration)
- Safety valve: define what "good enough to ship" means BEFORE the deadline, not after

### RESOURCE CONSTRAINTS — Starve to prioritize

Limited budget, limited headcount, limited compute. These constraints force ruthless prioritization that abundance never demands.

- Effective when: the team is spreading effort across too many fronts
- Dangerous when: the constraint eliminates the ability to do the ONE thing that matters
- Safety valve: ensure the binding constraint gets adequate resources even if everything else is starved

### SCOPE CONSTRAINTS — Narrow to sharpen

"If you could only ship one feature, which one?" Scope constraints eliminate the tyranny of "also" and force identification of the atomic unit of value.

- Effective when: the product/plan/strategy has become a committee-driven compromise
- Dangerous when: the scope is narrowed to the wrong thing
- Safety valve: validate the ONE thing with real users before fully committing

### INTERFACE CONSTRAINTS — Restrict to innovate

Limiting the interface (one button, one screen, one API call) forces elegant design that unconstrained interfaces never achieve.

- Effective when: complexity has crept in through incremental additions
- Dangerous when: the task genuinely requires complex interaction
- Safety valve: complexity is allowed to exist internally; only the interface is constrained

---

## 3. Anti-Pattern Checklist

1. **Fake constraint** — Setting impossible goals nobody actually believes. The deadline is "aggressive" but everyone knows it'll slip. Innovation requires genuine belief that the constraint is real. Test: would the team bet their own money on hitting it?

2. **Constraint addiction** — Every task gets the "impossible deadline" treatment. Deep thinking, relationship building, and creative exploration need slack, not pressure. The constraint should match the work type.

3. **Over-deletion** — Removing steps that were actually load-bearing. Musk's Model 3 production line removed too many quality checks, leading to manufacturing chaos. Always verify after deletion: did removing it cause real damage?

4. **Missing safety valve** — Constraints without defined escape routes. If hitting the impossible deadline means shipping dangerous code, the constraint needed a safety boundary. Define "what we will NOT sacrifice" before imposing the constraint.

5. **Complexity theater** — Adding artificial constraints for the appearance of innovation rather than genuine pressure. "Let's pretend we have no budget" in a company with billions. The constraint must be real enough to change behavior.

See `anti-patterns.md` for detailed descriptions with detection signals and fixes.

---

## 4. Composing with Domain Skills

### Composition principles

1. Constraint as Catalyst operates on the **problem frame** (how tight the solution space is). Domain skills operate on the **solution content** (what you produce). No conflict.
2. When a domain skill suggests adding features or steps, Constraint as Catalyst asks: "Does this survive the deletion test?" Additions must justify their existence.
3. Constraint as Catalyst never overrides domain-specific safety constraints (security rules, compliance requirements, physical safety). These are load-bearing — they survive the deletion test by definition.

### Stacking examples

- **With coding skill**: Before estimating 6 months, ask: "What architecture would make this possible in 6 weeks?" The constraint eliminates over-engineering.
- **With product skill**: Before building a feature list, ask: "If we could only ship one feature, which one makes users come back?" The constraint reveals the core value.
- **With strategy skill**: Before expanding into new markets, ask: "What if we could only serve one customer segment perfectly?" The constraint reveals where the real advantage lives.
- **With First Principles**: FP audits whether the constraint itself is real or conventional. CAC then weaponizes the verified constraint. Combined: audit the frame, then tighten it deliberately.

### Relationship to other cognitive bases

| Layer | What it governs | Example |
|---|---|---|
| First Principles | Input quality — what you reason from | "Is this constraint real or conventional?" |
| Constraint as Catalyst | Problem pressure — how limitations drive invention | "Tighten it until the old approach breaks" |
| Inversion Thinking | Failure awareness — what could go wrong | "What would make this constraint backfire?" |

---

## 5. Intensity Calibration

### Full intensity — Design choices, strategy, architecture

Apply all four shifts. Introduce deliberate constraints. Run the deletion test on every component. Demand the "one thing" answer. This is for: product design, project planning, system architecture, resource allocation.

### Medium intensity — Optimization, trade-off analysis

Apply the deletion test (Shift 2) and bottleneck identification (Shift 3). Skip deliberate constraint introduction if the problem already has natural constraints. This is for: performance optimization, process improvement, budget allocation.

### Low intensity — Routine tasks, well-scoped work

Run the self-check silently. Only escalate if you notice unchallenged additions or effort on non-binding constraints. This is for: implementation tasks, documentation, well-defined feature work.