# CEO Scorecard: Feature Evaluation Template

## Scoring Dimensions

Rate each dimension from 1 to 10. Be honest. A 7 should be genuinely strong, not "seems okay." Most features should cluster around 4-6. A 9 or 10 is exceptional and rare.

---

### 1. Strategic Alignment (1-10)

Does this feature advance the company's core mission and long-term strategy?

| Score | Criteria |
|-------|----------|
| 1-3 | Tangential to core strategy. Could be a separate product. Does not reinforce the company's competitive position or long-term vision. Feels opportunistic rather than intentional. |
| 4-6 | Loosely connected to strategy. Supports an adjacent use case or secondary persona. Defensible as "on-strategy" but not obviously so. Would not appear on a one-page strategy doc. |
| 7-10 | Directly advances the core mission. Strengthens the primary value proposition. Would appear on a one-page strategy doc. Makes the overall product more coherent and focused. |

---

### 2. Market Opportunity (1-10)

Is there a real, sizable market for this? Are real users experiencing real pain?

| Score | Criteria |
|-------|----------|
| 1-3 | Speculative demand. No quantitative evidence of user need. Based on intuition, a few anecdotes, or competitor mimicry. Target audience is vague or undefined. |
| 4-6 | Some evidence of demand: support tickets, survey data, or a identifiable segment requesting it. Market size is modest or unclear. Pain exists but may not be acute. |
| 7-10 | Strong quantitative evidence: significant volume of requests, measurable churn or conversion impact, large addressable segment. Pain is acute and frequent. Users are actively seeking alternatives. |

---

### 3. Defensibility / Moat (1-10)

Does this make the product harder to replicate or leave? Does it create lasting advantage?

| Score | Criteria |
|-------|----------|
| 1-3 | Easily copied. No switching costs. No data advantage. No network effects. A competitor could ship this in weeks. Commodity feature. |
| 4-6 | Moderate defensibility. Some integration depth or data leverage. Would take a competitor months to replicate. Creates mild switching costs. |
| 7-10 | Strong moat. Leverages proprietary data, network effects, or deep integration. Creates significant switching costs. Compounds over time -- gets stronger with usage. Competitors cannot easily replicate the value. |

---

### 4. Distribution Feasibility (1-10)

Can you actually get this in front of users? Is there a clear path to adoption?

| Score | Criteria |
|-------|----------|
| 1-3 | No distribution plan. Requires users to discover the feature on their own. No existing channel or habit to leverage. Requires behavior change with no clear incentive. |
| 4-6 | Leverages an existing channel but requires some effort to drive awareness. May need onboarding or education. Adoption path exists but is not frictionless. |
| 7-10 | Natural distribution through existing user flows. Discoverable within current product experience. Low friction to adopt. Has viral or organic growth potential. Users will pull it rather than needing to be pushed. |

---

### 5. Unit Economics / Financial Value (1-10)

Does the math work? Will this generate or protect revenue at acceptable cost?

| Score | Criteria |
|-------|----------|
| 1-3 | No clear revenue impact. High build and maintenance cost relative to value. Negative or unknown unit economics. Cannot articulate how this translates to financial outcomes. |
| 4-6 | Indirect revenue impact through retention or engagement. Moderate build cost. Unit economics are plausible but unproven. Financial case requires assumptions. |
| 7-10 | Direct, measurable revenue impact. Strong unit economics with evidence or credible projections. Build cost is proportionate to expected return. Clear path to positive ROI within a defined timeframe. |

---

### 6. Risk Profile (1-10, inverted scale)

What is the downside exposure? Lower score means riskier.

| Score | Criteria |
|-------|----------|
| 1-3 | High risk. Large resource commitment. Irreversible or expensive to unwind. Depends on multiple unproven assumptions. Significant technical uncertainty. Reputational risk if it fails. |
| 4-6 | Moderate risk. Manageable resource commitment. Partially reversible. Some proven, some unproven assumptions. Technical approach is known but execution is non-trivial. |
| 7-10 | Low risk. Small resource commitment. Easily reversible if it fails. Most assumptions are validated. Technical approach is well-understood. Limited downside. |

---

## Calculating the Verdict

Compute the simple average of all six dimension scores.

| Average Score | Verdict | Meaning |
|---------------|---------|---------|
| 7.0 or above | **BUILD** | Strong case. Proceed with defined milestones and kill criteria. |
| 5.0 - 6.9 | **DEFER** | Promising but incomplete. Identify what must be true to reach BUILD, and go validate those assumptions before committing resources. |
| Below 5.0 | **KILL** | Weak case. Do not invest further unless fundamental conditions change. Redirect resources to higher-impact work. |

**Important**: The average is a starting point, not gospel. A single dimension scoring 1-2 can override a high average if it represents a fatal flaw. Note any such overrides explicitly in the verdict.

---

## Output Format

Present the final scorecard in this format:

```
## Feature Scorecard: [Feature Name]

| Dimension                        | Score | Rationale |
|----------------------------------|-------|-----------|
| Strategic Alignment              | X/10  | [1-2 sentence justification] |
| Market Opportunity               | X/10  | [1-2 sentence justification] |
| Defensibility / Moat             | X/10  | [1-2 sentence justification] |
| Distribution Feasibility         | X/10  | [1-2 sentence justification] |
| Unit Economics / Financial Value | X/10  | [1-2 sentence justification] |
| Risk Profile                     | X/10  | [1-2 sentence justification] |

**Average Score: X.X / 10**

### Verdict: [BUILD / DEFER / KILL]

[2-3 sentence summary of the key reasoning behind the verdict.]

### Key Risks
1. [Risk 1]
2. [Risk 2]
3. [Risk 3]

### Conditions for [Proceeding / Reconsideration]
1. [Condition 1 with measurable criteria]
2. [Condition 2 with measurable criteria]
3. [Condition 3 with measurable criteria]

### Kill Criteria
- [Specific metric and threshold that would trigger killing this feature]
- [Timeline for evaluation]
```

---

## Scoring Discipline

- Do not inflate scores to be encouraging.
- Do not cluster all scores around 5-6 to avoid commitment. Take a position.
- A score of 10 means "best in class, no meaningful weakness in this dimension." Use it rarely.
- A score of 1 means "complete failure in this dimension." Use it when warranted.
- Every score must have a rationale. A number without reasoning is worthless.
- If you lack information to score a dimension, say so and score it as a 3 (assume the worst when evidence is missing).
