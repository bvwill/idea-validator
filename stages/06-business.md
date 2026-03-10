# Stage 06 — Business Model Stress Test

## Purpose

Determine whether this idea can be a viable business. Assess the revenue model, sketch unit economics, evaluate customer acquisition channels, and identify the biggest financial risks. This is a sanity check, not a financial model — the goal is to surface fatal flaws and key assumptions before investing in validation.

---

## Discovery Mode

Ask these questions **one at a time**, adapting based on previous answers:

1. "How do you plan to make money? Who pays, how much, and how often?"
2. "How will you reach your first 10 customers? Not at scale — literally the first 10."
3. "What does it cost to deliver your solution to one customer? (Time, infrastructure, content, support, etc.)"
4. "Are there comparable products in this space? What do they charge? How do customers feel about that pricing?"
5. "What is the biggest financial risk — is it that people won't pay, that acquisition costs too much, or that delivery costs don't scale?"

**Probe deeper when:**
- Revenue model is "freemium" or "we'll figure out monetization later" — push for who pays and why
- Acquisition channel is "content marketing" or "social media" with no specifics — ask for the concrete first step
- Unit economics rely on scale that hasn't been validated — flag the chicken-and-egg problem

---

## Draft Mode

Using context from prior stages, analyze business viability autonomously:

1. **Revenue Model Assessment**: Based on comparable products (Stage 04) and market dynamics (Stage 03), evaluate the proposed revenue model. If none was proposed, suggest 2-3 plausible models with tradeoffs.
2. **Unit Economics Sketch**: Estimate per-customer revenue vs. cost to serve. Flag if margins are negative at low scale and identify the break-even point.
3. **Channel Feasibility**: For each potential acquisition channel, assess:
   - Does the target user from Stage 02 actually spend time there?
   - What is the typical cost-to-acquire in this channel for this market?
   - Can the user realistically execute this channel? (Skills, budget, time)
4. **Market Timing Check** *(optional)*: If timing is a key factor (market is early/late, regulatory window, technology shift), call `pm-research/trend-analysis` with the relevant market to assess whether conditions favor entry now.

---

## Gate Criteria

Proceed to Stage 07 when:
- [ ] At least one revenue model is articulated with a price point rationale
- [ ] A plausible first-customer acquisition path exists (not just "marketing")
- [ ] Unit economics are sketched, even if approximate
- [ ] Major financial risks are named (not just "competition")

---

## Confidence Scoring

| Dimension | High | Medium | Low |
|-----------|------|--------|-----|
| Revenue Model | Comparable products validate pricing; willingness-to-pay evidence exists | Plausible model but no direct pricing validation | No clear model or "we'll monetize later" |
| Unit Economics | Positive margins at reasonable scale; cost structure understood | Margins plausible but key costs are estimates | Margins negative or unknown at any scale |
| Acquisition Channel | Specific channel with evidence of target user presence | General channel category identified | No concrete acquisition path |

---

## Output Section

```markdown
## 6. Business Model

### Revenue Model
[Who pays, how much, how often. Rationale for pricing — comparable products, willingness-to-pay signals, or value-based reasoning.]

### Unit Economics Sketch
| Metric | Estimate | Basis |
|--------|----------|-------|
| Revenue per customer | $X/mo or $X/yr | [comparable pricing, proposed pricing] |
| Cost to serve | $X/mo | [infrastructure, content, support estimates] |
| Gross margin | X% | [revenue - cost to serve] |
| Customer acquisition cost | $X | [channel estimate] |
| Payback period | X months | [CAC / monthly margin] |

### Channel Strategy
| Channel | Feasibility | Rationale |
|---------|------------|-----------|
| [channel] | High/Medium/Low | [why this channel, evidence of user presence] |

### Key Financial Risks
1. [Risk] — [why it matters, what would confirm or refute it]
2. [Risk] — [why it matters]

### Market Timing
[If trend analysis was triggered: summary of findings. Otherwise: "No timing concerns identified."]

**Confidence: [High/Medium/Low]**
```
