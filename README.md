# Explainable-MCF7-Cell-Segmentation-unet
Deep learning-based segmentation of MCF-7 breast cancer cells using U-Net with Grad-CAM explainability for accurate and interpretable biomedical image analysis.
# Deep Learning-Based Segmentation of MCF-7 Breast Cancer Cells with Explainable AI

## Overview

This project presents a deep learning framework for automatic segmentation of **MCF-7 breast cancer cells** from microscopy images using the **U-Net architecture**. In addition to accurate segmentation, the project incorporates **Gradient-weighted Class Activation Mapping (Grad-CAM)** to provide visual explanations of the model's predictions, improving interpretability for biomedical applications.

The proposed framework achieves high segmentation accuracy while enabling researchers to understand which image regions influence the model's decisions.

---

## Features

- Automatic segmentation of MCF-7 breast cancer cells
- U-Net implementation using Segmentation Models PyTorch
- Binary cell mask prediction
- Explainable AI using Grad-CAM
- Early stopping and model checkpointing
- Performance evaluation using:
  - Accuracy
  - Precision
  - Recall
  - Dice Coefficient
  - Intersection over Union (IoU)
- Visualization of:
  - Training & validation loss
  - Dice and IoU curves
  - Predicted masks
  - Grad-CAM heatmaps

---

## Dataset

**Dataset:** MCF-7 Breast Cancer Cell Dataset

Dataset Structure:

```
MCF7/
│
├── train/
│   ├── input/
│   └── output/
│
└── test/
    ├── input/
    └── output/
```

Ground truth masks are provided for supervised segmentation.

---

## Methodology

1. Data preprocessing
2. Image normalization
3. Binary mask generation
4. U-Net model training
5. Early stopping & checkpoint saving
6. Performance evaluation
7. Grad-CAM explainability

---

## Model

- Architecture: U-Net
- Framework: Segmentation Models PyTorch
- Input Channels: 1 (Grayscale)
- Output Classes: 1 (Binary Segmentation)

---

## Performance

| Metric | Score |
|---------|-------|
| Accuracy | **93.50%** |
| Precision | **88.30%** |
| Recall | **95.80%** |
| Dice Score | **91.84%** |
| IoU | **84.99%** |

---

## Explainable AI

Grad-CAM was integrated to visualize the regions responsible for segmentation decisions.

The visualizations demonstrate that the model focuses primarily on biologically relevant cellular regions, improving transparency and interpretability.

---

## Technologies Used

- Python
- PyTorch
- Segmentation Models PyTorch
- TorchVision
- NumPy
- Matplotlib
- OpenCV
- PyTorch Grad-CAM
- Google Colab

---

## Repository Structure

```
├── dataset/
├── notebooks/
├── models/
│   └── best_unet.pth
├── results/
│   ├── predictions/
│   ├── gradcam/
│   └── plots/
├── src/
│   ├── dataset.py
│   ├── train.py
│   ├── evaluate.py
│   └── gradcam.py
├── requirements.txt
└── README.md
```

---

## Results

The proposed framework achieved robust segmentation performance while maintaining high interpretability through Grad-CAM visualizations.

---

## Future Work

- Attention U-Net
- Multi-class cell segmentation
- Boundary-aware loss functions
- Transformer-based segmentation models
- Quantitative Explainable AI metrics

---

## References

1. Ronneberger et al., U-Net: Convolutional Networks for Biomedical Image Segmentation (MICCAI 2015)

2. Selvaraju et al., Grad-CAM: Visual Explanations from Deep Networks (ICCV 2017)

3. LIVECell: A Large-Scale Dataset for Label-Free Live Cell Segmentation (Nature Methods)

---

## Author

**Vansika Vimal**

Biomedical Engineering

PSG College of Technology
