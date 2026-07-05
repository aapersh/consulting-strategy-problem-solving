# Stage 8: Long-Form Content Rules

Use this guide for memos, reports, board papers, and narrative documents. Long-form content carries more nuance than slides, but it still needs crisp logic and executive pacing. Preserve a strategy-consulting voice: direct answer, structured support, and clear implications for leadership.

## Core Rules

- Lead with the answer.
- Use section headings that help the reader follow the argument.
- Keep paragraphs short.
- Put evidence close to the claim it supports.
- Use tables for comparison, decisions, risks, and roadmaps.
- Include source lines for sections with quantitative claims.

## Section Heading Choices

Ask which style the user prefers:

| Style | Use when | Example |
|---|---|---|
| Message headings | The document should read like a persuasive argument | "Enterprise renewals offer the fastest path to margin recovery" |
| Topic headings | The audience expects a formal report structure | "Enterprise Renewal Economics" |

With topic headings, make the first sentence of each section carry the point.

## Paragraph Standard

Each paragraph should have:

1. A topic sentence that states the point.
2. Two or three sentences of support.
3. A decision implication when useful.

Keep most paragraphs below five sentences.

## Executive Summary

Write two to four short paragraphs. The summary should tell the full story:

- The decision context
- The answer or recommendation
- The strongest reasons
- The expected impact
- The next decision required

Avoid describing the structure of the document. State the argument.

## Evidence Use

Good long-form writing integrates data into the argument.

Weak:

```text
Enterprise retention was 91%. Mid-market retention was 78%. SMB retention was 64%.
```

Stronger:

```text
Enterprise accounts are the most defensible base: 91% retention versus 78% in mid-market and 64% in SMB. That retention gap makes enterprise the logical first focus for pricing discipline.
```

## Recommended Structure

```markdown
---
id: "08-final-content"
type: "long-form-content"
stage: 8
title: "Final Content"
status: draft
addresses: "01-question-framing.md#dq"
presents:
  - "07-recommendation-brief.md#rec-core"
format: "long-form"
---

# [Document Title]

## Executive Summary
[Two to four paragraphs.]

## [Section heading]
[Argument, evidence, implication.]

## [Section heading]
[Argument, evidence, implication.]

## Recommendation
[Core recommendation and supporting moves.]

## Implementation Roadmap
| Phase | Timing | Actions | Owner | Metric |
|---|---|---|---|---|
| [Phase] | [Timing] | [Actions] | [Owner] | [Metric] |

## Risks and Mitigations
| Risk | Impact | Mitigation |
|---|---|---|
| [Risk] | [Impact] | [Mitigation] |

## Decisions Required
1. [Decision]
2. [Decision]
3. [Decision]

## Appendix
[Supporting detail, methods, data tables.]
```

## Tables and Figures

Use tables when they make comparison easier. Introduce each table with the takeaway the reader should see.

Every table or figure with data needs a source line:

```text
Source: [citation]; [citation]
```

## Recommendation Sections

Give each recommendation enough structure to be actionable:

```markdown
## [Action-oriented recommendation heading]

[One or two sentences describing the move.]

**Rationale**: [Evidence and logic.]

**Expected impact**: [Range, basis, confidence.]

**Implementation**: [Owner, timing, milestones.]

**Risks**: [Key risks and mitigations.]
```

## Editing Checklist

- Does the executive summary stand alone?
- Do section headings form a coherent story?
- Does each paragraph make one main point?
- Are claims supported by evidence?
- Are caveats clear but concise?
- Are next decisions visible?

## Common Failure Modes

- The document reads like pasted slide bullets.
- Sections start with throat-clearing.
- Evidence appears as a data dump.
- Recommendations hide inside body paragraphs.
- The appendix absorbs material that belongs in the main argument.
