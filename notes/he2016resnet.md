# He et al., 2016, CVPR

- **BibTeX key:** `he2016resnet`
- **Category:** Architectures (classification)
- **Link:** https://doi.org/10.1109/CVPR.2016.90
- **PDF:** [`papers/he2016resnet.pdf`](../papers/he2016resnet.pdf)

## Summary
Introduces residual connections, which make very deep CNNs trainable. ResNet won ILSVRC 2015 classification (3.57% top-5 error with an ensemble).

## Why it is relevant to my thesis
ResNet-50 is the most common baseline backbone in medical image classification and is available pre-trained on ImageNet, so it is a natural first baseline for transfer learning.

## Where I will use it
Background chapter (CNN architectures); baseline model in experiments.

## Limitations / open questions
Designed for natural images; medical images differ (grey-scale, 3D, small lesions), so transfer is not guaranteed to be optimal.
