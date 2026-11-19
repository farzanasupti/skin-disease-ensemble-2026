# Ensemble Deep Learning for Skin Disease Classification

This repo has the notebook and manuscript for our paper *Ensemble Deep Learning for Automated Skin Disease Classification: A Multi-Scale Patient-Level Validation Framework with Uncertainty Quantification* (Supti et al., 2026). The paper went up as a ResearchGate preprint in July 2026, and it is currently under review at *Scientific Reports*.

## What's here

- `manuscript/manuscript.pdf`: the submitted manuscript
- `notebooks/skin_disease_ensemble.ipynb`: the Kaggle notebook (TensorFlow/Keras), saved with its outputs

We trained a small custom CNN and seven ImageNet-pretrained models (VGG16, ResNet50, MobileNetV2, EfficientNetB0, DenseNet121, InceptionV3, Xception) to classify five skin conditions: acne, hyperpigmentation, nail psoriasis, SJS-TEN and vitiligo. We scored them per image, and also per patient by combining each patient's images with majority vote, average probability or maximum probability.

## About the numbers

The tables in the manuscript come from a separate run of these experiments, which the team ran on another machine. The outputs saved in this notebook are from a Kaggle run, so they won't match the tables exactly.

## Follow-up work

I later took a closer look at the public Mendeley version of this dataset and found that most of its images are augmented copies of a few hundred original photos. That work, with grouped cross-validation and testing on the original photos only, is in a separate repo: [skin-disease-classification](https://github.com/farzanasupti/skin-disease-classification).
