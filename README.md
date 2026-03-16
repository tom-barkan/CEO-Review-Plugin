# CEO Review Plugin

**Your AI-powered strategic advisor. Stop building. Start validating.**

[Install](#installation) · [How It Works](#how-it-works) · [Examples](#examples) · [Components](#components) · [Contributing](#contributing)

---

## What is this?

CEO Review is an open-source [Claude Code](https://docs.anthropic.com/en/docs/claude-code) plugin that turns Claude into a tough, experienced CEO advisor who stress-tests your feature ideas before you write a single line of code.

Run `/ceo-review` and the plugin will:

1. **Interrogate** your idea through Socratic questioning — one tough question at a time
2. **Dispatch 6 specialist analysts** in parallel to evaluate strategy, market, moat, distribution, unit economics, and risk
3. **Cross-check findings** across analysts and re-run any that need updating based on new context
4. **Deliver a scorecard** with a clear BUILD / DEFER / KILL verdict

The goal is simple: **catch bad ideas before they cost you weeks of engineering time.**

## Why?

Every team has shipped a feature that should have been killed in the planning phase. The post-mortem always reveals the same thing: nobody asked the hard questions early enough.

CEO Review forces those hard questions upfront. It applies real strategy frameworks — Hamilton Helmer's 7 Powers, Porter's Five Forces, TAM/SAM/SOM, Blue Ocean, JTBD — and demands specific metrics, not hand-waving. The tone is assertive and critical, but fundamentally wants you to succeed. Think of it as a co-founder who has been through this before and won't let you waste time on the wrong thing.

## Installation

**One-command install:**

```bash
claude install-plugin https://github.com/tom-barkan/CEO-Advisor-Plugin
```

**Manual install:**

```bash
# Clone the repo
git clone https://github.com/tom-barkan/CEO-Advisor-Plugin.git

# Run Claude with the plugin
claude --plugin-dir /path/to/CEO-Advisor-Plugin
```

## How It Works

### Phase 1: Input

Provide a feature description as text or point to a spec file:

```bash
/ceo-review "Add AI-powered search to our documentation platform"
/ceo-review ./specs/ai-search-feature.md
```

### Phase 2: Socratic Questioning

The CEO advisor asks 8-12 tough questions, one at a time. It adapts follow-up questions based on your answers and pushes back on vague responses.

| Category | Example Question |
|---|---|
| **Value** | "How are users solving this problem TODAY without your feature?" |
| **Strategy** | "What are you saying NO to by saying yes to this?" |
| **Financial** | "How will you price this? Which metric does it move, and by how much?" |
| **Distribution** | "How does a user DISCOVER this feature?" |
| **Risk** | "Assume it launched and failed — why did it fail?" |
| **Success** | "What's the kill criteria — at what point do you pull the plug?" |

If you give a vague answer, it pushes back once. If still vague, it flags it as a risk.

### Phase 3: Parallel Analysis

Six specialist agents run simultaneously, each evaluating a different dimension:

| Analyst | Focus | Key Output |
|---|---|---|
| **Strategy Analyst** | 7 Powers, Porter's, Blue Ocean, Wardley | Strategic Alignment (1-10) |
| **Market Scanner** | Competition research, alternatives, saturation | Market Opportunity (1-10) |
| **Moat Evaluator** | Network effects, switching costs, defensibility | Defensibility (1-10) |
| **Distribution Analyst** | GTM channels, CAC, virality, adoption friction | Distribution Feasibility (1-10) |
| **Unit Economics Analyst** | TAM/SAM/SOM, pricing, LTV/CAC, metrics | Financial Value (1-10) |
| **Pre-Mortem Analyst** | Failure modes, risks, biggest assumptions | Risk Profile (1-10) |

The **Market Scanner** uses web search to find real competitors — it names names, not hypotheticals.

### Phase 4: Scorecard & Verdict

An orchestrator reviews all analyst findings, checks for contradictions, re-runs agents if new context warrants it, and produces the final scorecard:

```
SCORECARD
─────────────────────────────────
Strategic Alignment:       7/10  — Strong 7 Powers fit (network effects)
Market Opportunity:        5/10  — Crowded space, 4 funded competitors
Defensibility / Moat:      6/10  — Data moat possible but unproven
Distribution Feasibility:  8/10  — Strong PLG channel via existing users
Unit Economics:            4/10  — No pricing model defined
Risk Profile:              5/10  — High dependency on third-party API

VERDICT: DEFER
─────────────────────────────────
Strong distribution story but weak financial case.
Define pricing model and validate willingness-to-pay
before committing engineering resources.

Conditions for re-evaluation:
- Pricing survey with n=50+ target users
- Competitive differentiation beyond "we have it built in"
- Fallback plan for API dependency
```

## Examples

```bash
# Review a feature idea from scratch
/ceo-review "Build a real-time collaboration feature for our design tool"

# Review from a spec file
/ceo-review ./specs/collaboration-feature.md

# Quick review with no arguments (will ask you to describe it)
/ceo-review
```

## Components

### Command

| Command | Description |
|---|---|
| `/ceo-review` | Run a full CEO-level strategic review of a feature |

### Agents

| Agent | Role | Color |
|---|---|---|
| `review-orchestrator` | Coordinates all analysts, synthesizes scorecard | Cyan |
| `strategy-analyst` | Strategic frameworks analysis (7 Powers, Porter's) | Blue |
| `market-scanner` | Competition research with web search | Cyan |
| `moat-evaluator` | Defensibility and competitive moat assessment | Green |
| `distribution-analyst` | Go-to-market and distribution feasibility | Yellow |
| `unit-economics-analyst` | Financial viability, TAM/SAM/SOM, pricing | Magenta |
| `pre-mortem-analyst` | Failure prediction and risk mitigation | Red |

### Skills

| Skill | Purpose |
|---|---|
| `strategic-frameworks` | Reference knowledge for 7 Powers, Porter's, Blue Ocean, JTBD, Wardley Mapping, TAM/SAM/SOM, RICE/ICE, Kano Model |
| `ceo-mindset` | CEO persona definition, evaluation criteria, scorecard template, Socratic questioning patterns |

## Requirements

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) CLI installed
- Internet access (for market research via web search)

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b my-feature`)
3. Commit your changes
4. Open a pull request

**Ideas for improvement:**

- Add industry-specific scoring rubrics (SaaS, marketplace, consumer, enterprise)
- Integrate with project management tools to pull existing specs
- Add a "quick mode" that skips Socratic questioning for rapid scoring
- Historical tracking of past reviews and their outcomes
- Custom framework plugins (bring your own strategy framework)

## License

[MIT](LICENSE)
