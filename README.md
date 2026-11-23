# Literature Survey: AI for Medical Condition Detection and Classification

Bachelor's thesis literature survey for **Methodology for writing the BSc Thesis**, West University of Timișoara (UVT), Computer Science (English).

**Student:** Ștefan Ivan · **Working title:** *Artificial Intelligence for Medical Condition Detection and Classification*

## Thesis direction
The thesis applies Machine Learning and Deep Learning to medical images (MRI, ultrasound, dermatoscopy) in order to detect and classify medical conditions. The plan is to:
- train and compare several models;
- evaluate them beyond accuracy (generalisation, calibration, explainability);
- where possible, contribute an improvement in accuracy or reliability.

A further option under consideration is to **combine images with clinical data** (multimodal AI).

The specific condition is not fixed yet. It will be chosen based on dataset availability and quality, and on what the literature leaves open. The current candidates are brain tumours (MRI), ovarian tumours (ultrasound), endometriosis (MRI) and skin lesions (dermatoscopy).

## Repository structure
```
references.bib   BibTeX entries for all sources (complete bibliographic data)
papers/          PDFs of the open-access sources
notes/           one note per source: summary, relevance to my thesis, where I will use it, limitations
```

## How the literature was collected
1. **Search sources:**
   - Google Scholar, PubMed and arXiv;
   - publisher pages (Nature Portfolio, PLOS, BMC, Elsevier, Springer, Wiley);
   - dataset repositories (Zenodo, TCIA).
2. **Search terms (combinations):**
   - "deep learning" + "medical image analysis" / "segmentation" / "classification";
   - "ovarian tumor ultrasound"; "endometriosis MRI dataset"; "pediatric brain tumor segmentation";
   - "multimodal fusion imaging EHR"; "generalization" / "calibration" / "bias" + "medical imaging".
3. **Inclusion criteria:**
   - peer-reviewed articles, or highly cited preprints from established groups;
   - directly relevant to one of four areas: (a) the state of the art, (b) model architectures I may use, (c) reliability and evaluation methodology, (d) the public datasets for the candidate conditions.
4. **Verification:** every bibliographic entry was checked against the arXiv, Crossref or Zenodo metadata APIs. Titles, authors, venue, volume, pages and DOI come from these records, not from memory.
5. **Copyright:** only open-access PDFs (arXiv preprints, or CC BY articles) are stored in this public repository. Sources that are not open access, or whose download was blocked, are referenced by DOI only.

## Sources (24)
| Source | Category | PDF in repo |
|---|---|---|
| [Litjens et al., 2017, Medical Image Analysis](notes/litjens2017survey.md) | Overview | yes |
| [Varoquaux & Cheplygina, 2022, npj Digital Medicine](notes/varoquaux2022failures.md) | Overview / methodology | yes |
| [Kelly et al., 2019, BMC Medicine](notes/kelly2019challenges.md) | Overview / clinical context | yes |
| [He et al., 2016, CVPR](notes/he2016resnet.md) | Architectures (classification) | yes |
| [Tan & Le, 2019, ICML](notes/tan2019efficientnet.md) | Architectures (classification) | yes |
| [Dosovitskiy et al., 2021, ICLR](notes/dosovitskiy2021vit.md) | Architectures (classification) | yes |
| [Ronneberger et al., 2015, MICCAI](notes/ronneberger2015unet.md) | Architectures (segmentation) | yes |
| [Isensee et al., 2021, Nature Methods](notes/isensee2021nnunet.md) | Architectures (segmentation) | yes |
| [Selvaraju et al., 2020, International Journal of Computer Vision](notes/selvaraju2020gradcam.md) | Explainability | yes |
| [Guo et al., 2017, ICML](notes/guo2017calibration.md) | Reliability (uncertainty) | yes |
| [Zech et al., 2018, PLOS Medicine](notes/zech2018generalization.md) | Reliability (generalisation) | yes |
| [Daneshjou et al., 2022, Science Advances](notes/daneshjou2022ddi.md) | Reliability (fairness) | link only |
| [Esteva et al., 2017, Nature](notes/esteva2017dermatologist.md) | Applications | link only |
| [Rajpurkar et al., 2017, arXiv](notes/rajpurkar2017chexnet.md) | Applications | yes |
| [Christiansen et al., 2021, Ultrasound in Obstetrics & Gynecology](notes/christiansen2021ovarian.md) | Applications (ovarian ultrasound) | link only |
| [Huang et al., 2020, npj Digital Medicine](notes/huang2020fusion.md) | Multimodal AI | yes |
| [Acosta et al., 2022, Nature Medicine](notes/acosta2022multimodal.md) | Multimodal AI | link only |
| [Tschandl et al., 2018, Scientific Data](notes/tschandl2018ham10000.md) | Dataset (dermatology) | yes |
| [Pacheco et al., 2020, Data in Brief](notes/pacheco2020padufes.md) | Dataset (dermatology, multimodal) | link only |
| [Bakas et al., 2018, arXiv](notes/bakas2018brats.md) | Dataset / benchmark (brain MRI) | yes |
| [Fathi Kazerooni et al., 2023, arXiv](notes/kazerooni2023bratspeds.md) | Dataset (pediatric brain MRI) | yes |
| [Zhao et al., 2022, arXiv](notes/zhao2022mmotu.md) | Dataset (ovarian ultrasound) | yes |
| [Liang et al., 2025, Scientific Data](notes/liang2025utendomri.md) | Dataset (endometriosis MRI) | yes |
| [Liang et al., 2025, Zenodo](notes/liang2025utendomri_data.md) | Dataset record | link only |

## Main findings so far
- **Architectures:**
  - CNN backbones (ResNet, EfficientNet) with ImageNet transfer learning remain the standard for classification.
  - Vision Transformers need more data.
  - For segmentation, U-Net and especially nnU-Net are the baselines to beat.
- **Data is the main bottleneck:** the quality, size, labels and representativeness of the dataset determine what is feasible (Litjens 2017; Varoquaux & Cheplygina 2022).
- **Reported accuracy often overestimates real performance:**
  - models degrade on other hospitals or populations (Zech 2018; Daneshjou 2022);
  - they are often over-confident (Guo 2017);
  - so reliability is a meaningful contribution direction, not only accuracy.
- **Multimodal fusion** of images and clinical data usually helps (Huang 2020), but public datasets that pair both are rare (PAD-UFES-20 is one exception).
- **Possible research gaps for the thesis:**
  1. generalisation and calibration of models for ovarian-ultrasound classification;
  2. adult-to-pediatric transfer for brain-tumour segmentation;
  3. segmentation of endometriomas with limited data;
  4. whether clinical metadata improves image-based classification.

## Next steps
- Select the condition and dataset with my supervisor.
- Extend the survey with the most recent (2023-2026) papers for the chosen condition.
- Define the research question and the evaluation protocol.
