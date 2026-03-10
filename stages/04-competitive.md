# Stage 4: Competitive Landscape

## Purpose

Map what already exists in this space and identify where a new entrant can credibly differentiate. This stage answers the question every investor and customer will ask: "Why not just use X?" If there is no good answer, the idea needs rethinking before proceeding to solution design.

---

## Discovery Mode

Start by surfacing the user's existing knowledge, then expand with research:

1. **What do you see as competition?** — Direct competitors, adjacent tools, DIY workarounds. Anything the target user might use instead.
2. **Why do you think you can do it better?** — What is your differentiation hypothesis? (Speed, price, UX, focus, integration, some new capability?)
3. **Have you used any of these competitors?** — First-hand experience reveals things research cannot.

After gathering answers, transition to research: "Let me map the full competitive landscape against what you've shared. This will take a few minutes."

Then run the competitive analysis and return with the key finding:

**"Given what exists, why would someone switch to your solution?"**

This is the critical question. If the user cannot articulate a compelling answer after seeing the landscape, that is a signal — not a failure, but a signal that the differentiation thesis needs more work.

---

## Draft Mode

When running autonomously:

1. Review the problem statement, ICP, and market context from Stages 1-3.
2. Run the competitive landscape subskill:

**Read and execute `src/skills/pm-research/competitive-landscape/prompt.md`** with:
- **Topic:** scoped to the validated problem space (e.g., "AI project estimation tools for engineering teams")
- **Focus:** solutions the defined ICP would evaluate
- **Depth:** "quick" for Low confidence ideas, "full" for Medium/High confidence ideas

3. Extract the key findings: player map, feature matrix, whitespace, and table stakes.
4. Assess differentiation viability given what was found.
5. Compile into the output format below.

---

## Gate Criteria

Both must be met to proceed to Stage 5:

- [ ] **Competitive landscape is mapped** — at least the top 3 alternatives are identified with their positioning and key features
- [ ] **Differentiation hypothesis exists** — the user or the analysis has articulated why this solution would be chosen over what already exists

A crowded market is not a blocker. A crowded market with no differentiation thesis is.

---

## Confidence Scoring

| Level | Criteria |
|-------|----------|
| High | Clear whitespace identified, differentiation is defensible, user has first-hand competitive knowledge |
| Medium | Differentiation exists but is narrow, or competitive data is incomplete |
| Low | Market is crowded with no clear angle, or too new for competitive data to exist |

If confidence is Low, flag that the solution design stage (Stage 5) must address differentiation head-on.

---

## Output Section

Write this section into the running validation document:

```markdown
## 4. Competitive Landscape

**Competitor Map:**

| Player | Type | Target | Key Strength | Key Weakness |
|--------|------|--------|-------------|-------------|
| [Name] | Incumbent/Challenger/Niche/Emerging | [who they serve] | [strength] | [weakness] |
| [Name] | ... | ... | ... | ... |
| [Name] | ... | ... | ... | ... |

**Differentiation Thesis:** [One paragraph: why would the target user choose this solution over the best available alternative? What is the wedge?]

**Positioning Gaps:** [Underserved segments or unmet needs no current player addresses well]

**Table Stakes:** [Capabilities any serious competitor must have — the cost of entry]

**Competitive Confidence:** {High|Medium|Low} — {brief justification}

**Key Risk:** [The single biggest competitive risk — e.g., "Incumbent X could ship this feature in a quarter"]
```

The full competitive analysis is saved separately by the competitive-landscape subskill. Reference its location here.
