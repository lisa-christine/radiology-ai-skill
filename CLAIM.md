# CLAIM 2024 Checklist (44 Items)

Required for: Original Research, Technical Development, AI in Brief

Mark each: **Yes** (page/line), **No** (explain), **NA** (justify)

---

## Title & Abstract
| # | Item | Look for |
|---|------|----------|
| 1 | AI method in title/abstract | "deep learning", "neural network", architecture names |
| 2 | Structured summary with partitions | Design, n, modality, train/val/test sizes, metrics+CI |

## Introduction
| # | Item | Look for |
|---|------|----------|
| 3 | Scientific/clinical background | Context with citations |
| 4 | Objectives/hypotheses | Purpose statement; pre-registration if applicable |

## Methods: Study Design
| # | Item | Look for |
|---|------|----------|
| 5 | Prospective/retrospective | Explicit statement |
| 6 | AI task and clinical role | Classification/segmentation/etc.; replacement/triage/add-on |

## Methods: Data
| # | Item | Look for |
|---|------|----------|
| 7 | Data source | Institution, how matches intended use |
| 8 | Eligibility criteria | Inclusion/exclusion with counts |
| 9 | Data partitioning | Split method, ratios, patient vs image level |
| 10 | Preprocessing | Cropping, normalization, augmentation |
| 11 | De-identification | HIPAA method, DICOM handling |
| 12 | Missing data | Handling method |
| 13 | Image acquisition | Manufacturer, parameters, resolution |

## Methods: Reference Standard
| # | Item | Look for |
|---|------|----------|
| 14 | Definition | Specific criteria (not just "radiologist labels") |
| 15 | Rationale | Why appropriate |
| 16 | Annotation tools | Software used |
| 17 | Annotators | Number, qualifications, training, inter-rater κ/ICC |

## Methods: Model
| # | Item | Look for |
|---|------|----------|
| 18 | Architecture | Name/citation, modifications |
| 19 | Pre-trained source | ImageNet/RadImageNet, fine-tuning approach |
| 20 | Inputs/outputs | Image size, channels, output type |
| 21 | Feature extraction | If hand-crafted features used |
| 22 | Feature selection | Method and rationale |
| 23 | Class imbalance | Oversampling, weighting, etc. |
| 24 | Uncertainty | Quantification method if used |
| 25 | Training | Loss, optimizer, LR, batch, epochs, stopping |
| 26 | Hyperparameter tuning | Search method, final values |
| 27 | Software | Framework versions |

## Methods: Evaluation
| # | Item | Look for |
|---|------|----------|
| 28 | Metrics | List with definitions |
| 29 | Statistical methods | Software, CI method, significance threshold |
| 30 | Reader study | Selection, training, blinding |

## Results
| # | Item | Look for |
|---|------|----------|
| 31 | Flow diagram | Figure showing selection through analysis |
| 32 | Demographics | Age, sex per partition |
| 33 | Performance summary | Metrics on all partitions with CIs |
| 34 | Failures/errors | Cases that failed, types |
| 35 | Test performance | Final metrics with 95% CIs |
| 36 | Reader comparison | Statistical comparison if applicable |

## Discussion
| # | Item | Look for |
|---|------|----------|
| 37 | Limitations | Bias, reference standard, generalizability |
| 38 | Clinical applicability | Translation implications |
| 39 | Safety/bias | Demographic subgroups, failure modes |

## Other
| # | Item | Look for |
|---|------|----------|
| 40 | Registration | Registry number |
| 41 | Conflicts | Disclosures |
| 42 | AI disclosure | AI tools in writing |
| 43 | Code/data availability | Repository URL, access conditions |
| 44 | Funding | Sources and role |

---

## Auto-fill Extraction Patterns

When generating checklist from manuscript:

**Item 1**: Search title + abstract for: deep learning, machine learning, neural network, CNN, transformer, AI, algorithm
**Item 5**: First Methods paragraph for: retrospective, prospective
**Item 9**: Methods for: training, validation, test, split, partition + percentages or ratios
**Item 11**: Methods for: de-identified, anonymized, HIPAA, Safe Harbor
**Item 14**: Reference standard section length >50 words with specific criteria
**Item 17**: Pattern: `\d+ (radiologist|reader|annotator)` + κ/kappa/ICC
**Item 25**: All of: loss, optimizer, learning rate, batch, epoch, stopping
**Item 31**: "Figure 1" near flow/selection/STARD
**Item 35**: Metric + CI pattern: `(AUC|sensitivity|accuracy).*\d+.*CI`
**Item 43**: URL pattern: github|gitlab|zenodo|bitbucket

---

## Critical Deficiencies (Address These First)

| Item | Issue | Compliance |
|------|-------|------------|
| 37 | No failure analysis | 8% |
| 43 | Code not shared | 34% |
| 11 | De-identification undocumented | 23% |
| 12 | Missing data not addressed | 32% |
| 17 | No inter-rater reliability | 45% |
| 31 | No explainability | 40% |
