# Stage 7: Shape the Recommendation

This stage translates the integrated answer into choices, actions, economics, timing, and risks. A recommendation should tell the decision-maker what to do next and why that path beats the alternatives. Use a strategy-consulting recommendation posture: direct, option-aware, evidence-backed, and practical enough to assign to an owner.

## Partner Input

Ask:

1. Which strategic direction are you leaning toward?
2. Which options are unacceptable because of politics, risk, cost, or timing?
3. What level of change is the organization willing to absorb?
4. Who must approve the recommendation?
5. What investment range is realistic?
6. What has been tried before?

When the user has a strong preference, build around it and test it against evidence.

## Recommendation Standard

Each recommendation should be:

- Specific: names the action
- Measurable: includes a success metric where possible
- Feasible: fits resources and constraints
- Relevant: traces to the integrated answer
- Timed: includes sequence and milestones
- Evidence-backed: links to findings and insights

## Option Development

Before writing the final brief, present two or three strategic options:

| Option | Description | Upside | Trade-off | Fit with evidence |
|---|---|---|---|---|
| [Option A] | [What it means] | [Benefit] | [Cost or risk] | [Fit] |
| [Option B] | [What it means] | [Benefit] | [Cost or risk] | [Fit] |
| [Option C] | [What it means] | [Benefit] | [Cost or risk] | [Fit] |

State which option you would choose and why. Ask the user to decide or revise.

## Recommendation Architecture

Use a simple pyramid:

```text
Core recommendation
├── Supporting move 1
├── Supporting move 2
└── Supporting move 3
```

Each supporting move needs:

- What to do
- Why it matters
- Expected impact
- Timing
- Owner
- Evidence link

## Phasing

Use phases that create momentum:

| Phase | Timing | Purpose |
|---|---|---|
| Mobilize | 0 to 90 days | Decisions, quick wins, team setup |
| Scale | 3 to 12 months | Major implementation and operating changes |
| Institutionalize | 12 months and beyond | Capabilities, governance, measurement |

Adjust timing to the user's industry and decision cycle.

## Template

```markdown
---
id: "07-recommendation-brief"
type: "recommendation-brief"
stage: 7
title: "Recommendation Brief"
status: draft
addresses: "01-question-framing.md#dq"
recommends:
  anchor: "07-recommendation-brief.md#rec-core"
  label: "[Core recommendation]"
  supported_by:
    - "06-integrated-answer.md#ins-[slug]"
supporting_moves:
  - anchor: "07-recommendation-brief.md#move-[slug]"
    label: "[Move]"
    supported_by:
      - "05-analysis-findings.md#f-[slug]"
---

# Recommendation Brief

## Options Considered
| Option | Upside | Trade-off | Recommendation |
|---|---|---|---|
| [Option] | [Upside] | [Trade-off] | [Chosen or rejected] |

## Core Recommendation
> [One or two sentences naming the recommended path.]

**Rationale**: [Why this path follows from the integrated answer.]

**Expected impact**: [Range, basis, confidence.]

## Supporting Moves

### 1. [Move]
- **Action**: [What to do]
- **Reason**: [Evidence and insight]
- **Impact**: [Expected result]
- **Owner**: [Role]
- **Timing**: [Period]

## Implementation Roadmap
| Phase | Timing | Actions | Owner | Success metric |
|---|---|---|---|---|
| Mobilize | [Timing] | [Actions] | [Owner] | [Metric] |

## Economics and Impact
| Move | Investment | Annual impact | Payback | Confidence |
|---|---|---|---|---|
| [Move] | [Range] | [Range] | [Period] | [Level] |

## Risks, Objections, and Mitigations
| Risk or objection | Likely concern | Response |
|---|---|---|
| [Risk] | [Concern] | [Mitigation] |

## Next Decisions
1. [Decision or action]
2. [Decision or action]
3. [Decision or action]

## Story-Ready Summary
- [Core move in one crisp line]
- [Supporting move with impact]
- [Implementation phase with owner]
```

## Review Gate

Ask the user to approve:

- Chosen option
- Core recommendation
- Supporting moves
- Impact ranges and confidence
- Phasing
- Risk and objection handling

Do not move to Stage 8 until the recommendation brief is approved.

## Common Failure Modes

- Recommendation sounds like a theme rather than an action.
- Options are skipped, so the user cannot compare paths.
- Impact is asserted without evidence.
- Implementation is too vague for owners to act.
- Objections are handled after the presentation rather than before.
