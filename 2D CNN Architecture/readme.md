# Brain Tumor Classification Using Deep Learning

## Overview
This project aims to classify brain tumors into four categories: **glioma**, **meningioma**, **pituitary**, and **no tumor** using 2D Convolutional Neural Networks (CNNs). We explored various CNN configurations, fine-tuned hyperparameters, and tested different activation functions, kernel sizes, regularization techniques, and epoch ranges to achieve the best performance. 

Our final goal was to achieve a high classification accuracy with reduced overfitting, improving upon the initial models by iterating and refining key components such as dropout rates, kernel size, activation functions, and regularization techniques.

## Models Tested and Results

We conducted several tests with different configurations and achieved the following results:

### **1. Kernel Size Variations**
- **Test 1a: Kernel Size = 3x3**
  - **Test Accuracy:** 83.58%
  - **Test Loss:** 0.4453
  - **AUC Score:** 0.9674
  
- **Test 1b: Kernel Size = 5x5**
  - **Test Accuracy:** 83.66%
  - **Test Loss:** 0.3926
  - **AUC Score:** 0.9662

- **Test 1c: Kernel Size = 7x7**
  - **Test Accuracy:** 83.66%
  - **Test Loss:** 0.4134
  - **AUC Score:** 0.9583

### **2. Number of Kernels in Layers**
- **Test 2a: Increased Number of Kernels (64, 128, 256)**
  - **Test Accuracy:** 81.07%
  - **Test Loss:** 0.4898
  - **AUC Score:** 0.9467

- **Test 2b: Constant Number of Kernels (64)**
  - **Test Accuracy:** 83.82%
  - **Test Loss:** 0.3932
  - **AUC Score:** 0.9622

### **3. Activation Functions**
- **Test 3a: Sigmoid Activation Function**
  - **Test Accuracy:** 88.30%
  - **Test Loss:** 0.2814
  - **AUC Score:** 0.9724

- **Test 3b: ReLU Activation Function**
  - **Test Accuracy:** 87.35%
  - **Test Loss:** 0.3649
  - **AUC Score:** 0.9708

- **Test 3c: tanH Activation Function**
  - **Test Accuracy:** 86.65%
  - **Test Loss:** 0.3343
  - **AUC Score:** 0.9724

### **4. Regularization Techniques**
- **Test 4a: L1 Regularization**
  - **Test Accuracy:** 62.22%
  - **Test Loss:** 2.6644
  - **AUC Score:** 81.69

- **Test 4b: L2 Regularization**
  - **Test Accuracy:** 76.75%
  - **Test Loss:** 0.7038

- **Test 4c: Elastic Net Regularization (L1 & L2, Sigmoid Function)**
  - **Test Accuracy:** 81.93%
  - **Test Loss:** 0.7984
  - **AUC Score:** 0.9479

### **5. Dropout Layers**
- **Test 5a: Dropout Rate (0.5)**
  - **Test Accuracy:** 73.21%
  - **Test Loss:** 0.9151

### **6. Final Results After Increasing Epochs to 50**
- **ReLU Activation:**
  - **Test Accuracy:** 91.59%
  - **Test Loss:** 0.2400
  
- **Sigmoid Activation:**
  - **Test Accuracy:** 93.79%
  - **Test Loss:** 0.1733
  
- **Sigmoid with ElasticNet Regularization:**
  - **Test Accuracy:** 87.04%
  - **Test Loss:** 0.6455
  
- **tanH Activation:**
  - **Test Accuracy:** 92.22%
  - **Test Loss:** 0.1881

---

## Conclusion

Our analysis demonstrates that increasing the number of epochs and experimenting with different activation functions and regularization methods improved the performance of the CNN model significantly. Specifically, the **Sigmoid** activation function provided the best test accuracy after 50 epochs, but **tanH** also performed strongly in comparison.

This project illustrates the importance of tuning hyperparameters and the impact of epoch count on model performance. Through this experimentation, we managed to refine our model to achieve over **93% test accuracy**.

## Future Work
- Explore additional regularization techniques to further mitigate overfitting.
- Extend the analysis to include other types of architectures such as deeper ResNet-based models.
- Implement more aggressive data augmentation techniques to see if they can further improve model performance.

