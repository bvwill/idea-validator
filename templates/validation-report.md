# Validation Report Template

This template defines the output format for all idea validations. Each section maps to one or more pipeline stages. The synthesis stage (08) assembles the final report.

---

## Output Format

```markdown
---
date: {YYYY-MM-DD}
idea: "{idea title}"
mode: {discovery|draft}
status: {Draft|Validated|Invalidated}
overall_confidence: {High|Medium|Low}
---

# Idea Validation: {Idea Title}

## Executive Summary

[3-5 sentences. Written last, during synthesis. State the overall assessment — validated, invalidated, or needs more evidence. Lead with the single most important finding. Mention the strongest and weakest dimensions.]

## Validation Scorecard

| Dimension | Confidence | Key Finding |
|-----------|-----------|-------------|
| Problem | {High/Medium/Low} | {One-sentence finding} |
| Market Size | {High/Medium/Low} | {One-sentence finding} |
| Competition | {High/Medium/Low} | {One-sentence finding} |
| Solution Fit | {High/Medium/Low} | {One-sentence finding} |
| Business Model | {High/Medium/Low} | {One-sentence finding} |

**Overall: {High/Medium/Low}** — {One-sentence rationale for overall confidence}

## 1. Problem & Opportunity

### Problem Statement

[Clear articulation of the problem. Who has it? How often? What is the cost of the status quo?]

### Evidence

[What evidence supports that this problem exists and matters? Cite sources.]

### Who Has This Problem

[Target persona(s) with specifics — role, company size, industry, context.]

### Severity Assessment

- **Frequency:** {How often does this problem occur?}
- **Impact:** {What happens when it does?}
- **Willingness to pay:** {Are people already spending money to solve it?}

## 2. Target Market

### Ideal Customer Profile

[Specific description of the best-fit customer. Not "everyone" — the narrowest viable segment.]

### Market Sizing

| Metric | Estimate | Basis |
|--------|----------|-------|
| TAM | {$X} | {methodology — top-down or bottom-up with source} |
| SAM | {$X} | {segment constraints applied} |
| SOM | {$X} | {realistic near-term capture with assumptions} |

### Market Dynamics

[Growth rate, key trends, tailwinds or headwinds relevant to this idea.]

## 3. Competitive Landscape

### Competitive Map

| Competitor | Category | Strengths | Weaknesses | Pricing |
|-----------|----------|-----------|------------|---------|
| {Name} | {Direct/Indirect/Substitute} | {Key strengths} | {Key gaps} | {Pricing model} |

### Differentiation Assessment

[How would this idea differentiate? Is the gap defensible? What would it take for incumbents to close it?]

### Competitive Risk

[Biggest competitive threat and why. What could make differentiation irrelevant?]

## 4. Solution Fit

### Proposed Solution

[Brief description of what the solution does and how it addresses the problem.]

### Value Proposition

[One clear statement: "For {customer} who {problem}, {solution} provides {benefit} unlike {alternatives}.]

### Feasibility Assessment

- **Technical complexity:** {Low/Medium/High} — {brief rationale}
- **Time to MVP:** {estimate with key assumptions}
- **Key technical risks:** {what could go wrong}

### Evidence of Fit

[Any signal that this solution approach works — analogies, prototypes, customer conversations, similar products in adjacent markets.]

## 5. Business Model

### Revenue Model

[How does this make money? Pricing structure, tiers, expected ACV.]

### Unit Economics (Estimated)

| Metric | Estimate | Assumption |
|--------|----------|-----------|
| ACV | {$X} | {basis} |
| CAC | {$X} | {channel assumptions} |
| LTV | {$X} | {retention and expansion assumptions} |
| LTV:CAC | {X:1} | {assessment: healthy >3:1, marginal 1-3:1, unsustainable <1:1} |

### Go-to-Market

[Primary acquisition channel(s). Why these channels fit the ICP. What early traction would look like.]

## 6. Assumptions & Evidence Gaps

### Assumption Map

| # | Assumption | Criticality | Evidence Level | Validation Plan |
|---|-----------|-------------|---------------|-----------------|
| 1 | {assumption} | {Critical/Important/Nice-to-know} | {Strong/Moderate/Weak/None} | {How to test — interview, prototype, data, etc.} |

### Highest-Risk Assumptions

[Call out the 2-3 assumptions that, if wrong, would invalidate the idea. These are the priority for next steps.]

## 7. Recommended Next Steps

### Priority Actions

1. **{Action}** — {Why this is next. What it would prove or disprove. Effort estimate.}
2. **{Action}** — {Why. What it proves. Effort.}
3. **{Action}** — {Why. What it proves. Effort.}

### Decision Framework

- **Proceed if:** {what evidence would you need to see?}
- **Pivot if:** {what signals suggest the idea needs significant changes?}
- **Kill if:** {what would make this clearly not worth pursuing?}

## Sources

| # | Source | Type | Confidence |
|---|--------|------|-----------|
| 1 | {source name or URL} | {Analyst/Filing/Product/News/Interview} | {High/Medium/Low} |

*Confidence: High = named analyst firm, public filing, or direct customer interview; Medium = industry press, product data, or expert opinion; Low = aggregator, estimate, or older than 18 months.*
```

---

## Confidence Rating Guide

Use these definitions consistently across all dimensions:

- **High** — Multiple independent sources confirm. Evidence is recent (<12 months), specific, and from credible sources. Key assumptions are well-supported.
- **Medium** — Some supporting evidence but gaps remain. Sources may be indirect, older, or limited in number. Reasonable to proceed but specific risks need attention.
- **Low** — Mostly assumption-based. Little direct evidence found. Key claims are unvalidated. Significant research or testing needed before committing resources.

## Overall Status

- **Validated** — Majority of dimensions are Medium or High confidence. No critical assumptions at "None" evidence level. Clear path to next steps.
- **Draft** — Analysis is in progress or evidence is too thin to make a call. More research needed.
- **Invalidated** — One or more critical dimensions are Low confidence with evidence pointing against the idea, OR a fatal flaw was identified (e.g., market too small, problem already solved well, economics don't work).
