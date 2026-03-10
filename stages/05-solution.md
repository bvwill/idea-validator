# Stage 05 — Solution-Market Fit Check

## Purpose

Evaluate whether the proposed solution actually addresses the validated problem in a way that is differentiated from existing alternatives. This stage connects findings from problem validation (Stage 02), market sizing (Stage 03), and competitive analysis (Stage 04) to the user's solution concept.

---

## Discovery Mode

Ask these questions **one at a time**, adapting based on previous answers:

1. "How does your solution specifically address [validated problem from Stage 02]? Walk me through the core mechanism."
2. "What does a minimum viable version of this look like? What is the smallest thing you could build that delivers the core value?"
3. "Why would someone switch from [top competitor from Stage 04] to your solution? What is the switching trigger?"
4. "What does your solution require from the user that existing alternatives don't? (New behavior, data access, workflow change, etc.)"
5. "Is there a technical or operational capability you have that makes this solution possible for you specifically?"

**Probe deeper when:**
- The solution description is generic ("we make it easier/faster/better") — ask for the specific mechanism
- The differentiation is feature-level only — push for structural advantages (data, distribution, cost structure)
- The MVP sounds like the full product — push for what can be cut

---

## Draft Mode

Using context from prior stages, analyze solution fit autonomously:

1. **Problem-Solution Mapping**: For each validated pain point from Stage 02, assess whether the solution directly addresses it. Flag gaps where the solution solves a different problem than the one validated.
2. **Competitive Gap Exploitation**: Cross-reference Stage 04 competitive gaps. Does the solution target a real opening, or does it compete head-on with entrenched players?
3. **MVP Feasibility Sketch**: Based on the core mechanism, outline what a testable MVP looks like. Identify the single feature that delivers the primary value proposition.
4. **Pivot Triggers**: Explicitly flag if:
   - The solution addresses a problem that was NOT validated in Stage 02
   - The competitive landscape makes the proposed approach unviable
   - The differentiation depends on a capability the user hasn't demonstrated

---

## Gate Criteria

Proceed to Stage 06 when:
- [ ] Solution addresses at least one validated problem from Stage 02
- [ ] Differentiation is articulated beyond feature comparison (structural, not cosmetic)
- [ ] A testable MVP concept exists (not the full product vision)
- [ ] Any pivot triggers have been surfaced and discussed

---

## Confidence Scoring

| Dimension | High | Medium | Low |
|-----------|------|--------|-----|
| Problem-Solution Fit | Solution directly addresses top validated pain point | Addresses a related but secondary pain point | Solves a different problem than validated |
| Differentiation | Structural advantage (data, distribution, cost) | Feature-level advantage with switching trigger | No clear differentiation from alternatives |
| MVP Clarity | Specific, buildable, testable concept defined | General concept but scope unclear | Full product vision only, no scoping |

---

## Output Section

```markdown
## 5. Solution-Market Fit

### Solution Description
[What the solution does, core mechanism, target user]

### Problem-Solution Fit
| Validated Problem | Addressed? | How |
|-------------------|-----------|-----|
| [from Stage 02]   | Yes/Partial/No | [specific mechanism] |

### Differentiation Assessment
[Structural vs. feature-level. What is the switching trigger? Does it exploit a competitive gap from Stage 04?]

### MVP Concept
[Smallest testable version. What is included, what is cut, what does success look like.]

### Pivot Considerations
[If any pivot triggers fired, describe them here. Otherwise: "No pivot triggers identified."]

**Confidence: [High/Medium/Low]**
```
