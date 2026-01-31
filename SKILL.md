# Radiology: Artificial Intelligence Publication Skill

Create publication-ready manuscripts for Radiology: Artificial Intelligence with CLAIM 2024 compliance.

## Workflow

1. **Ask user for article type** (if not specified)
2. **Load article-specific guidance** from `article-types/[type].md`
3. **Apply formatting rules** from this file
4. **Generate CLAIM checklist** using `CLAIM.md` (AI manuscripts only)

## Article Types

| Type | File | CLAIM Required |
|------|------|----------------|
| Original Research | `article-types/original-research.md` | Yes |
| Technical Development | `article-types/technical-development.md` | Yes |
| AI in Brief | `article-types/ai-in-brief.md` | Yes |
| Review Article | `article-types/review.md` | No |
| Data Resources | `article-types/data-resources.md` | No |
| Letter to Editor | `article-types/letter.md` | No |

---

## Universal Formatting Rules

### Statistical Reporting
```
P values:     P < .05, P = .03 (no leading zero)
CIs:          95% CI: 0.82, 0.91 (always for primary outcomes)
Sample size:  (n = 271)
Percentages:  76.3% (71/93) (always include n/N)
AUC/ICC:      2 decimals (0.87, 0.85)
Bootstrap:    ≥2000 iterations for CIs
```

### CLAIM 2024 Terminology (Mandatory)
| Use | Not |
|-----|-----|
| reference standard | ground truth, gold standard |
| internal testing | validation (for evaluation) |
| external testing | external validation |
| tuning/optimization | validation (for hyperparameters) |

### Style Rules
- **Voice**: 75% active, 25% passive (passive in Methods acceptable)
- **Tense**: Present (facts, literature), Past (methods, results)
- **Person**: Third person; "we" for team actions (not in abstract)
- **Abbreviations**: Max 10; define as "term (ABBR)" on first use

### Prohibited
- Em dashes (use commas, parentheses, semicolons)
- Contractions
- Self-evaluative terms: novel, unique, groundbreaking, innovative, first-of-its-kind
- Vague qualifiers without data: very, quite, somewhat
- First person in abstract or results

### Required First Methods Paragraph
Every manuscript must begin Methods with:
1. Study design (retrospective/prospective)
2. IRB approval statement
3. Informed consent status
4. HIPAA compliance
5. Date range

**Template**: "This [retrospective/prospective] study was approved by the institutional review board of [institution], and [informed consent was obtained / the requirement for informed consent was waived]. The study was compliant with the Health Insurance Portability and Accountability Act."

---

## Code and Data Sharing (Mandatory for AI)

**Code**: Must deposit in public repository (GitHub, Zenodo, etc.)
- Include: training code, inference code, requirements.txt, README
- State repository URL in Methods with commit hash/version
- "Available upon request" is NOT acceptable

**Data Availability Statement** (title page):
- Public data: "[Dataset] is available at [URL]"
- Restricted: "Data cannot be shared due to [reason]. Requests may be directed to [contact]."

---

## Pre-submission Essentials

Before submitting, verify:
- [ ] CLAIM checklist completed (AI manuscripts)
- [ ] Summary statement ≤255 characters, no abbreviations
- [ ] Key points (up to 3) include data, no uncommon abbreviations
- [ ] All statistics have 95% CIs
- [ ] Code deposited with URL in manuscript
- [ ] IRB statement in first Methods paragraph
- [ ] Limitations addressed in Discussion
- [ ] No self-evaluative language
- [ ] Word count within limits

---

## Addressing Top Reviewer Critiques

| Critique | Prevention |
|----------|------------|
| Insufficient detail | Complete CLAIM checklist during writing |
| Missing external validation | Test externally OR explicitly acknowledge in limitations |
| Statistical concerns | CIs on all metrics; state comparison tests |
| Weak clinical relevance | Discuss clinical implications in Discussion |
| Reference standard issues | Document annotator qualifications, inter-rater reliability |
| No failure analysis | Include confusion matrix; analyze misclassifications |

---

## CLAIM Checklist

For AI manuscripts, see `CLAIM.md` for the complete 44-item checklist with auto-fill guidance.

**Critical items (most commonly missed)**:
- Item 12: De-identification methods (77% miss)
- Item 13: Missing data handling (68% miss)
- Item 18: Inter-rater variability (55% miss)
- Item 31: Explainability methods (60% miss)
- Item 37: Failure analysis (92% miss)
- Item 43: Code availability (66% miss)
