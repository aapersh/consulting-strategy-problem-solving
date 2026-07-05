# Stage 1: Frame the Question

The first stage turns a broad concern into one decision-oriented question. Spend enough time here to remove ambiguity before analysis begins. Use a strategy-consulting framing habit: force the work toward the exact question an executive needs answered.

## Partner Input

Ask before drafting:

1. What situation triggered this work?
2. What decision, action, or recommendation must come out of it?
3. What would a successful answer enable?
4. What is in scope by product, geography, segment, time horizon, and decision rights?
5. What constraints matter: budget, timing, politics, data, regulation, capability?
6. What do you already suspect is true?

Use the user's wording where it is crisp. If their framing contains a hidden solution, step back to the business question that sits underneath it.

## Deliverable

Create `01-question-framing.md` with:

- Situation context
- Decision question
- Scope boundaries
- Success measures
- Constraints
- Stakeholder map
- Starting hypotheses

## Decision Question Patterns

Convert a loose prompt into a question that implies action.

| Starting prompt | Stronger question pattern |
|---|---|
| "Our renewals are weakening" | "What is driving renewal weakness in [segment], and what actions can restore retention by [date]?" |
| "We may need a partner strategy" | "Which partnership model should we pursue, and what economics would justify it?" |
| "The sales team misses forecast" | "Which forecast drivers are least reliable, and how should the commercial operating model change?" |
| "The product roadmap feels crowded" | "Which product bets deserve priority given customer value, margin impact, and delivery capacity?" |

Good strategy-consulting questions have four traits:

- They name the decision.
- They define the unit of analysis.
- They include a practical time horizon.
- They leave room for multiple answers.

## Scope Discipline

Be explicit about:

- Geography
- Customer or product segments
- Time horizon
- Financial metric or operating metric
- Implementation authority
- Exclusions

If a boundary is missing, ask. Do not fill it silently.

## Template

```markdown
---
id: "01-question-framing"
type: "question-framing"
stage: 1
title: "Question Framing"
status: draft
addresses: null
entities:
  decision_question:
    anchor: "01-question-framing.md#dq"
    text: "[Decision question]"
  success_measures:
    - anchor: "01-question-framing.md#sm-[slug]"
      label: "[Success measure]"
      metric: "[Metric or test]"
  starting_hypotheses:
    - anchor: "01-question-framing.md#hyp-[slug]"
      label: "[Hypothesis]"
---

# Question Framing

## Context
[Brief account of the situation, trigger, and stakes.]

## Decision Question
> [One clear question that points toward a decision.]

## Scope
- **Included**: [Boundaries]
- **Excluded**: [Boundaries]
- **Time horizon**: [Period]

## Success Measures
[How the answer will be judged.]

## Constraints
[Budget, time, data, politics, regulation, capability.]

## Stakeholders
| Stakeholder | Role | What they care about |
|---|---|---|
| [Name or group] | [Decision-maker, influencer, operator] | [Interest] |

## Starting Hypotheses
1. [Hypothesis to test]
2. [Hypothesis to test]
3. [Hypothesis to test]
```

## Review Gate

Present the draft and ask the user to confirm:

- Does the decision question capture the real issue?
- Are scope boundaries right?
- Are success measures useful?
- Are constraints complete?
- Which hypotheses should be added, removed, or sharpened?

Do not move to Stage 2 until the user approves the question framing.

## Common Failure Modes

- The question is too broad to answer with available time.
- The wording assumes the answer.
- Scope boundaries remain vague.
- Success measures describe activity rather than outcomes.
- Stakeholder concerns are discovered too late.
