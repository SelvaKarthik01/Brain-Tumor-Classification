# Brain Tumor Classification using Deep Learning

This repository contains the code and resources for the classification of brain tumors using deep learning models. The project aims to classify brain tumors into four categories: glioma, pituitary, meningioma, and no tumor. The work includes the development and training of two advanced models, EfficientNetB4 and a hybrid EfficientNetB4 + Vision Transformer (ViT), achieving high accuracy and robust performance.

## Overview

Brain tumors are a serious health condition requiring precise and accurate diagnosis. This project leverages deep learning techniques to build and train models that can classify brain tumor types using MRI images. The repository includes the following models:

1. **EfficientNetB4 Model**
   - Achieved a test accuracy of 99.76%
   - Utilizes the EfficientNetB4 architecture for robust feature extraction and classification
   - Trained on a comprehensive dataset of MRI images with extensive preprocessing and augmentation

2. **Hybrid EfficientNetB4 + Vision Transformer (ViT) Model**
   - Achieved a test accuracy of 99.14%
   - Combines the strengths of EfficientNetB4 and Vision Transformer for improved accuracy and generalization
   - Incorporates innovative hybrid architecture to enhance feature learning and classification performance

## Features

- **Data Preprocessing and Augmentation:** Code for loading, preprocessing, and augmenting the MRI images to enhance model training.
- **Model Definition and Training:** Scripts to define, train, and evaluate the EfficientNetB4 and hybrid models.
- **Performance Evaluation:** Metrics and visualization tools to assess the accuracy and performance of the models.
- **Research Insights:** Detailed analysis and insights derived from the training process and model performance.

## Dataset

The dataset used for training and testing the models consists of 6500 brain MRI images, categorized into four classes:
- Glioma
- Pituitary
- Meningioma
- No Tumor

- Source : Kaggle - https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset

All images are preprocessed to 240x240 dimensions. The dataset is divided into training and testing sets, ensuring a balanced distribution of classes.

## Usage

### Prerequisites

- Python 3.x
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
