# Original Research

## Limits
| Element | Limit |
|---------|-------|
| Words | 3000 (Intro–Discussion) |
| Abstract | 250 (structured) |
| References | 35 |
| Figures | 6 |
| Tables | 4 |

**Required**: Summary statement (≤255 chars), Key Points (≤3), CLAIM checklist

---

## Structure

### Title
Include AI method + task + modality.
*Example*: "Deep Learning Detection of Pulmonary Nodules on Chest Radiographs: A Multicenter Validation Study"

### Abstract (Structured)
```
Purpose: To [develop/evaluate] [method] for [task] on [modality].

Materials and Methods: This [retrospective/prospective] study included [n] patients (mean age, X years ± SD; n male) from [source] between [dates]. [Methods 1-2 sentences]. [Statistics]; P < .05 indicated significance.

Results: [Primary metric] was [value] (95% CI: X, Y). [Secondary findings with CIs].

Conclusion: [Method] [demonstrated] [finding], [implication].
```

### Introduction (2-4 paragraphs)
1. Clinical context with prevalence [1-3]
2. Literature review [4-8]
3. Gap identification
4. Purpose statement (final paragraph)

### Materials and Methods
**First paragraph**: Design, IRB, consent, HIPAA, dates

**Subsections**:
- Study Population (inclusion/exclusion with counts, flow diagram reference)
- Image Acquisition (manufacturer, parameters)
- Reference Standard (specific criteria, annotators, inter-rater reliability)
- Model Architecture (or cite + modifications)
- Training (loss, optimizer, LR, batch, epochs, stopping, hardware)
- Statistical Analysis (software, CIs, tests, threshold)

### Results
**First paragraph**: Demographics (n, age, sex), Table 1, Figure 1 references

**Subsequent**: Primary metric with CI → secondary metrics → subgroups → external testing (if any) → failure analysis

### Discussion
1. Summary of findings
2. Literature comparison (multiple paragraphs)
3. **Limitations** (second-to-last paragraph, ≥3 limitations)
4. Conclusions (final paragraph)

---

## Required Elements

### Summary Statement
≤255 characters, no abbreviations, includes primary metric.

*Template*: "[Method] achieved [metric] of [value] for [task], [implication]."

### Key Points (up to 3)
Each includes data, no uncommon abbreviations.

*Example*:
- Deep learning nodule detection achieved sensitivity of 91% (95% CI: 87%, 94%).
- Performance maintained across nodule sizes 6-30 mm (P = .42).
- Workflow integration reduced interpretation time by 23%.

### Figure 1: Study Flow Diagram
Required. Show: initial population → exclusions with counts → final partitions.

### External Validation
Strongly encouraged. If absent, explicitly acknowledge in limitations with plans for future validation.
