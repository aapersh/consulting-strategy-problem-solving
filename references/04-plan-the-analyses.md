# Stage 4: Plan the Analyses

This stage converts focus areas into a practical workplan. Each analysis should answer one question, test one piece of logic, or size one important implication. The strategy-consulting bias is toward a short, sharp analysis plan that can change the answer, not a long inventory of interesting work.

## Partner Input

Ask:

1. What internal data can you provide?
2. Which analyses will stakeholders expect to see?
3. What timing, milestones, or decision meetings constrain the work?
4. Which methods are acceptable: model, benchmark, interview, survey, process review, scenario analysis?
5. What level of estimation is acceptable where data is missing?

## Deliverable

Create an analysis plan. Use a spreadsheet when the user wants a live workplan, and include a markdown summary for traceability.

Recommended workbook tabs:

- **Overview**: decision question, workstreams, milestones, owners, status
- **Analysis inventory**: one row per analysis
- **Data register**: required data, source, owner, status, workaround
- **Dependency map**: gating analyses, parallel work, follow-up decisions

## Analysis Inventory Fields

| Field | Purpose |
|---|---|
| ID | Stable reference such as `WS1-A1` |
| Workstream | P1 focus area served |
| Question | Specific question answered |
| Method | Analytical approach |
| Data required | Inputs needed |
| Source or owner | Where data comes from |
| Status | Have, requested, gap, proxy |
| Output | Chart, table, model, memo, interview synthesis |
| Hypothesis | Expected answer |
| Dependency | Prior analysis or decision needed |
| Confidence target | High, medium, or directional |

## Method Menu

Use the simplest method that can answer the question.

- Trend analysis
- Cohort or segment analysis
- Driver tree
- Benchmarking
- Unit economics
- Sensitivity model
- Scenario model
- Process map
- Stakeholder interview synthesis
- Competitive teardown
- Risk assessment

## Sequencing

Classify analyses:

- **Gating**: must finish before choosing a direction.
- **Parallel**: can run independently.
- **Confirmatory**: validates a likely answer.
- **Optional**: useful only if earlier findings point there.

## Template

```markdown
---
id: "04-analysis-plan"
type: "analysis-plan"
stage: 4
title: "Analysis Plan"
status: draft
addresses: "01-question-framing.md#dq"
plans:
  - "03-focus-plan.md#fa-[slug]"
workstreams:
  - anchor: "04-analysis-plan.md#ws-[slug]"
    label: "[Workstream]"
    focus_area: "03-focus-plan.md#fa-[slug]"
analyses:
  - anchor: "04-analysis-plan.md#ax-ws1-a1"
    label: "[Analysis]"
    workstream: "04-analysis-plan.md#ws-[slug]"
---

# Analysis Plan

## Workstream Overview
| Workstream | Linked focus area | Analyses | Key dependency | Milestone |
|---|---|---:|---|---|
| [Name] | [Focus area] | [#] | [Dependency] | [Date] |

## Analysis Inventory
| ID | Workstream | Question | Method | Data required | Source | Status | Hypothesis | Dependency |
|---|---|---|---|---|---|---|---|---|
| WS1-A1 | [Name] | [Question] | [Method] | [Data] | [Source] | [Status] | [Hypothesis] | [Dependency] |

## Data Register
| Data item | Owner or source | Status | Workaround |
|---|---|---|---|
| [Data] | [Owner] | [Have or gap] | [Proxy] |

## Sequencing Notes
[What runs first, what runs in parallel, and what gates later work.]
```

## Review Gate

Ask the user to approve:

- Analysis list
- Data assumptions
- Workstream sequencing
- Proxy choices
- Timeline and milestones

Do not begin Stage 5 until the analysis plan is approved.

## Common Failure Modes

- Analyses are named as broad topics rather than answerable questions.
- Data sources are missing.
- Dependencies appear during execution because sequencing was skipped.
- The plan is too large for the decision timeline.
- Proxy assumptions are accepted without user review.
