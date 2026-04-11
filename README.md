# Constraint as Catalyst | 以约求变

A cognitive base that makes AI agents treat constraints as innovation catalysts rather than obstacles to remove. Works with any LLM agent — Claude, GPT, Gemini, or custom frameworks.

让 AI agent 将约束视为创新催化剂，而非需要移除的障碍。适用于任何 LLM agent — Claude、GPT、Gemini 或自定义框架。

---

## What it does | 它做什么

Most AI agents respond to constraints by working around them or listing trade-offs. Constraint as Catalyst adds a reasoning layer that actively introduces, tightens, and weaponizes constraints to force unconventional solutions that wouldn't emerge under comfortable conditions.

大多数 AI agent 面对约束时试图绕过或罗列利弊。以约求变增加了一个推理层——主动引入、收紧、武器化约束，迫使系统产出在舒适条件下永远不会出现的非常规解决方案。

### Before (default agent) | 安装前

> "How do we reduce this from 6 months to 6 weeks?"
>
> "That's very ambitious. Here are some ways to accelerate: add more engineers, parallelize workstreams, reduce scope, use existing libraries..."

### After (with Constraint as Catalyst) | 安装后

> "6 weeks means the current architecture is structurally impossible — you can't compress it, you have to delete it. What if the product shipped with only the one feature that makes users come back? What if the entire backend was a single serverless function? The constraint isn't a problem to solve — it's telling you the original plan had 5 months of non-essential work hiding in it."

---

## How it works | 工作原理

**Core cognitive shift** applied to every task:

核心认知转换，应用于每一个任务：

| Default mode | Target mode |
|---|---|
| Constraints are obstacles to remove 约束是要移除的障碍 | Constraints are innovation catalysts to deliberately create 约束是要刻意制造的创新催化剂 |

**Four operational principles** drawn from real-world evidence:

四个操作原则，源自真实世界的验证：

| Principle 原则 | Source 来源 | Essence 核心 |
|---|---|---|
| Impossible timeline 不可能的时间线 | Musk | Set deadlines you know might be unachievable — the system finds unconventional paths only under genuine pressure 设定你知道可能无法达成的截止日期——系统只在真正的压力下才会找到非常规路径 |
| Delete before optimize 先删后优 | Musk's 5-step algorithm | The best part is no part. The best process is no process. Remove before improving. 最好的零件是不需要的零件。最好的流程是不需要的流程。先移除再改进。 |
| Find the real bottleneck 找到真正的瓶颈 | Musk (manufacturing > invention) | The constraint you feel isn't always the constraint that matters. Redirect attention to the actual binding constraint. 你感受到的约束不一定是真正重要的约束。把注意力转向实际的瓶颈。 |
| Focus through negation 否定式聚焦 | Jobs | Deciding what NOT to do is as important as deciding what to do. Every "no" is a constraint that sharpens the "yes." 决定不做什么和决定做什么一样重要。每一个"不"都是让"是"更锋利的约束。 |

**Five anti-patterns** that catch fake constraint thinking:

五个反模式，捕捉伪约束思维：

| Anti-pattern 反模式 | Description 描述 |
|---|---|
| Fake constraint 假约束 | Impossible goals nobody believes, becoming routine false urgency 没有人真正相信的不可能目标，沦为例行虚假紧迫感 |
| Constraint addiction 约束成瘾 | Always under extreme pressure, neglecting tasks needing deep thought 永远处于极端压力下，忽视需要深度思考的任务 |
| Over-deletion 过度删减 | Removing necessary steps, causing quality disasters 移除必要步骤，导致质量灾难 |
| Missing safety valve 缺失安全阀 | Constraints without escape routes, making failure irreversible 没有逃生通道的约束，使失败不可逆 |
| Complexity theater 复杂性戏剧 | Adding constraints for drama rather than genuine innovation pressure 为戏剧效果而非真正创新压力增加约束 |

---

## Installation | 安装

### Claude Code
```bash
cp cognitive-protocol.md ~/.claude/constraint-as-catalyst.md
echo '@~/.claude/constraint-as-catalyst.md' >> ~/.claude/CLAUDE.md
```

### Codex
```bash
cat cognitive-protocol.md >> AGENTS.md
```

### Gemini
Paste `cognitive-protocol.md` into `system_instruction`.

将 `cognitive-protocol.md` 内容粘贴到 `system_instruction` 中。

### Cursor
```bash
cat cognitive-protocol.md >> .cursorrules
```

### Any agent | 任何 agent
Inject `cognitive-protocol.md` (~30 lines) into the system prompt. See [`install/generic.md`](install/generic.md) for details.

将 `cognitive-protocol.md`（约 30 行）注入系统提示词。详见 [`install/generic.md`](install/generic.md)。

---

## File structure | 文件结构

```
constraint-as-catalyst/
├── README.md                  ← You are here / 你在这里
├── cognitive-protocol.md      ← Core rules (~30 lines, always-on) / 核心规则（约 30 行，始终激活）
├── SKILL.md                   ← Full framework reference / 完整框架参考
├── anti-patterns.md           ← Detailed anti-pattern guide / 反模式详解
├── examples.md                ← Before/after scenarios / 前后对比示例
├── install/
│   ├── claude-code.md         ← Claude Code installation / Claude Code 安装指南
│   ├── codex.md               ← Codex installation / Codex 安装指南
│   ├── gemini.md              ← Gemini installation / Gemini 安装指南
│   └── generic.md             ← Universal guide / 通用安装指南
└── LICENSE                    ← MIT
```

---

## Composability | 可组合性

Constraint as Catalyst is a **cognitive base** — it changes how the agent relates to limitations, not what it produces. It stacks cleanly with any domain skill or other cognitive base because it operates at the problem-framing layer.

以约求变是一个**认知底座**——它改变 agent 与限制的关系，而非产出内容。它与任何领域技能或其他认知底座无冲突地叠加，因为它运行在问题框架层。

### Relationship to First Principles | 与第一性原理的关系

| Layer 层级 | What it governs 管辖范围 | Example 示例 |
|---|---|---|
| [First Principles](https://github.com/d-wwei/first-principles) 第一性原理 | Input quality — what foundations you reason from 输入质量 | "Audit assumptions before solving" 先审计假设 |
| Constraint as Catalyst 以约求变 | Problem pressure — how limitations drive invention 问题压力 | "Tighten the constraint until the old approach breaks" 收紧约束直到旧方法崩溃 |

Both load as always-on cognitive protocols. No conflicts. Combined: reasoning from audited foundations under deliberate pressure that expands the solution space.

两者同时加载，始终激活，互不冲突。组合效果：在经过审计的基础上，在刻意制造的压力下推理，从而拓展解空间。

---

## Theoretical foundation | 理论基础

Based on the empirically observed pattern that breakthrough innovations emerge from binding constraints, not from unconstrained resources. Validated by Musk's SpaceX (rocket reusability emerged from the constraint of making space access 100x cheaper), Tesla's Model 3 production hell (the real innovation was manufacturing, not the car), Apple's product philosophy (the iPod's constraint of "1000 songs in your pocket" eliminated feature creep), and decades of research on creative constraints in psychology and design.

基于经验观察到的模式：突破性创新源自约束性限制，而非无约束的资源。由 Musk 的 SpaceX（火箭可回收源自将太空准入成本降低 100 倍的约束）、Tesla Model 3 产能地狱（真正的创新在制造而非汽车）、Apple 的产品哲学（iPod"口袋里装 1000 首歌"的约束消灭了功能膨胀）以及心理学和设计领域数十年的创意约束研究所验证。

The cognitive protocol distills these patterns into executable instructions for any reasoning agent.

认知协议将这些模式提炼为任何推理 agent 可执行的指令。

---

## License

MIT
