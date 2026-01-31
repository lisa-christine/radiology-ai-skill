# Technical Development

## Limits
| Element | Limit |
|---------|-------|
| Words | 2000 (Intro–Discussion) |
| Abstract | 250 (structured) |
| References | 25 |
| Figures | 6 |
| Tables | 2 |

**Required**: Summary statement (≤255 chars), CLAIM checklist

---

## Purpose
Describes new algorithms, software, or datasets. Emphasizes methodology over clinical validation. Appropriate for exploratory feasibility studies.

## Key Differences from Original Research
- Shorter Introduction and Discussion
- Focus on technical innovation
- Smaller sample sizes acceptable
- External validation encouraged but not required

---

## Structure

### Title
Emphasize technical innovation.
*Example*: "Self-Supervised Contrastive Learning for Chest Radiograph Classification: A Technical Development Study"

### Abstract (Structured)
Same format as Original Research but emphasize technical contribution.

### Introduction (1-2 paragraphs)
1. Technical gap and motivation
2. Purpose statement

### Materials and Methods
**First paragraph**: Design, IRB, consent, HIPAA, dates

**Core section** (most important): Detailed technical description
- Architecture with sufficient detail for reproduction
- Key innovations distinguished from prior work
- Implementation details (layers, parameters)

**Also include**: Data, evaluation methodology, software/hardware

### Results
- Technical performance metrics with CIs
- Ablation studies (if applicable)
- Computational efficiency (training time, inference time, model size)
- Failure cases

### Discussion (1-2 paragraphs)
1. Technical contributions summarized
2. Limitations and future work

---

## Code Sharing (Critical)

Technical Development has heightened reproducibility expectations:
- Complete source code
- Detailed README
- Requirements with versions
- Example data or synthetic test cases
- Pretrained weights (if shareable)
- Configuration files
