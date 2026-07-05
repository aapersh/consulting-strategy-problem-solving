# Stage 6: Integrate the Answer

This stage turns approved findings into a coherent answer. The work shifts from analysis to judgment: what the evidence means, how the pieces connect, and where uncertainty remains. Use a strategy-consulting synthesis lens: the output should read as a point of view, not a research recap.

## Partner Input

Ask:

1. Which finding feels most important to you?
2. Which result would surprise or worry stakeholders?
3. What organizational context should shape the interpretation?
4. Which tensions in the evidence matter most?
5. How bold should the answer be?

The user's context helps decide what to lead with, what to qualify, and what to handle carefully.

## Synthesis Method

1. Lay out the major findings by workstream.
2. Cluster findings that point to the same implication.
3. Identify tensions or exceptions.
4. Build a logic chain from evidence to insight to answer.
5. Pressure-test the answer against the decision question.
6. State confidence and what could change the answer.

## Pattern Types

| Pattern | Meaning | Response |
|---|---|---|
| Converging evidence | Independent findings point to the same answer | Lead with confidence |
| Evidence tension | Findings pull in different directions | Explain the trade-off |
| Sequence dependency | The right action depends on order | Recommend phases |
| Conditional answer | A key uncertainty remains unresolved | Present scenarios |
| Missing proof | Evidence is too thin for a firm claim | Lower confidence or request more data |

## Integrated Answer Standard

The answer should:

- Address the decision question directly.
- Use three to five supporting insights.
- Show how evidence connects.
- Acknowledge the strongest counterargument.
- State confidence plainly.

## Template

```markdown
---
id: "06-integrated-answer"
type: "integrated-answer"
stage: 6
title: "Integrated Answer"
status: draft
addresses: "01-question-framing.md#dq"
synthesizes:
  - "05-analysis-findings.md#f-[slug]"
answer:
  anchor: "06-integrated-answer.md#answer"
  text: "[Answer]"
insights:
  - anchor: "06-integrated-answer.md#ins-[slug]"
    label: "[Insight]"
    supported_by:
      - "05-analysis-findings.md#f-[slug]"
confidence:
  overall: medium
---

# Integrated Answer

## Answer
> [One or two sentences that directly answer the decision question.]

## Supporting Insights

### 1. [Insight headline]
[Explain the insight and cite the strongest evidence.]

### 2. [Insight headline]
[Explain the insight and cite the strongest evidence.]

### 3. [Insight headline]
[Explain the insight and cite the strongest evidence.]

## Logic Chain
[Show how the insights combine into the answer.]

## Counterarguments and Uncertainties
| Challenge | Why it matters | Response or mitigation |
|---|---|---|
| [Challenge] | [Reason] | [Response] |

## Confidence Assessment
- **Overall confidence**: [High/Medium/Low]
- **Strongest evidence**: [Where the case is best supported]
- **Weakest evidence**: [Where the case is thinnest]
- **What would change the answer**: [Trigger]
```

## Review Gate

Present the integrated answer and ask:

- Does the answer match the evidence and your context?
- Which insight should lead?
- What alternative interpretation should we show?
- Is the confidence level right?
- Are any stakeholder concerns missing?

Do not move to Stage 7 until the user approves the integrated answer.

## Common Failure Modes

- Findings are listed without forming an argument.
- The answer is buried below supporting detail.
- Evidence tension is hidden.
- Confidence language sounds stronger than the data.
- The user sees the story differently and the draft fails to adapt.
