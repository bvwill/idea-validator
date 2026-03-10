# Stage 3: ICP & Market Sizing

## Purpose

Define who specifically has the validated problem and how big the opportunity is. This stage takes the problem from Stage 2 and puts boundaries around it — who exactly is the customer, how many of them exist, and what is the market worth. Without this, every other decision (pricing, GTM, positioning) is guesswork.

---

## Discovery Mode

Build the ICP collaboratively by asking these questions **one at a time**:

1. **What role does your ideal customer hold?** — Job title, function, seniority level.
2. **What kind of company are they at?** — Size (employees or revenue), industry, stage (startup, growth, enterprise).
3. **What's their budget authority?** — Can they buy independently, or do they need approval? What's a reasonable price they'd pay?
4. **Where do they congregate?** — Communities, events, publications, Slack groups. This signals reachability.
5. **Who is explicitly NOT the customer?** — Defining who you're not building for is as important as who you are.

After gathering answers, present the ICP profile and confirm: "Does this describe the person you'd most want as your first 10 customers?"

Then transition to research: "Now I'll size the market for this ICP. This will take a few minutes."

---

## Draft Mode

When running autonomously:

1. Review the problem statement, target user, and problem evidence from Stages 1-2.
2. Construct an ICP from available information. Flag any dimensions that are assumed rather than stated.
3. Run the market sizing subskill:

**Read and execute `src/skills/pm-research/market-sizing/prompt.md`** with:
- **Topic:** scoped to the validated problem + ICP (e.g., "AI-powered project estimation tools for mid-market engineering teams")
- **Focus:** the specific segment defined by the ICP
- **Depth:** "quick" for Low confidence ideas, "full" for Medium/High confidence ideas

4. Extract the key figures (TAM/SAM/SOM, CAGR) from the market sizing output.
5. Compile into the output format below.

---

## Gate Criteria

Both must be met to proceed to Stage 4:

- [ ] **ICP is defined** — specific enough to identify real people (not "SMBs" or "tech companies" without further scoping)
- [ ] **Market size has a floor** — at least a rough SAM estimate exists, even if the range is wide

If the market sizing research returns very thin data, note it as a risk factor rather than a blocker — some markets are emerging and poorly measured.

---

## Confidence Scoring

| Level | Criteria |
|-------|----------|
| High | Named analyst estimates for the market, ICP validated by user interviews |
| Medium | Bottom-up estimate from reasonable assumptions, ICP based on founder's direct experience |
| Low | Market is too new or niche for reliable sizing data, ICP is assumed |

Confidence here is a composite of ICP confidence and market data quality.

---

## Output Section

Write this section into the running validation document:

```markdown
## 3. ICP & Market Sizing

**ICP Profile:**
- Role: [title, function, seniority]
- Company: [size, industry, stage]
- Budget: [authority level, expected price sensitivity]
- Where to find them: [communities, channels, events]
- Explicitly not: [who is excluded and why]

**Market Size:**
- TAM: ${X} ({range}) — [one-line methodology]
- SAM: ${X} ({range}) — [segment constraints applied]
- SOM: ${X} ({range}) — [realistic capture assumptions]
- CAGR: {X}% — [source]

**Key Assumptions:** [2-3 assumptions the market estimate depends on most]

**Market Confidence:** {High|Medium|Low} — {brief justification}
```

The full market sizing analysis is saved separately by the market-sizing subskill. Reference its location here.
