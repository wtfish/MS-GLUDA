# MS-GLUDA: Multi-Source Global-Local UDA for Brain Tumor Segmentation

**MS-GLUDA** is a hybrid framework designed for unsupervised domain adaptation (UDA) in brain tumor segmentation across heterogeneous MRI datasets. It combines global and local feature alignment strategies and incorporates YOLOv8-based tumor localization to enhance segmentation precision without requiring target domain labels.

## Key Features

- **Global Feature Alignment** via adversarial autoencoder to produce domain-invariant latent representations.
- **Local Feature Alignment** using a U-Net model to preserve spatial tumor structures at the pixel level.
- **YOLOv8 Tumor Detection** for locating tumor regions before segmentation, improving spatial focus.
- **Uncertainty-aware Entropy Loss** for confidence-calibrated predictions in ambiguous regions.
- **Multi-source Adaptation** using leave-one-out cross-domain evaluation on BraTS 2013, CBICA, TCIA01, and TMC datasets.
