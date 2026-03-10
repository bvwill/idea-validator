# Idea Validator

A structured validation coach for product ideas. Instead of a checklist or spreadsheet, this walks you through 8 stages of validation as a conversation, then produces a scored report with confidence levels and next steps.

## What Problem Does This Solve?

PMs have ideas constantly. The hard part is figuring out which ones are worth pursuing before you invest weeks of engineering time or burn political capital pitching something half-baked.

Most validation approaches fall into two camps: a quick gut check ("the market feels big") or a 40-page business plan nobody reads. This sits in between. It forces you to answer the hard questions, one at a time, with evidence instead of optimism.

## Who Is This For?

- PMs evaluating new products, features, or business ideas
- Founders pressure-testing an early concept before building
- Product leaders deciding which bets to fund next quarter

If you have an idea and the next step feels like "just start building," this is the thing to do first.

## How It Works

The validation runs through 8 stages, each building on the last:

| Stage | What It Covers |
|-------|---------------|
| 1. Intake | What's the idea? Who has the problem? Why now? |
| 2. Problem | Is the problem real, frequent, and painful enough to pay for? |
| 3. Market | Who specifically has this problem? How big is the opportunity? |
| 4. Competitive | Who else is solving this? Where are the gaps? |
| 5. Solution | Does your proposed solution actually fit the validated problem? |
| 6. Business | Do the unit economics work? What's the go-to-market? |
| 7. Gaps | What assumptions have zero evidence? What's the plan to test them? |
| 8. Synthesis | Scorecard, go/no-go assessment, and concrete next steps |

Two modes:

- **Discovery (default):** Conversational. The coach asks one question at a time, challenges your assumptions, runs research mid-conversation, and builds the report as you go.
- **Draft (`--draft`):** The coach does an autonomous first pass using whatever context you provide, then walks you through the findings section by section, starting with the weakest areas.

Each stage has gate criteria. You can't skip ahead. If you don't have evidence for a claim, it gets flagged as an assumption, not glossed over.

## When to Use It

- Before committing engineering resources to a new idea
- Before pitching to leadership (the report becomes your evidence base)
- When evaluating a competitive move or market shift
- When you have a hunch but no structured analysis behind it

## Key Decisions and Tradeoffs

**Why conversational coaching over a checklist?**
Checklists let you fill in answers without thinking. A coaching conversation pushes back. When you say "the market is big," it asks "how do you know?" That friction is the point.

**Why 8 stages?**
Each stage maps to a dimension that matters for go/no-go decisions. Problem, market, competition, solution fit, business model, evidence gaps, and synthesis. Fewer stages skip important angles. More stages create busywork.

**What's the scoring methodology?**
Each dimension gets a confidence level (High, Medium, Low) based on the quality and quantity of evidence, not on whether the finding is positive or negative. A well-researched "this market is too small" scores High confidence. A hopeful "the market feels huge" scores Low. The overall assessment synthesizes across dimensions.

**Why does it flag assumptions instead of just answering them?**
Some questions can only be answered by talking to real customers or building a prototype. The coach distinguishes between what it found (evidence), what it inferred (analysis), and what nobody knows yet (assumptions). That honesty is more useful than false confidence.

## How to Use It

This is a [Claude Code](https://docs.anthropic.com/en/docs/claude-code) skill. Run it with the slash command:

```
/validate "AI-powered onboarding tool for mid-market SaaS companies"
```

With additional context files:

```
/validate "AI-powered onboarding tool" --context @interview-notes.md @market-research.md
```

Draft mode (autonomous first pass, then collaborative review):

```
/validate "AI-powered onboarding tool" --draft
```

### Setup

1. Clone this repo into your Claude Code skills directory
2. Add a slash command in `.claude/commands/` that reads `prompt.md`

The skill reads its stage files, templates, and examples at runtime. No build step, no dependencies.

## Example Output

See [`examples/example-validation.md`](examples/example-validation.md) for a complete validation report on an AI-powered onboarding tool. It demonstrates:

- Varied confidence levels across dimensions (High for Problem, Low for Solution Fit)
- A scorecard that leads with the verdict, not the reasoning
- An assumption map that prioritizes what to validate first
- Concrete next steps with timeframes and decision criteria
- Honest assessment of competitive threats and timing risk

## File Structure

```
idea-validator/
├── README.md
├── prompt.md                # Main skill prompt
├── stages/
│   ├── 01-intake.md         # Idea intake and problem framing
│   ├── 02-problem.md        # Problem validation
│   ├── 03-market.md         # ICP and market sizing
│   ├── 04-competitive.md    # Competitive landscape
│   ├── 05-solution.md       # Solution-market fit
│   ├── 06-business.md       # Business model stress test
│   ├── 07-gaps.md           # Evidence gap analysis
│   └── 08-synthesis.md      # Scorecard and recommendations
├── templates/
│   ├── validation-report.md # Output report template
│   └── interview-script.md  # Customer interview script template
└── examples/
    └── example-validation.md # Complete example report
```
