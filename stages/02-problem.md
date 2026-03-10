# Stage 2: Problem Validation

## Purpose

Validate that the problem identified in Stage 1 actually exists beyond the founder's assumption and is painful enough to drive behavior change. This stage separates real problems from imagined ones before investing effort in market sizing or competitive analysis.

---

## Discovery Mode

Ask these questions **one at a time**, adapting based on responses:

1. **How do you know this is real?** — What evidence do you have that people actually experience this problem?
2. **Who have you talked to?** — Have you spoken with potential users? How many? What did they say?
3. **How painful is it?** — On a scale of "mild annoyance" to "hair on fire," where does this land? What's the cost of the status quo?
4. **How often does it happen?** — Is this a daily friction, a quarterly headache, or a once-in-a-career event?
5. **Are people already paying to solve it?** — Do they spend money, time, or political capital on workarounds?

After gathering answers, summarize the evidence and give an honest assessment: "Based on what you've shared, here's where problem validation stands."

---

## Draft Mode

When running autonomously from a brief:

1. Review the problem statement and target user from Stage 1.
2. Search for evidence that the problem exists in the wild:
   - `"{problem space} frustration pain point"` — forums, Reddit, community posts
   - `"{target user role} challenges {problem domain} 2025 2026"` — industry surveys and reports
   - `"{problem space} workaround hack"` — signs people are actively working around the problem
3. Search for counter-evidence:
   - `"{problem space} solved by {existing solution}"` — has this already been adequately addressed?
4. Assess severity: frequency x impact x willingness to pay.
5. Compile findings into the output format below.
6. Flag if evidence is thin — recommend user interviews before proceeding.

---

## Gate Criteria

At least two must be met to proceed to Stage 3:

- [ ] **External evidence exists** — the problem appears in forums, surveys, reviews, or industry reports (not just the founder's head)
- [ ] **Severity is meaningful** — the problem is frequent enough or costly enough that someone would change behavior to solve it
- [ ] **People are already spending** — there is evidence of money, time, or effort being spent on workarounds

If only one criterion is met, proceed with a Low confidence flag and a recommendation to gather primary data. If zero are met, recommend pausing the validation until the user can conduct user interviews.

---

## Confidence Scoring

| Level | Criteria |
|-------|----------|
| High | Primary data from 5+ user conversations, or strong quantitative evidence (surveys, market data) |
| Medium | Desk research confirms the problem — forum posts, review complaints, industry reports |
| Low | Assumption only — no external evidence found, or evidence is anecdotal and thin |

If confidence drops from Stage 1, note the shift and why.

---

## Output Section

Write this section into the running validation document:

```markdown
## 2. Problem Validation

**Evidence Summary:**
- [Source 1]: [what it shows]
- [Source 2]: [what it shows]
- [Source 3]: [what it shows]

**Severity Assessment:**
- Frequency: {daily|weekly|monthly|quarterly|rare}
- Impact: {high|medium|low} — [brief justification]
- Willingness to pay: {strong|moderate|weak|unknown} — [evidence]

**Counter-Evidence:** [anything suggesting the problem is already solved or not as painful as assumed]

**Problem Confidence:** {High|Medium|Low} — {brief justification}

**Recommendation:** {Proceed|Proceed with caution|Pause for user interviews}
```
