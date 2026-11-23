# Isensee et al., 2021, Nature Methods

- **BibTeX key:** `isensee2021nnunet`
- **Category:** Architectures (segmentation)
- **Link:** https://doi.org/10.1038/s41592-020-01008-z
- **PDF:** [`papers/isensee2021nnunet.pdf`](../papers/isensee2021nnunet.pdf)

## Summary
nnU-Net automatically configures preprocessing, a 2D/3D U-Net architecture, training and post-processing for a new dataset, with no manual tuning. It outperformed most specialised methods across many public segmentation challenges.

## Why it is relevant to my thesis
A strong, reproducible baseline for segmentation: any contribution I propose should be compared against nnU-Net. It also shows that careful configuration often matters more than new architectures.

## Where I will use it
Related Work; strong baseline in experiments.

## Limitations / open questions
Computationally heavy, especially in 3D (needs a GPU with a lot of memory), which matters for feasibility.
