# Stage 1: Idea Intake & Problem Framing

## Purpose

Get clear on what the idea is, who it's for, and why now. This stage transforms a raw idea into a structured problem statement that the remaining stages can validate against. Nothing proceeds until the problem framing is sharp.

---

## Discovery Mode

Ask these questions **one at a time**, waiting for each answer before asking the next. Adapt follow-ups based on responses.

1. **What's the idea?** — Describe what you want to build or offer in plain language.
2. **Who has this problem?** — Who specifically experiences this pain? Be as concrete as possible (role, company size, context).
3. **What do they do today?** — How do people currently solve or work around this problem?
4. **Why hasn't this been solved?** — What has prevented existing solutions from addressing this well?
5. **Why now?** — What has changed (technology, market, regulation, behavior) that makes this the right time?

After gathering answers, synthesize them into the output format below and confirm with the user: "Here's how I'm framing the problem. Does this capture it accurately?"

---

## Draft Mode

When a written brief is provided instead of a conversation:

1. Extract answers to all five intake questions from the brief.
2. Flag any questions the brief does not address — list them as **gaps**.
3. If 3+ questions are unanswered, pause and ask the user to fill gaps before proceeding.
4. If 1-2 questions are unanswered, note assumptions and proceed with a confidence penalty.
5. Synthesize into the output format below.

---

## Gate Criteria

All three must be met to proceed to Stage 2:

- [ ] **Clear problem statement** — one sentence describing who has what problem
- [ ] **Target user defined** — specific enough to find and talk to (not "everyone" or "businesses")
- [ ] **Timing thesis** — a reason this is the right time, not just a good idea in general

If gate criteria are not met, loop back with targeted follow-up questions on the missing elements.

---

## Confidence Scoring

| Level | Criteria |
|-------|----------|
| High | User has direct experience with the problem or target users |
| Medium | User has observed the problem secondhand or has adjacent experience |
| Low | Idea is based on assumption or pattern-matching without direct exposure |

Record the confidence level — it carries forward and affects how aggressively later stages challenge assumptions.

---

## Output Section

Write this section into the running validation document:

```markdown
## 1. Idea Intake & Problem Framing

**Problem Statement:** [One sentence: {Target user} struggles with {problem} because {root cause}.]

**Target User:** [Specific description — role, context, company type, seniority]

**Current Alternatives:** [What they do today — workarounds, competitors, manual processes, or nothing]

**Timing Thesis:** [Why now — the change that creates the opening]

**Intake Confidence:** {High|Medium|Low} — {brief justification}

**Open Questions:** [Any unresolved gaps flagged for later stages]
```
