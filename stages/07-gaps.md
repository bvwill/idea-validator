# Stage 07 — Qualitative Data Gap Analysis

## Purpose

This is the core differentiator of the validate skill. Every prior stage produced findings based on desk research and the user's assertions. This stage systematically identifies what we are still *assuming* without primary evidence, and generates concrete, actionable validation plans to get real signal from real people. The output is not "do more research" — it is specific scripts, experiments, and surveys the user can execute this week.

---

## Discovery Mode

Walk through the assumptions map with the user **one category at a time**:

1. "Let me walk you through what we're confident about vs. what we're still assuming. For the problem — [summarize Stage 02 findings]. The evidence here came from [sources]. What direct conversations have you had with potential users about this problem?"
2. "For the market and competitive landscape — [summarize Stages 03-04]. This is based on desk research. Have you talked to anyone who uses [competitor] or buys in this space?"
3. "For the solution and business model — [summarize Stages 05-06]. These are largely our projections. Have you tested pricing, shown a prototype, or described the concept to potential customers?"
4. "Based on these gaps, here are the assumptions I think are most critical to validate. Which of these feel most uncertain to you?"
5. "For each critical gap, I have a specific validation plan. Let me walk you through the options and we can pick the right approach for your situation."

**Probe deeper when:**
- User says "I've talked to people" — ask how many, what they said, whether it was structured
- User is confident about an assumption — ask what evidence supports it specifically
- User wants to skip validation — explain the risk of the specific assumption being wrong

---

## Draft Mode

This is a structured analytical process. Execute all steps before presenting findings.

### Step 1: Build the Assumptions Map

Review every finding from Stages 02-06. For each claim, classify its evidence:

| Evidence Type | Definition | Examples |
|--------------|-----------|----------|
| **Primary** | Direct signal from target users or customers | User interviews, surveys, prototype tests, sales conversations, usage data |
| **Secondary** | Desk research about the market or problem | Analyst reports, competitor reviews, forum posts, published case studies |
| **Assumption** | No direct evidence; inferred or asserted | "Users would pay $X", "The market is underserved", "People want this feature" |

Map every key finding:

```
| Stage | Finding | Evidence Type | Source | Confidence |
|-------|---------|--------------|--------|------------|
| 02 - Problem | [finding] | Primary/Secondary/Assumption | [source] | H/M/L |
| 03 - Market | [finding] | ... | ... | ... |
| 04 - Competitive | [finding] | ... | ... | ... |
| 05 - Solution | [finding] | ... | ... | ... |
| 06 - Business | [finding] | ... | ... | ... |
```

### Step 2: Identify Critical Assumptions

Filter the map for findings that are:
- Evidence type = **Assumption** or **Secondary only**
- AND the finding is load-bearing (other conclusions depend on it)

Rank by criticality:
- **Critical**: If wrong, the entire idea fails (e.g., "the problem exists", "people will pay")
- **Important**: If wrong, the approach needs significant change (e.g., "this channel works", "the MVP scope is right")
- **Nice-to-know**: If wrong, minor adjustments needed (e.g., "exact pricing tier", "secondary feature priority")

### Step 3: Generate Validation Plans

For each Critical and Important assumption, generate a specific validation plan using ONE of these approaches:

#### Option A: Customer Discovery Interviews
Best for: Problem validation, solution feedback, willingness-to-pay
- Generate a **focused interview script** (5-7 questions, 20 minutes)
- Questions must be open-ended and non-leading (no "Would you use a product that...?")
- Include: opening context, core questions, follow-up probes, closing
- Specify: target interviewee profile, where to find them, sample size (minimum 5)
- Template reference: `templates/interview-script.md` (if available)

**Script structure:**
```
Opening: "I'm exploring [problem space]. I'd love to understand your experience with [topic]."
Q1: [Current behavior question — how do they handle this today?]
Q2: [Pain/frequency question — how often, how painful?]
Q3: [Alternatives question — what have they tried?]
Q4: [Value question — what would solving this be worth?]
Q5: [Solution reaction — describe concept, get reaction]
Closing: "Who else should I talk to about this?"
```

#### Option B: Smoke Test / Landing Page Experiment
Best for: Demand validation, willingness-to-pay, feature prioritization
- Describe the specific test (landing page, fake door, waitlist, pre-order)
- Define the success metric and threshold (e.g., ">5% email signup rate from 200 visitors")
- Specify traffic source and budget needed
- Estimate time to run: typically 1-2 weeks

#### Option C: Community Survey
Best for: Quantifying known problems, validating market segments, pricing research
- Generate **5-10 targeted questions** (mix of multiple choice and scale)
- Specify target respondent profile and where to distribute
- Define minimum sample size for statistical relevance (typically 30-50)
- Include one open-ended question for unexpected insights

#### Option D: Competitive User Interviews
Best for: Understanding switching triggers, unmet needs, willingness to pay more
- Target: current users of the top 1-2 competitors from Stage 04
- Generate a script focused on: what they use, what they wish were different, what they've tried
- Specify where to find these users (communities, review sites, LinkedIn)
- Sample size: 3-5 per competitor

### Step 4: Recommend and Prioritize

For each gap, recommend the best validation approach based on:
- Speed to signal (interviews are fastest, experiments take longer)
- User's resources (time, budget, access to target users)
- Criticality of the assumption (critical assumptions get the fastest method)

Estimate total validation effort:
- Number of interviews/surveys/experiments needed
- Calendar time to complete
- Minimum viable sample sizes

---

## Gate Criteria

Proceed to Stage 08 when:
- [ ] Every finding from Stages 02-06 is mapped to an evidence type
- [ ] All Critical assumptions are identified with validation plans
- [ ] All Important assumptions are identified (plans optional but recommended)
- [ ] At least one interview script or experiment design is fully specified
- [ ] Validation plans include concrete next steps (not just "talk to users")

---

## Confidence Scoring

| Dimension | High | Medium | Low |
|-----------|------|--------|-----|
| Assumptions Coverage | All stages mapped, no blind spots | Most stages mapped, 1-2 gaps in coverage | Major stages have unmapped findings |
| Plan Specificity | Scripts written, metrics defined, sample sizes set | General approach identified for each gap | "Do more research" level of specificity |
| Prioritization | Clear critical path, sequenced by dependency | Priorities identified but sequencing unclear | Flat list with no prioritization |

---

## Output Section

```markdown
## 7. Qualitative Data Gap Analysis

### Assumptions Map

| # | Stage | Finding | Evidence | Source | Criticality |
|---|-------|---------|----------|--------|-------------|
| 1 | Problem | [finding] | Primary/Secondary/Assumption | [source] | Critical/Important/Nice-to-know |
| 2 | Market | [finding] | ... | ... | ... |
| ... | ... | ... | ... | ... | ... |

**Summary:** X findings mapped. Y based on primary evidence. Z are assumptions requiring validation.

### Critical Assumptions (Must Validate)

#### Assumption: [description]
- **Why critical:** [what breaks if this is wrong]
- **Recommended approach:** [A/B/C/D] — [name]
- **Validation plan:** [specific details — script, experiment design, or survey questions]
- **Target:** [who to talk to / test with]
- **Where to find them:** [specific communities, channels, methods]
- **Sample size:** [minimum needed]
- **Time to signal:** [estimated days/weeks]

[Repeat for each critical assumption]

### Important Assumptions (Should Validate)

[Same structure as critical, but may have less detailed plans]

### Validation Roadmap

| Priority | Assumption | Method | Time | Dependencies |
|----------|-----------|--------|------|-------------|
| 1 | [assumption] | [method] | X days | None |
| 2 | [assumption] | [method] | X days | Depends on #1 |
| ... | ... | ... | ... | ... |

**Total estimated validation time:** [X weeks if sequential, Y weeks if parallelized]

**Confidence: [High/Medium/Low]**
```
