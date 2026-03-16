---
name: strategic-frameworks
description: This skill should be used when the user asks about "7 Powers", "Porter's Five Forces", "Blue Ocean", "JTBD", "Wardley Mapping", "TAM SAM SOM", "Kano Model", "RICE scoring", "ICE scoring", "strategic analysis", "competitive strategy", "market sizing", "feature evaluation frameworks", "what framework should I use", "analyze the competitive landscape", "size the market", "prioritize features", or needs to apply business strategy frameworks to evaluate features, products, or strategic decisions.
version: 0.1.0
---

# Strategic Frameworks for Feature & Product Evaluation

Apply the following business strategy frameworks when evaluating features, products, or strategic decisions. Each framework illuminates a different dimension of strategic value. Select the appropriate framework based on the type of question being asked, or combine multiple frameworks for a comprehensive evaluation.

Strategic evaluation is not about applying a single lens. The best feature decisions emerge from layering complementary frameworks: one to validate demand, another to assess competitive dynamics, and a third to quantify and prioritize. The frameworks below are organized from customer-facing (demand validation) through structural (competitive positioning) to quantitative (prioritization and sizing).

## Framework Overview

### Hamilton Helmer's 7 Powers

The 7 Powers framework, from Hamilton Helmer's book of the same name, identifies the only seven sources of durable competitive advantage that allow a business to sustain differential returns over time. The seven powers are: Scale Economies (unit cost declines with volume), Network Effects (value grows with each user), Counter-Positioning (a model incumbents cannot adopt without self-damage), Switching Costs (the pain of leaving), Branding (durable reputation-based value attribution), Cornered Resource (exclusive access to talent, data, patents), and Process Power (embedded processes that are nearly impossible to replicate). Apply this framework when evaluating whether a feature creates or strengthens a lasting strategic moat. A feature that does not create or reinforce at least one power may generate short-term value but is unlikely to sustain differentiation.

### Porter's Five Forces

Porter's Five Forces analyzes the competitive intensity and attractiveness of a market by examining five structural forces: threat of new entrants (how easily can newcomers enter?), bargaining power of suppliers (how much leverage do they hold?), bargaining power of buyers (can customers pressure pricing?), threat of substitutes (what alternatives exist?), and competitive rivalry (how intense is head-to-head competition?). Use this framework to assess how a feature affects the company's position relative to these forces and whether it shifts industry dynamics in the company's favor. A strong feature investment raises barriers to entry, reduces buyer power, or neutralizes substitute threats. A weak one inadvertently commoditizes the offering or escalates rivalry without margin improvement.

### Blue Ocean Strategy (Value Innovation)

Blue Ocean Strategy focuses on creating uncontested market space rather than competing head-to-head in existing "red ocean" markets. Its core tool is the Eliminate-Reduce-Raise-Create (ERRC) grid, which challenges assumptions about which factors of competition matter by asking what to eliminate entirely, what to reduce below industry standard, what to raise above standard, and what to create new. Value innovation, the cornerstone of the strategy, occurs when differentiation and cost reduction are pursued simultaneously. Apply this when evaluating whether a feature opens new demand or merely fights for share in a crowded space. Features that attract non-customers are particularly high-signal blue ocean moves.

### Jobs-to-be-Done (JTBD)

JTBD frames customer needs as "jobs" that people hire products to accomplish, encompassing functional, emotional, and social dimensions. It shifts focus from demographics and feature lists to the underlying progress a customer seeks in a specific circumstance. The canonical job statement follows the pattern: "When [situation], I want to [motivation], so I can [expected outcome]." Use this framework to evaluate whether a feature addresses a real, high-priority job that customers are actively trying to solve. The strongest feature candidates address jobs that are important, frequent, and poorly satisfied by existing alternatives, where customers resort to costly or inconvenient workarounds.

### Wardley Mapping

Wardley Mapping, created by Simon Wardley, plots components of a value chain along two axes: visibility to the user (y-axis) and evolutionary stage (x-axis, from Genesis through Custom-Built, Product, to Commodity). Every component inevitably evolves rightward toward commoditization over time, and the map reveals where to invest in differentiation versus where to leverage commodity solutions. Apply this when deciding whether a feature targets the right evolutionary stage, when assessing build-vs-buy decisions, or when evaluating strategic timing. A feature that custom-builds a commodity wastes resources; a feature that commoditizes a lower layer to enable genesis-stage innovation above it is strategically powerful.

### TAM/SAM/SOM (Market Sizing)

TAM (Total Addressable Market) represents the entire revenue opportunity if a product achieved 100% share globally. SAM (Serviceable Addressable Market) narrows to segments reachable given the company's business model, geography, and capabilities. SOM (Serviceable Obtainable Market) is the realistic near-term capture given competition and go-to-market capacity. Market sizing can be done top-down (industry reports), bottom-up (unit economics times customer count), or via value-theory (willingness to pay for value delivered). Use this framework to ground feature decisions in revenue potential and validate that an opportunity is worth pursuing. Features that expand SAM by unlocking new segments are often more strategically valuable than those that marginally improve conversion within existing SOM.

### RICE and ICE Scoring

RICE (Reach, Impact, Confidence, Effort) and ICE (Impact, Confidence, Ease) are quantitative prioritization frameworks that score features on standardized dimensions to enable apples-to-apples comparison. RICE calculates as (Reach x Impact x Confidence) / Effort, where Reach is measured in users or events per time period, Impact on a scale from minimal (0.25) to massive (3), Confidence as a percentage, and Effort in person-months. ICE is simpler: Impact (1-10) x Confidence (1-10) x Ease (1-10). Apply these when ranking multiple features against each other and needing a defensible numerical basis. These are prioritization tools, not strategy tools: they answer "in what order" but not "whether" a feature is strategically sound. Always pair with a strategic framework for context.

### Kano Model

The Kano Model, developed by Noriaki Kano, classifies features into categories based on their nonlinear relationship to customer satisfaction. Must-Have (Basic) features do not increase satisfaction when present but cause strong dissatisfaction when absent (e.g., security, uptime). Performance (Linear) features increase satisfaction proportionally to execution quality (e.g., speed, capacity). Delighters (Attractive) features create disproportionate satisfaction when present but cause no dissatisfaction when absent (e.g., a surprisingly elegant experience). A critical dynamic is Kano decay: over time, today's delighters become tomorrow's performance features and eventually must-haves as customer expectations rise. Use this to determine the strategic category of a feature, whether it drives differentiation or merely prevents churn, and whether the roadmap has a healthy balance across all three categories.

## Quick-Reference: Question-to-Framework Mapping

| Question Type | Primary Framework | Supporting Framework |
|---|---|---|
| "Does this feature build a moat?" | 7 Powers | Porter's Five Forces |
| "How big is the opportunity?" | TAM/SAM/SOM | RICE Scoring |
| "What do customers actually need?" | JTBD | Kano Model |
| "Are we competing or creating?" | Blue Ocean Strategy | Wardley Mapping |
| "How should we prioritize this?" | RICE / ICE Scoring | Kano Model |
| "Will this delight or just satisfy?" | Kano Model | JTBD |
| "Where does this sit in the value chain?" | Wardley Mapping | Porter's Five Forces |
| "Can competitors easily copy this?" | 7 Powers | Porter's Five Forces |
| "Should we build, buy, or partner?" | Wardley Mapping | TAM/SAM/SOM |
| "Is this market attractive?" | Porter's Five Forces | Blue Ocean Strategy |

## How to Conduct a Multi-Framework Evaluation

When performing a comprehensive strategic evaluation of a feature or product, layer the frameworks in this sequence:

1. Start with JTBD to confirm there is a real customer job worth solving.
2. Size the opportunity with TAM/SAM/SOM to confirm the job is commercially meaningful.
3. Assess the competitive landscape with Porter's Five Forces to understand structural pressures.
4. Evaluate strategic differentiation using Blue Ocean Strategy (are we creating or competing?).
5. Check for durable advantage with 7 Powers (will this advantage persist?).
6. Position the feature with Wardley Mapping to confirm evolutionary timing.
7. Classify using the Kano Model to understand the satisfaction dynamics.
8. Score with RICE or ICE to compare against other candidates in the backlog.

Present findings as a structured assessment with clear go/no-go signals and risk flags.

## Output Format for Strategic Assessment

When delivering a multi-framework evaluation, structure the output as follows:

1. **Executive Summary**: One-paragraph verdict with the primary recommendation (proceed, pivot, or pass) and the single most important reason.
2. **Demand Validation** (JTBD + Kano): State the job, classify the feature category, and summarize customer evidence.
3. **Market Opportunity** (TAM/SAM/SOM): Provide bottom-up and top-down estimates with key assumptions stated explicitly.
4. **Competitive Landscape** (Porter's Five Forces + Blue Ocean): Describe which forces are affected, whether this creates or contests market space, and how competitors are likely to respond.
5. **Strategic Durability** (7 Powers + Wardley): Identify which powers are created or strengthened, evolutionary stage, and expected longevity of advantage.
6. **Prioritization Score** (RICE or ICE): Provide the numerical score with each component justified, and compare to the top three alternatives in the current backlog.
7. **Risk Flags**: List the top three risks with severity and mitigation options.
8. **Recommendation**: Go/no-go with conditions, sequencing guidance, and suggested validation steps before full commitment.

## Common Pitfalls to Avoid

- **Framework theater**: Applying frameworks without genuine analysis to justify a predetermined conclusion. Each framework should genuinely inform the decision, not decorate it.
- **Single-framework tunnel vision**: Relying on one framework (typically RICE) while ignoring strategic context. A high RICE score means nothing if the feature commoditizes a core differentiator.
- **Ignoring Kano decay**: Treating a feature as a delighter when competitors have already made it table stakes. Always benchmark against current market expectations, not last year's.
- **Confusing TAM with opportunity**: A large TAM does not mean a feature is worth building. SOM is the number that matters for near-term planning; TAM matters for long-term trajectory.
- **Over-indexing on novelty**: Blue Ocean thinking is powerful but not every feature needs to be a category creator. Sometimes the right move is to execute a performance feature better than anyone else.

## Detailed Reference

For full framework explanations, application guides, key diagnostic questions, and red/green flag indicators, consult the detailed reference at `references/frameworks-guide.md`.
