# Detection of Deepfakes in Lung CT Scans Using GAN-Generated Images with Custom and Pretrained CNN Models

## 📌 Overview

This project focuses on detecting deepfake lung CT scan images using deep learning. Since publicly available fake medical image datasets are limited, synthetic CT scan images were generated using a Generative Adversarial Network (GAN). These generated images, along with real CT scans, were used to train and evaluate both pretrained and custom Convolutional Neural Network (CNN) models.

The objective is to build a reliable system capable of distinguishing between authentic and GAN-generated lung CT scans, helping improve the trustworthiness of AI-assisted medical diagnosis.

---

## 🎯 Objectives

- Generate realistic fake lung CT scan images using GANs.
- Build a balanced dataset containing real and synthetic CT scans.
- Train pretrained CNN models using transfer learning.
- Develop custom CNN architectures from scratch.
- Compare the performance of pretrained and custom models.
- Improve the reliability of AI systems in medical imaging.

---

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- PyTorch
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab
- Jupyter Notebook

---

## 📂 Dataset

### Real Images
- Lung CT scan images collected from Kaggle.

### Fake Images
- Generated using a Generative Adversarial Network (GAN).

### Dataset Summary

| Category | Images |
|----------|--------|
| Real CT Images | 900 |
| GAN Generated Images | 900 |
| Total Images | 1800 |

### Dataset Split

- Training: 80%
- Validation: 10%
- Testing: 10%

---

## 🔄 Image Preprocessing

- Resize images to **224 × 224**
- Convert grayscale images to RGB
- Normalize pixel values to **[0,1]**
- Store processed images for efficient loading

---

# Methodology

## Method 1: Transfer Learning

Pretrained models:

- VGG16
- InceptionV3 (GoogleNet)
- ResNet50

Custom variants:

- ResNet34
- ResNet50 Variant 1
- ResNet50 Variant 2

### Training Configuration

- Transfer Learning
- Adam / AdamW Optimizer
- Binary & Categorical Cross-Entropy Loss
- Dropout Regularization
- Early Stopping
- Model Checkpointing

---

## Method 2: Custom CNN Models

Designed and trained from scratch.

Models:

- CNN 1
- CNN 2
- CNN 3
- CNN 4

Training Features:

- Adam / RMSProp Optimizer
- Binary Cross-Entropy Loss
- Dropout Regularization
- Early Stopping
- Learning Rate Tuning

---

# 📊 Results

## Pretrained Models

| Model | Accuracy |
|--------|----------|
| VGG16 | **98%** |
| InceptionV3 | 96% |
| ResNet50 | 92% |
| ResNet50 Variant 1 | 96.11% |
| ResNet50 Variant 2 | 93% |
| ResNet34 | 50% |

---

## Custom CNN Models

| Model | Accuracy |
|--------|----------|
| CNN 1 | **98%** |
| CNN 2 | **98%** |
| CNN 3 | 96% |
| CNN 4 | **98%** |

---

## 🏆 Best Performing Models

### Transfer Learning

- VGG16
- Accuracy: **98%**

### Custom Models

- CNN 1
- CNN 2
- CNN 4

Accuracy: **98%**

---

## 📈 Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 🔍 Key Findings

- Transfer learning significantly improves convergence speed and classification performance.
- VGG16 achieved the highest accuracy among pretrained models.
- Properly designed custom CNNs can achieve performance comparable to pretrained models.
- Dropout and regularization effectively reduced overfitting.
- GAN-generated images provide an effective solution when fake medical datasets are unavailable.

---

## 🚀 Future Work

- Increase dataset diversity.
- Generate higher-quality synthetic images using StyleGAN or CycleGAN.
- Explore Vision Transformers (ViT).
- Develop real-time medical deepfake detection systems.
- Extend the framework to MRI and X-ray datasets.

---

## 👨‍💻 Authors

**Uppalapati Venkata Ashok Adithya**

**Mannem Yuvaraju**

School of Computer Science and Engineering

VIT-AP University
