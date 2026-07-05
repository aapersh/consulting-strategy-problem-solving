# Stage 8: Package the Story

This stage converts the approved answer and recommendation into final content for a deck, memo, report, or board paper. It prepares the message and structure. A downstream builder handles design and rendering. Apply strategy-consulting storyline discipline: the audience should understand the answer from the page titles or section headings alone.

## Choose the Output Track

Ask the user which format they want:

- **Slides**: concise, visual, one main message per page. Use [08-slide-content.md](08-slide-content.md).
- **Long-form**: memo, report, board paper, or narrative document. Use [08-long-form-content.md](08-long-form-content.md).

If the user is unsure, recommend slides for live discussion and long-form content for asynchronous review.

## Partner Input

Collect these choices:

1. Audience: roles, seniority, prior knowledge, likely concerns
2. Desired format: slides or long-form
3. Narrative pattern
4. Executive summary: include or exclude
5. Context section: include or exclude
6. Approximate length
7. Sensitive points to soften, sequence carefully, or move to appendix

## Narrative Patterns

| Pattern | Structure | Best fit |
|---|---|---|
| Answer-first | Recommendation -> reasons -> evidence -> action | Senior aligned audiences |
| Evidence-build | Observations -> pattern -> conclusion -> action | Skeptical audiences |
| Situation-change-response | Context -> disruption -> required response | Persuasion and urgency |
| Current-to-target | Current reality -> target state -> path | Transformations |
| Options evaluation | Options -> criteria -> decision -> next steps | Investment or board choices |
| Roadmap | Phases -> owners -> milestones -> outcomes | Implementation planning |

Use the pattern to shape the story. Avoid displaying framework labels as page titles unless the label is genuinely helpful to the user.

## Assembly Order

Use this order unless the user requests otherwise:

1. Title
2. Executive summary, if selected
3. Context and objectives, if selected
4. Core story pages or sections
5. Implementation and economics
6. Risks and decisions needed
7. Appendix, if selected

## Stage Gates

### Gate 1: Storyline

Present a page or section sequence with headlines and one-line purpose for each. Ask the user to approve structure before drafting final content.

### Gate 2: Independent Challenge Review

Launch the challenge review described in `SKILL.md`. Present proposed changes to the user and apply only approved changes.

### Gate 3: Content Draft

Draft the content using the selected track rules:

- Slides: read [08-slide-content.md](08-slide-content.md)
- Long-form: read [08-long-form-content.md](08-long-form-content.md)

### Gate 4: Final Content Approval

Save the approved content to the engagement folder:

- Slides: `08-slide-content.md`
- Long-form: `08-final-content.md`

Stop after approved content. Hand off to a builder skill if the user wants rendered slides or a formatted document.

## Frontmatter Template

```yaml
---
id: "08-final-content"
type: "final-content"
stage: 8
title: "Final Content"
status: draft
addresses: "01-question-framing.md#dq"
presents:
  - "07-recommendation-brief.md#rec-core"
  - "06-integrated-answer.md#answer"
narrative_pattern: "answer-first"
format: "slides"
page_count: 0
---
```

## Review Prompts

Ask the user:

- Does the storyline lead with the right message?
- Is the tone right for this audience?
- Which point needs more proof?
- Which point should move to appendix?
- What decision should the audience make after reading?

## Common Failure Modes

- Page titles name topics instead of arguments.
- The story follows the analysis sequence instead of the decision logic.
- Data appears before the point it supports.
- Sensitive issues are presented without context.
- Builder work starts before the content is approved.
