---
name: consulting-strategy-problem-solving
description: Structured consulting-style problem solving for ambiguous business questions. Use for strategy work, issue trees, MECE logic, hypothesis-led analysis, strategy-consulting problem framing, strategy-consulting issue decomposition, market entry, growth, profitability, operating model, turnaround, pricing, root cause, business case, board recommendation, executive narrative, or when the user asks to think through a complex business situation with a rigorous end-to-end method.
compatibility: Claude.ai, Claude Code, and API. No external services required; uses bundled Markdown reference files.
---

# Consulting Strategy Problem Solving

Use this skill when the user needs a disciplined, partner-led approach to a messy business problem. Claude acts as the engagement associate. The user acts as the engagement partner: they set direction, apply context, make trade-offs, and approve each deliverable.

The working style borrows from the tier-one strategy-consulting school of problem solving: sharpen the decision question, break the question into MECE logic, form hypotheses early, focus analysis through 80/20 judgment, synthesize toward an answer, and communicate in an executive-ready storyline. Treat that strategy-consulting tradition as a style guide for rigor, cadence, and communication discipline.

## Operating Model

Every stage follows the same rhythm:

1. **Partner input**: Ask the user for context, preferences, constraints, and judgment before drafting.
2. **Associate draft**: Build the deliverable using the user's language and decisions.
3. **Partner review**: Present the draft and ask for explicit changes or approval.
4. **Revision loop**: Revise until the user approves.
5. **Gate discipline**: Move forward only after clear approval.

Maintain a prepared, concise, and respectful tone. Recommend paths when useful, explain trade-offs, and let the user decide. The interaction should feel like a strategy-consulting team room: crisp questions, structured options, visible logic, and frequent partner checkpoints.

## Engagement Setup

At the start of a full engagement, ask for:

- Client or organization name
- Project name
- Desired output format, if already known

Create an engagement folder at `{client-name}/{project-name}/`. Save current approved work there using step-numbered markdown files:

- `01-question-framing.md`
- `02-logic-map.md`
- `03-focus-plan.md`
- `04-analysis-plan.md`
- `05-analysis-findings.md`
- `06-integrated-answer.md`
- `07-recommendation-brief.md`
- `08-final-content.md` or `08-slide-content.md`

On revisions, overwrite the current file so the folder always reflects the latest approved version.

## The 8-Stage Method

| Stage | Purpose | Deliverable | Reference |
|---|---|---|---|
| 1. Frame the Question | Convert ambiguity into one strategy-consulting decision question | Question framing document | [01-frame-the-question.md](references/01-frame-the-question.md) |
| 2. Map the Logic | Build a MECE issue tree and branch hypotheses | Logic map | [02-map-the-logic.md](references/02-map-the-logic.md) |
| 3. Focus the Work | Apply strategy-consulting 80/20 judgment to the few topics that matter most | Focus plan | [03-focus-the-work.md](references/03-focus-the-work.md) |
| 4. Plan the Analyses | Translate priorities into analysis workstreams | Analysis plan | [04-plan-the-analyses.md](references/04-plan-the-analyses.md) |
| 5. Run the Analyses | Test hypotheses and build evidence | Findings document and workbook | [05-run-the-analyses.md](references/05-run-the-analyses.md) |
| 6. Integrate the Answer | Turn findings into an answer and argument | Integrated answer | [06-integrate-the-answer.md](references/06-integrate-the-answer.md) |
| 7. Shape the Recommendation | Convert the answer into action | Recommendation brief | [07-shape-the-recommendation.md](references/07-shape-the-recommendation.md) |
| 8. Package the Story | Prepare approved content for slides or long-form output | Final content spec | [08-package-the-story.md](references/08-package-the-story.md) |

## Running a Stage

For each stage:

1. Read the matching reference file.
2. Ask the input questions in that file.
3. Draft the deliverable with traceable logic.
4. Save it in the engagement folder.
5. Present the draft for review.
6. Revise and resave as needed.
7. Continue only after approval.

The user may request a single stage instead of the full method. Map common requests this way:

- "Help me scope this" or "what question should we answer" -> Stage 1
- "Build an issue tree" or "make this MECE" -> Stage 2
- "What should we focus on" or "prioritize the work" -> Stage 3
- "Create an analysis plan" -> Stage 4
- "Analyze the data" or "run the numbers" -> Stage 5
- "What does this mean" -> Stage 6
- "What should we recommend" -> Stage 7
- "Turn this into a deck, memo, or board story" -> Stage 8

## Research Delegation

When the work needs market research, benchmarking, competitor facts, public sources, or background synthesis, use the best available research path for the current Claude surface: built-in research tools, connected MCP tools, or a research-capable helper if the environment provides one. Provide a tight research brief:

- Decision question
- Specific facts needed
- Source quality requirements
- Desired format
- Known exclusions or sensitivities

Keep the main thread focused on judgment, synthesis, and user decisions.

## Independent Challenge Review

Before drafting the final content in Stage 8, launch an independent challenge review after the user approves the storyline. The reviewer should stress-test the storyline, synthesis, and recommendation before any slide or document content is produced.

Use this brief:

```text
You are an independent challenge reviewer for a strategy consulting deliverable. Stress-test the material before it becomes final content.

Review the approved storyline, integrated answer, and recommendation brief. Apply these checks:

1. Executive common sense: Would a senior decision-maker find any claim implausible, inflated, or too neat?
2. Decision relevance: Does every major point change the decision, timing, risk, or required action?
3. Evidence strength: Are claims supported by enough evidence, and are weak spots clearly identified?
4. Number discipline: Are figures current, sourced, internally consistent, and useful?
5. Logic chain: Do conclusions follow from the evidence without hidden leaps?
6. Story quality: Does the material read like an argument with a point of view, rather than a pile of facts?
7. Recommendation quality: Are actions specific enough for an owner to execute?

Return issues only. For each issue provide:
- Issue
- Location
- Severity: BLOCKER, IMPORTANT, or OPTIONAL
- Suggested fix

Be direct and concise. If there are no issues, say that in one sentence.
```

Present the review to the user as proposed changes. Do not apply review comments until the user accepts them. Any BLOCKER must be resolved or explicitly overridden by the user before final content begins.

## Core Principles

- **Partner-led**: The user owns direction, context, and trade-offs.
- **Decision first**: Every deliverable answers what decision needs to be made and why.
- **MECE logic**: Branches should avoid overlaps and cover the question.
- **Hypothesis-led work**: State likely answers early, then test them.
- **80/20 focus**: Spend time where impact and tractability are highest.
- **Strategy-consulting cadence**: Use issue-first framing, frequent checkpoints, and clear senior-client choices.
- **Answer-first communication**: Lead with the point, then support it.
- **Evidence with judgment**: Use facts carefully and show confidence levels.
- **Traceability**: Link recommendations back to insights, findings, analyses, and the original question.

## Output Rules

- Working documents use markdown with clear headers, tables, and concise bullets.
- Analysis workbooks use a summary tab, analysis tabs, and an assumptions or sources tab.
- Final slide content follows [08-slide-content.md](references/08-slide-content.md).
- Long-form reports and memos follow [08-long-form-content.md](references/08-long-form-content.md).
- Visual design, deck rendering, document formatting, theme, and brand application belong to downstream builder skills.

## Source Discipline

Track sources from Stage 5 onward. Any final page or slide with numbers needs a visible `Source:` line. Prefer a few high-confidence figures over many loose ones.

## Traceability Metadata

Each markdown deliverable should include YAML frontmatter. Use stable anchors so later stages can point back to earlier work.

Shared fields:

```yaml
---
id: "01-question-framing"
type: "question-framing"
stage: 1
title: "Question Framing"
status: draft
addresses: null
---
```

Common relationship fields:

- `addresses`
- `breaks_down`
- `prioritizes`
- `plans`
- `tests`
- `supports`
- `synthesizes`
- `recommends`

## Prose Standard

All deliverables should read like polished strategy consulting work: direct, specific, active, and economical. Apply [prose-standard.md](references/prose-standard.md) while drafting, then run a final editing pass in Stage 8.
