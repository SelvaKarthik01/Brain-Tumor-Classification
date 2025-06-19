# Brain Tumor Detection and Classification Using Multiple Deep Learning Models
This repository contains code and resources for our research on brain tumor detection and classification using multiple deep learning architectures. Our project focuses on distinguishing four classes of brain tumors in MRI images using three distinct models: EfficientNetB4, Vision Transformer (ViT) + EfficientNetB4 Hybrid Model, and a Custom 2D CNN. Each model is evaluated for accuracy, computational efficiency, and overall performance in classifying MRI images into specific brain tumor categories.

Paper : https://doi.org/10.1007/s00521-025-11335-x

## Overview
Brain tumors, either malignant or benign, are challenging to diagnose due to the variety of tumor appearances on MRI scans. Early detection of brain tumors is critical to prevent severe cognitive damage and improve patient outcomes. This project aims to provide a robust solution for accurate and efficient tumor classification using MRI images through deep learning models.

## Key Features
High accuracy models for brain tumor classification.
Automated MRI-based diagnosis for four tumor classes: Glioma, Meningioma, Pituitary Tumors, and No Tumor.
Comparative analysis of three deep learning architectures.
Data augmentation for improved model generalization.
## Evaluation Metrics: Accuracy, F1-Score, AUC, Precision, and Recall.
## Models and Methodology
### 1. EfficientNetB4
EfficientNetB4 provides high accuracy with a simpler, parameter-efficient architecture. This model includes:

Data pre-processing: Resized images to 240x240 and normalized pixel values.
Data augmentation techniques, including rotation, shifts, zoom, and flips.
Model achieves 99.76% validation accuracy.
### 2. Vision Transformer (ViT) + EfficientNetB4 Hybrid Model
Our hybrid model combines the feature extraction power of Vision Transformers with EfficientNetB4’s efficiency. Key aspects:

Uniform image resizing to 224x224 pixels.
Brightness adjustments and further data augmentation.
Model achieves 99.6% validation accuracy and superior generalization.
### 3. Custom 2D CNN
A custom CNN architecture designed specifically for this task. Highlights include:

A series of convolutional, pooling, and dense layers for feature extraction.
Hyperparameter tuning and regularization for overfitting control.
Model achieves 97.25% validation accuracy.
Dataset
The dataset was sourced from Kaggle: https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset , consisting of 7023 images categorized as:

Glioma: 1321 training, 262 testing
Meningioma: 1399 training, 306 testing
Pituitary: 1457 training, 300 testing
No Tumor: 1591 training, 405 testing
Evaluation and Results
### EfficientNetB4: Accuracy - 99.76%
### Hybrid Model (ViT + EfficientNetB4): Accuracy - 99.6%
### Custom CNN: Accuracy - 97.25%
## Performance Metrics
Models were evaluated using:

Confusion Matrix
Precision, Recall, and F1-Score
AUC-ROC Curves
## Training Journey
Each model's training process included:

Early stopping to prevent overfitting.
Learning rate adjustments based on validation loss.
Checkpointing for saving the best-performing models.
## Future Work
We plan to explore:

Additional imaging modalities (CT, PET) alongside MRI for multi-modal classification.
Integration of GANs for handling data imbalance.
Application of explainable AI techniques (e.g., Grad-CAM, SHAP) for clinical transparency.
## Conclusion
This repository presents a comprehensive approach to brain tumor classification using deep learning models. Our findings demonstrate the effectiveness of EfficientNetB4 and ViT + EfficientNetB4 Hybrid models in achieving high accuracy while maintaining computational efficiency. This work offers promising insights into developing automated tools for clinical diagnostics in MRI-based brain tumor detection.

