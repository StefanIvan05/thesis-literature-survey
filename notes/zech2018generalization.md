# Zech et al., 2018, PLOS Medicine

- **BibTeX key:** `zech2018generalization`
- **Category:** Reliability (generalisation)
- **Link:** https://doi.org/10.1371/journal.pmed.1002683
- **PDF:** [`papers/zech2018generalization.pdf`](../papers/zech2018generalization.pdf)

## Summary
CNNs for pneumonia detection were trained on chest X-rays from three hospital systems (158,323 images). Performance often dropped on external hospitals, and CNNs could identify which hospital an image came from, so they partly learned hospital-specific confounders.

## Why it is relevant to my thesis
Concrete evidence that internal test accuracy overestimates real performance. It motivates testing on an external dataset or site if possible, and is a possible research gap (generalisation across centres).

## Where I will use it
Introduction (problem statement), Methodology (external validation), Discussion.

## Limitations / open questions
Chest X-ray only; the size of the effect may differ for MRI or ultrasound.
