# Brain Tumor Classification using Deep Learning

This repository contains the code and resources for classifying brain tumors using deep learning models. The project aims to classify brain tumors into four categories: Glioma, Pituitary, Meningioma, and No Tumor. The work includes the development and training of advanced models, including EfficientNetB4 and a hybrid EfficientNetB4 + Vision Transformer (ViT), achieving high accuracy and robust performance.

## Overview

Brain tumors are a serious health condition requiring precise and accurate diagnosis. This project leverages deep learning techniques to build and train models that can classify brain tumor types using MRI images. The repository includes the following models:

### EfficientNetB4 Model
- **Test Accuracy:** 99.76%
- Utilizes the EfficientNetB4 architecture for robust feature extraction and classification.
- Trained on a comprehensive dataset of MRI images with extensive preprocessing and augmentation.

### Hybrid EfficientNetB4 + Vision Transformer (ViT) Model
- **Test Accuracy:** 99.14%
- Combines the strengths of EfficientNetB4 and Vision Transformer for improved accuracy and generalization.
- Incorporates innovative hybrid architecture to enhance feature learning and classification performance.

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

**Source:** [Kaggle - Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)

All images are preprocessed to 240x240 dimensions. The dataset is divided into training and testing sets, ensuring a balanced distribution of classes.

## Usage

### Prerequisites
- Python 3.x
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib

## Ongoing Work
Currently, we are developing a custom 2D CNN model from scratch. This novel model incorporates customized layers and architecture designed to enhance classification performance without relying on pre-built models. The goal is to contribute a unique approach to brain tumor classification and further improve overall model efficacy.

## Conclusion

This project demonstrates the application of advanced deep learning techniques to classify brain tumors with high accuracy using MRI images. The EfficientNetB4 model achieved the highest test accuracy, showcasing its robustness for this classification task. Our ongoing efforts include developing a custom 2D CNN model to offer a unique approach and potentially enhance classification performance further. We hope this work serves as a solid foundation for future research and advancements in brain tumor detection and classification.
