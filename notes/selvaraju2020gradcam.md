# Selvaraju et al., 2020, International Journal of Computer Vision

- **BibTeX key:** `selvaraju2020gradcam`
- **Category:** Explainability
- **Link:** https://doi.org/10.1007/s11263-019-01228-7
- **PDF:** [`papers/selvaraju2020gradcam.pdf`](../papers/selvaraju2020gradcam.pdf)

## Summary
Grad-CAM produces heatmaps of the image regions that most influenced a CNN's decision, using the gradients flowing into the last convolutional layer. Works with any CNN without retraining.

## Why it is relevant to my thesis
Lets me check whether a model looks at the lesion or at artefacts such as rulers, text or scanner markings. This makes the results easier for a doctor or examiner to interpret.

## Where I will use it
Methods (explainability analysis) and Results (qualitative examples, failure cases).

## Limitations / open questions
Heatmaps are coarse and can be misleading; they explain where the model looks, not why.
