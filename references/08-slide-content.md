# Stage 8: Slide Content Rules

Use this guide after the storyline and challenge review are approved. The output is a slide content specification that a builder skill can render. The slide standard should feel like structured strategy-consulting work: answer-first titles, tight evidence, and no filler between the insight and the implication.

## Core Rules

- One main message per slide.
- Titles are complete sentences that state the point.
- Body content is structured as bullets, tables, points, or labeled elements.
- Use numbers to support the message.
- Include source lines on slides with quantitative claims.
- Keep visual styling out of the content spec.

## Slide Roles

| Role | Use |
|---|---|
| cover | Title and context |
| executive-summary | Full argument in three to five bullets |
| context | Why the work exists |
| argument | One point with evidence |
| comparison | Options, trade-offs, criteria |
| roadmap | Phases, owners, milestones |
| framework | Operating model, pillars, logic structure |
| metrics | Focused quantitative dashboard |
| appendix | Detail, method, backup |
| closing | Decisions and next steps |

## Title Standard

A slide title should let the reader understand the message before reading the body.

Weak:

- "Customer Segments"
- "Pricing Analysis"
- "Implementation Plan"

Stronger:

- "Enterprise expansion should lead the growth plan because it has the strongest retention economics"
- "Discount leakage is concentrated in renewal accounts with weak approval discipline"
- "The first 90 days should lock decisions, owners, and measurement"

## Body Content Standards

### Argument Slides

- Three to five bullets
- One line per bullet where possible
- Parallel structure
- Strongest evidence first

### Comparison Slides

- Use a table or point pairs
- Keep cell text short
- Identify the recommended option clearly in words
- Include criteria that matter to the decision

### Roadmap Slides

- Show phase, timing, owner, and major actions
- Limit each phase to two or three actions
- Include dependencies only when material

### Framework Slides

- Use short labels
- Group related elements
- Number elements when later slides unpack them

### Metrics Slides

- Use a few metrics with direct decision relevance
- Add context, benchmark, or trend where needed
- Remove metrics that do not change the point

## Content Specification Format

Save slide content like this:

```markdown
# Slide Content Specification
<!-- Engagement: {client}/{project} -->
<!-- Builder should use this content verbatim -->

---

## Slide 1: Cover
- **Role**: cover
- **Layout**: hero
- **Eyebrow**: STRATEGIC REVIEW
- **Hero Title**:
  - "Pricing Discipline"
  - "for Enterprise Renewals"
- **Body Text**: Prepared for leadership discussion | May 2026

---

## Slide 2: Executive Summary
- **Role**: executive-summary
- **Layout**: full-width-stack
- **Eyebrow**: EXECUTIVE SUMMARY
- **Title**: Renewal margin can recover if discount authority moves closer to value evidence
- **Body Text** (bullets):
  - Concentrate approval on high-risk renewal deals above 15% discount
  - Equip account teams with value proof before negotiation begins
  - Pilot the new governance in enterprise software and financial services
- **Callout Bar**: Target 4 to 6 margin points recovered within two renewal cycles
- **Source**: Internal renewal analysis; leadership interviews

---

## Slide 3: Discount Leakage
- **Role**: argument
- **Layout**: multi-col (3)
- **Eyebrow**: FINDING
- **Title**: Discount leakage is concentrated enough to address through targeted governance
- **Point 1**: Segment concentration: two verticals drive most leakage
- **Point 2**: Approval gap: high discounts often bypass value review
- **Point 3**: Timing issue: concessions occur late in renewal cycles
- **Source**: Renewal cohort analysis, FY2025
```

## Field Rules

| Field | Rule |
|---|---|
| Role | Use one of the listed slide roles |
| Layout | Use a simple hint such as `hero`, `split`, `multi-col (3)`, `full-width-stack`, `metric-row (3)`, or `roadmap` |
| Eyebrow | Short uppercase label |
| Title | Complete sentence with the slide message |
| Body Text | Plain text or bullets |
| Point N | Numbered content blocks |
| Callout Bar | One takeaway sentence |
| Source | Required when numbers appear |

## Distillation Process

1. Start with the approved storyline.
2. Map each slide to source material from Stages 6 and 7.
3. Decide the slide role.
4. Draft the title as the point.
5. Add only the content needed to prove or act on the point.
6. Move detail to appendix.
7. Check that the headline sequence tells the story by itself.

## Source Lines

Use:

```text
Source: [citation]; [citation]
```

Do not use superscript footnotes in slide content specs.

## Common Failure Modes

- A slide contains multiple competing messages.
- Bullets become full paragraphs.
- The title is a topic label.
- Visual instructions appear in the content spec.
- A number appears without source context.
- Appendix material stays in the main story.
