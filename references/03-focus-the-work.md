# Stage 3: Focus the Work

This stage selects the few branches that deserve deep analysis. A structured strategy-consulting problem-solving process protects senior attention by forcing choices early.

## Partner Input

Ask:

1. Where do you believe the biggest value or risk sits?
2. Which branches must be addressed for stakeholder confidence?
3. Which branches are already understood well enough?
4. What data is easy, hard, or unavailable?
5. Are any topics politically sensitive or off limits?

Treat the user's judgment as important evidence. Challenge only with clear reasoning.

## Prioritization Logic

Score each branch on:

- **Decision impact**: How much the branch could change the answer or recommendation.
- **Tractability**: Whether useful evidence can be gathered in the available time.
- **Stakeholder importance**: Whether the audience expects the topic to be addressed.
- **Uncertainty**: Whether the current answer could be wrong without further work.

## Priority Tiers

| Tier | Meaning | Typical action |
|---|---|---|
| P1 | High decision impact and workable evidence path | Analyze deeply |
| P2 | Important but constrained by data, timing, or dependency | Use proxies or lighter analysis |
| P3 | Low impact, known answer, or outside current scope | Park with rationale |

Aim for two to four P1 focus areas. More than four usually means the team has avoided the hard choices.

## Signals to Elevate

- Large financial or strategic consequence
- Rapid recent change
- High variance across segments
- Direct tie to the decision question
- Strong user or stakeholder emphasis
- Evidence gap that could change the conclusion

## Signals to Park

- Small effect size
- Already answered by prior work
- Weak link to the decision
- Data unavailable within the timeline
- Outside decision authority

## Template

```markdown
---
id: "03-focus-plan"
type: "focus-plan"
stage: 3
title: "Focus Plan"
status: draft
addresses: "01-question-framing.md#dq"
prioritizes:
  - "02-logic-map.md#br-[slug]"
focus_areas:
  - anchor: "03-focus-plan.md#fa-[slug]"
    label: "[Focus area]"
    tier: P1
    branch: "02-logic-map.md#br-[slug]"
parked:
  - branch: "02-logic-map.md#br-[slug]"
    reason: "[Reason]"
---

# Focus Plan

## Priority Assessment
| Branch | Decision impact | Tractability | Stakeholder importance | Priority | Rationale |
|---|---|---|---|---|---|
| [Branch] | High | Medium | High | P1 | [Reason] |

## P1 Focus Areas
### 1. [Focus area]
- **Why it matters**: [Reason]
- **Hypothesis to test**: [Hypothesis]
- **Evidence path**: [Likely data or proxy]

## P2 Topics
[Topics to investigate lightly or through proxies.]

## Parking Lot
| Topic | Why parked | Revisit trigger |
|---|---|---|
| [Topic] | [Reason] | [Trigger] |

## Implications for the Analysis Plan
[How this prioritization shapes Stage 4.]
```

## Review Gate

Ask the user to confirm:

- P1 list
- P2 treatment
- Parking lot
- Data availability assumptions
- Any topic that must be added for politics or credibility

Do not park a branch without user approval.

## Common Failure Modes

- Everything receives equal attention.
- Easy analyses crowd out important questions.
- Parked topics lack a documented rationale.
- Stakeholder expectations are ignored.
- Prioritization uses scores without judgment.
