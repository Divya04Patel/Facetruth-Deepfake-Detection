# FaceTruth: Deepfake Detection for Images  


## Introduction  
Deepfakes are synthetic media generated using deep learning techniques, often to create hyper-realistic fake images and videos. They can pose significant threats to security, trust, and authenticity in digital communications. This project focuses on detecting deepfake images using machine learning and deep learning models, aiming to distinguish between real and fake images based on subtle inconsistencies introduced during synthetic generation.  

![Project Overview](https://github.com/user-attachments/assets/02861838-f1d7-46c4-99d0-19dc2da350f0)  


## Problem Statement
The primary challenge is to build a model that can analyze an image and classify it as real or fake (deepfake). Deepfakes often contain minute artifacts such as unnatural skin textures, inconsistent lighting, irregular facial features, and other anomalies not easily detected by the human eye. The goal is to automate this detection process reliably and accurately.

## Methodology
*1.Data Collection and Preprocessing:-*
A dataset containing both real and fake images is collected (e.g., FaceForensics++, DeepFake Detection Dataset).
Images are preprocessed through resizing, normalization, and augmentation techniques to enhance the robustness of the model.

*2.Model Architecture:-*
A Convolutional Neural Network (CNN) architecture is employed for feature extraction and classification.
Transfer learning techniques (e.g., using pretrained models like EfficientNet, XceptionNet) can be used to improve performance.
Regularization methods such as dropout and data augmentation are applied to prevent overfitting.

*3.Training:-*
The model is trained on labeled data using appropriate loss functions (e.g., Binary Crossentropy) and optimization algorithms (e.g., Adam Optimizer).
Performance is monitored using metrics like accuracy, precision, recall, and F1 score.

*4.Prediction:-*
Users can upload images (JPEG/PNG/JPG) up to 10MB. The interface includes options to clear or reprocess the file, ensuring flexibility during analysis.

<img width="1887" height="829" alt="image" src="https://github.com/user-attachments/assets/ec9ec3fe-3aa8-4118-9254-026336f8267a" />


The "Detect Deepfake" button triggers the model to scan the uploaded image for AI-generated artifacts, providing a real-or-fake prediction based on learned features.

<img width="1892" height="821" alt="image" src="https://github.com/user-attachments/assets/c86a7316-7e46-4c4b-8c2a-88974a464328" />


The model analyzes the input image and detects patterns consistent with authentic (non-deepfake) content, displaying a confidence indicator like "This image appears Authentic."

<img width="1894" height="828" alt="image" src="https://github.com/user-attachments/assets/1468d7c1-7792-41bd-95e4-8243a2f0ef0f" />

# Key Techniques Used
1) CNN-based Feature Extraction
2) Transfer Learning with pretrained models
3) Image Data Augmentation
4) Regularization to Prevent Overfitting
5) Binary Classification Metrics for Evaluation
6) Flask-based Web Deployment


