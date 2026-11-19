# Ensemble Deep Learning for Automated Skin Disease Classification

Code and manuscript for *Ensemble Deep Learning for Automated Skin Disease Classification: A Multi-Scale Patient-Level Validation Framework with Uncertainty Quantification* (Supti et al., 2026). The paper is a ResearchGate preprint from July 2026 and is under review at *Scientific Reports*.

## Contents

| Path | What it is |
|---|---|
| `manuscript/manuscript.pdf` | The manuscript as submitted |
| `notebooks/skin_disease_ensemble.ipynb` | The Kaggle notebook (TensorFlow/Keras), with its saved outputs |

## What the study compares

- A custom CNN and seven ImageNet-pretrained backbones: VGG16, ResNet50, MobileNetV2, EfficientNetB0, DenseNet121, InceptionV3 and Xception.
- Five-class skin-condition classification (acne, hyperpigmentation, nail psoriasis, SJS-TEN, vitiligo).
- Image-level evaluation, plus patient-level aggregation by majority vote, average probability and maximum probability.

## Note on results

The numbers in the manuscript's tables were collected from a separate run of the experiments. The outputs saved in this notebook come from a different run, so they do not match those tables.

## Related work

A separate study on the public Mendeley skin-disease dataset, with duplicate-aware grouped cross-validation: [farzanasupti/skin-disease-classification](https://github.com/farzanasupti/skin-disease-classification).
