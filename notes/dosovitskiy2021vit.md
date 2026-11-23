# Dosovitskiy et al., 2021, ICLR

- **BibTeX key:** `dosovitskiy2021vit`
- **Category:** Architectures (classification)
- **Link:** https://arxiv.org/abs/2010.11929
- **PDF:** [`papers/dosovitskiy2021vit.pdf`](../papers/dosovitskiy2021vit.pdf)

## Summary
Vision Transformer (ViT): splits an image into 16x16 patches and processes them with a standard Transformer. It matches or beats CNNs when pre-trained on very large datasets, but is weaker when trained on small data.

## Why it is relevant to my thesis
Represents the transformer family in a model comparison (CNN vs. ViT). The finding that ViT needs a lot of data is directly relevant, because medical datasets are small.

## Where I will use it
Background (architectures); possibly a research question: do transformers help on small medical datasets?

## Limitations / open questions
Needs large-scale pre-training; results on small medical datasets vary.
