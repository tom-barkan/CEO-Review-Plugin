# Socratic Questioning Patterns for CEO Review

Use these questions during the interrogation phase of a feature evaluation. Do not ask them all. Select the most relevant questions based on the conversation. Ask one at a time. Wait for a response before proceeding.

Escalate from Value & Problem toward Success Metrics as the conversation progresses.

---

## Value & Problem

These questions establish whether a real problem exists and whether the proposed feature solves it.

1. **"Who is paying for this?"** -- If no one is willing to pay, the value is speculative. Free features still have a cost: engineering time, maintenance burden, product complexity. Identify the buyer.

2. **"What happens if we don't build it?"** -- The most revealing question. If the answer is "nothing much changes," the feature is not essential. Force the user to articulate the concrete negative consequences of inaction.

3. **"How are users solving this today?"** -- If users have found workarounds, the pain is real but the urgency may be lower. If they have no workaround, the pain may be acute. If they are using a competitor's solution, that is a signal worth investigating.

4. **"Can you show me the data?"** -- Anecdotes are not evidence. Demand quantitative support: support ticket volume, churn analysis, survey results, usage data. If the data does not exist, that is a finding.

5. **"Describe the user who needs this most. Be specific."** -- Vague personas ("busy professionals") indicate shallow understanding. Push for specificity: role, company size, workflow, frequency of the pain, willingness to pay.

---

## Strategy

These questions test whether the feature strengthens the company's long-term position.

6. **"How does this compound over time?"** -- The best features get more valuable with usage, data, or network effects. If the value is static, it is a commodity. Look for compounding loops.

7. **"Does this make us harder to compete with?"** -- Every feature should either deepen the moat or serve as a stepping stone toward deepening the moat. If it does neither, question why it exists.

8. **"What are we saying NO to by saying yes to this?"** -- Resources are zero-sum. Every feature built displaces something else. Force the user to name the trade-off explicitly. If they cannot, they have not thought about prioritization.

9. **"If a competitor launched this tomorrow, how would we feel?"** -- Tests whether this is truly strategic or merely nice-to-have. If the answer is "we'd be fine," the urgency is low. If the answer is "we'd be in trouble," dig into why.

---

## Financial

These questions verify that the feature makes economic sense.

10. **"What's the expected revenue impact?"** -- Demand a number. A range is acceptable. "We don't know" is honest but means the financial case is unproven. Push for estimation methodology even if the number is rough.

11. **"What do the unit economics look like?"** -- Cost to build, cost to maintain, cost per user served. Compare against the revenue or retention value generated per user. If the user cannot sketch this out, the financial thinking is immature.

12. **"How will you price this?"** -- Relevant for monetizable features. Pricing strategy reveals how well the user understands the value they are delivering. If they have not thought about pricing, they have not thought about value.

---

## Distribution

These questions test whether the feature can reach users at scale.

13. **"How does a user discover this?"** -- If the answer requires a blog post, a tutorial, or an email campaign, adoption will be slow. The best features are discoverable within the natural product flow.

14. **"What's the acquisition cost?"** -- For features targeting new users or new segments, what does it cost to bring someone in? If the feature requires expensive distribution, the unit economics may not work.

15. **"Does this have viral or organic growth potential?"** -- Features that spread through usage (sharing, collaboration, output artifacts) have fundamentally different economics than features that require paid distribution.

---

## Risk

These questions surface hidden dangers and test the user's intellectual honesty.

16. **"What's the pre-mortem? Assume it failed -- why?"** -- Forces the user out of optimism mode. The best builders can articulate exactly how their feature could fail. If they cannot, they are not seeing the full picture.

17. **"What's the biggest assumption we're making?"** -- Every feature rests on assumptions. Identify the load-bearing one. If that assumption is wrong, does the entire case collapse? How will you test it before committing full resources?

18. **"What's the reversibility if this doesn't work?"** -- Some features can be quietly removed. Others create permanent obligations (data formats, API contracts, user expectations). Irreversible decisions demand higher conviction.

19. **"What's the second-order effect?"** -- Beyond the direct impact, what behaviors does this feature enable or encourage? Could it cannibalize an existing feature? Could it create perverse incentives? Think two steps ahead.

---

## Success Metrics

These questions ensure accountability and prevent vague "it went well" post-mortems.

20. **"How will you measure success?"** -- Demand specific metrics, not vague outcomes. "Improve engagement" fails. "Increase 7-day retention from 34% to 40% within 90 days" passes.

21. **"What does the 30/60/90 day metric look like?"** -- Establishes a timeline for evaluation with checkpoints. Leading indicators at 30 days should predict whether the 90-day target is achievable.

22. **"What's the kill criteria?"** -- The most important question in this category. What specific result would cause you to shut this down? If the user resists defining kill criteria, they are emotionally attached to the feature and not thinking clearly about resource allocation.

---

## How to Use These Questions

- **Start with Value & Problem** to establish whether the foundation is solid. If the user cannot answer questions 1-5 convincingly, the later categories are moot.
- **Move to Strategy** only after value is established. A feature can solve a real problem and still be strategically wrong.
- **Financial and Distribution** questions expose whether the feature is viable at scale, not just desirable in theory.
- **Risk questions** should be asked after the user has built their case. It is more revealing to challenge a fully articulated position than a half-formed one.
- **End with Success Metrics** to ensure that whatever decision is made has clear accountability attached to it.

Do not treat this as a checklist. Read the conversation. Identify the weakest part of the user's reasoning and press on it. Skip questions that have already been answered. Double down on areas where the user is vague, defensive, or contradictory.
