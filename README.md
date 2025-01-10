# Artificial Neural Networks and Deep Learning

This repo contains the code and the reports of two challenges carried on during "Artificial Neural Networks and Deep Learning" course.

## 🩸 Challenge 1: Blood Cell Image Classification 🧬

### 📋 Project Overview

This project focuses on developing a deep learning model to classify blood cell images into 8 distinct classes, by leveraging advanced techniques such as transfer learning, data augmentation, and regularization.

### 📂 Dataset

The dataset contains **13,759 images** of size **96x96 pixels** in RGB format.

### 🛠️ Methodology

- **Data Preprocessing**: Removed duplicates and outliers, balanced classes using weighting and augmentation.
- **Model Development**: Started with a custom CNN, then moved to transfer learning with **MobileNetV3** and **ConvNeXt**.
- **Regularization**: Applied early stopping, dropout, and L1-L2 regularization to prevent overfitting.
- **Optimization**: Used the **Lion optimizer** for faster convergence.

### 📊 Results

- **Custom CNN**: 35.4% accuracy on Codabench.
- **MobileNetV3Large**: 65% accuracy on Codabench.
- **ConvNeXt**: 77% accuracy on Codabench.

✅ Score: 5.5/5.5

## 🪐 Martian Terrain Semantic Segmentation 🛸

### 📋 Project Overview

This project focuses on developing a deep learning model for semantic segmentation of Martian terrain images. The goal is to classify each pixel into one of five categories: **Background (0)**, **Soil (1)**, **Bedrock (2)**, **Sand (3)**, and **Big Rock (4)**.

### 📂 Dataset

The dataset contains **2,615 images** of size **64x128 pixels** in grayscale.

### 🛠️ Methodology

- **Model**: U-Net with **Squeeze and Excitation** blocks.
- **Data Augmentation**: Applied **CutMix** and **horizontal flips**.
- **Class Imbalance**: Addressed using **weighted loss** and **targeted augmentation** for class 4.
- **Loss Function**: Excluded background (class 0) to focus on relevant classes.

### 📊 Results

The final model achieved a **mean IoU of 73.22%** on the test set.

| **Model**                          | **Mean IoU (Test)** |
|------------------------------------|---------------------|
| U-Net 1                            | 36.09%              |
| U-Net 2 (CutMix + Flip + SE Block) | 46.45%              |
| U-Net 3 (Weighted Loss)            | 54.66%              |
| U-Net 4 (Exclude Class 0 from Loss)| 71.17%              |
| **Final U-Net**                    | **73.22%**          |

✅ Score: 5.5/5.5


