# Stage 2: Map the Logic

This stage decomposes the approved decision question into a structured logic map. The goal is a practical issue tree that directs analysis, not a theoretical taxonomy. Use the strategy-consulting issue tree mindset: every branch should help prove, disprove, or refine the answer.

## Partner Input

Ask:

1. Do you have a preferred way to break down the problem?
2. Which dimensions must appear in the tree?
3. Should the tree stay executive-level or go into working detail?
4. Which branches already feel most important?
5. Which hypotheses should we test first?

If the user asks you to choose, offer two or three structures with trade-offs and a recommendation.

## MECE Standard

Apply the classic strategy-consulting discipline:

- **Mutually exclusive**: A fact or analysis should belong mainly in one branch.
- **Collectively exhaustive**: Answering every branch should answer the decision question.

Use two tests:

- Completeness test: "If every leaf were answered, would the decision question be answerable?"
- Overlap test: "Would the same data point naturally sit in multiple branches?"

## Common Logic Frames

Use these as starting points. Adapt them to the problem.

### Growth Strategy

```text
How can we reach the growth target?
├── Expand current customers
│   ├── Increase usage
│   ├── Improve retention
│   └── Raise monetization
├── Acquire new customers
│   ├── Improve channel productivity
│   ├── Enter new segments
│   └── Expand geographically
└── Add new offerings
    ├── Build
    ├── Partner
    └── Acquire
```

### Margin Improvement

```text
How can we improve margin sustainably?
├── Revenue quality
│   ├── Pricing
│   ├── Mix
│   └── Discounts
├── Cost structure
│   ├── Direct costs
│   ├── Sales and service costs
│   └── Corporate overhead
└── Operating model
    ├── Process efficiency
    ├── Automation
    └── Governance
```

### Market Entry

```text
Should we enter this market?
├── Market attractiveness
├── Right to win
├── Entry economics
└── Execution risk
```

### Operating Model

```text
What operating model should support the strategy?
├── Capabilities required
├── Decision rights
├── Organization design
├── Process and governance
└── Technology enablement
```

## Hypothesis Rules

For each level-one branch, state a hypothesis that is:

- Specific enough to disprove
- Tied to the decision question
- Testable with available or obtainable evidence
- Useful if confirmed

Weak: "Pricing matters."

Better: "Renewal discounts above 20% are concentrated in three enterprise segments and explain most margin leakage."

## Template

```markdown
---
id: "02-logic-map"
type: "logic-map"
stage: 2
title: "Logic Map"
status: draft
addresses: "01-question-framing.md#dq"
breaks_down: "01-question-framing.md#dq"
branches:
  - anchor: "02-logic-map.md#br-[slug]"
    label: "[Branch]"
    level: 1
branch_hypotheses:
  - anchor: "02-logic-map.md#bh-[slug]"
    label: "[Hypothesis]"
    branch: "02-logic-map.md#br-[slug]"
    test_method: "[Analysis approach]"
---

# Logic Map: [Decision Question]

## Chosen Structure
[Name the frame and why it fits.]

## Issue Tree
[Indented tree.]

## Branch Hypotheses
| Branch | Hypothesis | Test |
|---|---|---|
| [Branch] | [Hypothesis] | [Analysis] |

## MECE Check
- **Overlap check**: [Result]
- **Completeness check**: [Result]
```

## Review Gate

Ask the user to approve:

- Structure choice
- Level-one branches
- Tree depth
- Branch hypotheses
- MECE assessment

If the user changes the structure, rebuild the tree before moving on.

## Common Failure Modes

- The tree copies a standard framework without adapting to the question.
- Level-one branches exceed five and become hard to manage.
- Branches mix causes, actions, and metrics at the same level.
- Hypotheses are too vague to test.
- The user approves the shape but not the underlying logic.
