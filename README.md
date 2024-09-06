# Brain Tumor Classification Using Deep Learning

This repository contains the code and resources for classifying brain tumors into four categories: Glioma, Pituitary Tumors, Meningioma, and No Tumor. The project employs various deep learning models to achieve high accuracy and robust performance.

## Overview

The project includes the following models and their results:

### 1. EfficientNetB4 Model
- **Test Accuracy:** 99.76%
- **Test Loss:** 0.1313
- Utilizes the EfficientNetB4 architecture for feature extraction and classification.

### 2. Hybrid EfficientNetB4 + Vision Transformer (ViT) Model
- **Test Accuracy:** 99.14%
- **Test Loss:** 0.1809
- Combines EfficientNetB4 and Vision Transformer for improved accuracy and generalization.

### 3. Custom 2D CNN Model
The custom 2D CNN model was developed from scratch, achieving the following results after tuning:

#### Initial Results (30 Epochs)
- **Kernel Size 3x3, No Dropout, ReLU Activation:**
  - **AUC Score:** 0.9674
  - **Test Accuracy:** 0.8358
  - **Test Loss:** 0.4453

- **Kernel Size 5x5:**
  - **AUC Score:** 0.9662
  - **Test Accuracy:** 0.8366
  - **Test Loss:** 0.3926

- **Activation Function Sigmoid:**
  - **Test Accuracy:** 0.8830
  - **Test Loss:** 0.2814

#### Results with Extended Training (50 Epochs)
- **Activation Function ReLU:**
  - **Test Accuracy:** 0.9159
  - **Test Loss:** 0.2400

- **Activation Function Sigmoid:**
  - **Test Accuracy:** 0.9379
  - **Test Loss:** 0.1733

- **Activation Function Sigmoid with Regularization:**
  - **Test Accuracy:** 0.8704
  - **Test Loss:** 0.6455

## Features
- **Data Preprocessing and Augmentation:** Scripts for loading, preprocessing, and augmenting MRI images.
- **Model Definition and Training:** Code to define, train, and evaluate EfficientNetB4, the hybrid model, and the custom CNN model.
- **Performance Evaluation:** Tools for assessing model accuracy and loss, including AUC scores and visualizations.
- **Research Insights:** Detailed analysis and insights from training and model performance.

## Dataset
- **Source:** [Kaggle - Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)
- **Description:** 6500 brain MRI images categorized into Glioma, Pituitary, Meningioma, and No Tumor. Images are preprocessed to 240x240 dimensions and divided into training and testing sets.

## Usage
### Prerequisites
- Python 3.x
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
## Conclusion

This project showcases the application of advanced deep learning techniques for brain tumor classification using MRI images. The combination of EfficientNetB4, Vision Transformers, and custom 2D CNN models demonstrates the potential for high-accuracy medical imaging solutions. Despite some challenges, the models achieved significant performance metrics, highlighting their robustness and effectiveness. Our ongoing efforts aim to refine these models further, contributing valuable insights and advancements in medical image analysis. We hope this work serves as a solid foundation for future research and development in brain tumor detection and classification.

