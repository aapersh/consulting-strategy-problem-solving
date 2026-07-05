# Stage 5: Run the Analyses

This stage tests the logic map with evidence. Each analysis should produce a finding, an implication, and a confidence level. Keep the strategy-consulting standard: analysis earns its place only when it sharpens the decision or changes confidence in the recommendation.

## Partner Input

Before each analysis or batch, ask:

1. Are these assumptions reasonable?
2. Do the low, base, and high cases fit your experience?
3. Is there better internal data than the source or proxy proposed?
4. Does the method match how stakeholders will evaluate the answer?
5. Should any sensitivity or segment cut be added?

Pause when assumptions are material. Do not bury judgment calls inside the model.

## Deliverables

Produce:

- `05-analysis-findings.md`: narrative findings and implications
- Analysis workbook when calculations, models, or tabular data are used

Workbook tabs:

- Summary of findings
- One tab per major analysis
- Assumptions and sources
- Sensitivities, where relevant

## Per-Analysis Flow

For each analysis:

1. Restate the question.
2. Confirm assumptions or data.
3. Run the analysis.
4. State the finding.
5. Apply the decision relevance test.
6. Mark the hypothesis status.
7. Record confidence and limitations.

## Data Standards

Use facts with discipline:

- Record source, year, and access date when available.
- Label internal estimates, management estimates, public benchmarks, and model outputs.
- Flag stale data in fast-moving markets.
- Cross-check figures that appear together.
- Use ranges when precision would mislead.
- Keep numbers that support the argument; move extra detail to appendix.

If data is missing, offer a proxy with rationale and sensitivity range. Ask the user to approve before using it.

## Analysis Patterns

| Pattern | Best use | Output |
|---|---|---|
| Driver tree | Quantify causes of a metric shift | Contribution table |
| Cohort analysis | Compare customer or product groups | Segment chart |
| Benchmark | Size gaps against peers or standards | Gap table |
| Sensitivity model | Test economics under uncertainty | Low, base, high cases |
| Scenario model | Compare strategic futures | Scenario table |
| Process analysis | Diagnose operating friction | Bottleneck map |
| Interview synthesis | Capture stakeholder reality | Theme and evidence table |

## Findings Template

```markdown
---
id: "05-analysis-findings"
type: "analysis-findings"
stage: 5
title: "Analysis Findings"
status: draft
addresses: "01-question-framing.md#dq"
findings:
  - anchor: "05-analysis-findings.md#f-[slug]"
    label: "[Finding]"
    tests: "04-analysis-plan.md#ax-ws1-a1"
    branch: "02-logic-map.md#br-[slug]"
    confidence: medium
hypothesis_status:
  - hypothesis: "02-logic-map.md#bh-[slug]"
    status: supported
    evidence: "05-analysis-findings.md#f-[slug]"
---

# Analysis Findings

## Findings at a Glance
| # | Finding | Decision implication | Confidence | Source base |
|---|---|---|---|---|
| 1 | [Finding] | [Implication] | High/Medium/Low | [Sources] |

## Detailed Findings

### Analysis [ID]: [Name]
**Question**: [Question answered]

**Finding**: [What the evidence shows]

**Evidence**: [Data, model result, or qualitative support]

**Decision implication**: [How this changes the answer]

**Hypothesis status**: Supported / Partly supported / Challenged

**Confidence**: [Level and reason]

**Limitations**: [What remains uncertain]

## Emerging Themes
[Patterns across analyses.]

## Open Questions
[Questions that should be resolved before final recommendation.]

## Assumptions and Sources
[Material assumptions and source list.]
```

## Review Gate

Review findings with the user after each major batch. Ask:

- Which findings match or challenge your experience?
- Which assumptions need revision?
- Which finding changes the direction of the work?
- Do any results require deeper analysis?

Do not move to Stage 6 until the main findings are reviewed and approved.

## Common Failure Modes

- A chart is produced without a decision implication.
- The analysis confirms a preferred view while contradictory evidence is ignored.
- Estimates appear as facts.
- Confidence is overstated.
- Source tracking starts too late.
