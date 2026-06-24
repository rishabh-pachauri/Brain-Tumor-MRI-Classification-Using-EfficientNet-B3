# Brain Tumor MRI Classification Using EfficientNet-B3

## Overview

This project presents a deep learning-based solution for automated brain tumor classification using MRI scans and the EfficientNet-B3 architecture. The objective is to accurately classify brain MRI images into different tumor categories, assisting in the early detection and diagnosis of brain tumors.

The project serves as a practical introduction to medical image analysis, transfer learning, and deep learning-based healthcare applications.

---

## Problem Statement

Brain tumors are among the most critical neurological disorders, requiring timely and accurate diagnosis for effective treatment planning. Manual interpretation of MRI scans is time-consuming and relies heavily on expert radiologists.

This project aims to develop an automated image classification system capable of identifying different types of brain tumors from MRI images using deep learning techniques.

---

## Classification Categories

The model classifies MRI images into the following categories:

- Glioma Tumor
- Meningioma Tumor
- Pituitary Tumor
- No Tumor

---

## Learning Objectives

After completing this project, students will be able to:

- Understand medical image classification workflows
- Apply transfer learning using EfficientNet-B3
- Perform image preprocessing and augmentation
- Train deep learning models on MRI datasets
- Evaluate classification performance using standard metrics
- Understand AI applications in healthcare

---

## Dataset Structure

```text
Brain_Tumor_MRI_Dataset/
├── train/
│   ├── glioma/
│   ├── meningioma/
│   ├── pituitary/
│   └── notumor/
│
├── test/
│   ├── glioma/
│   ├── meningioma/
│   ├── pituitary/
│   └── notumor/
```

Each folder contains MRI images corresponding to a specific class.

---

## Technology Stack

- Python
- TensorFlow / Keras
- EfficientNet-B3
- NumPy
- OpenCV
- Matplotlib
- Scikit-Learn
- Jupyter Notebook

---

## Why EfficientNet-B3?

EfficientNet-B3 provides:

- High classification accuracy
- Efficient parameter utilization
- Faster convergence
- Reduced computational cost
- Strong transfer learning performance

These characteristics make it well-suited for medical image classification tasks.

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/brain-tumor-mri-classification.git
cd brain-tumor-mri-classification
```

### Install Dependencies

```bash
pip install tensorflow
pip install numpy matplotlib opencv-python scikit-learn
```

---

## Project Workflow

### 1. Data Loading

- Load MRI images
- Organize training and testing sets
- Verify class distribution

### 2. Image Preprocessing

- Resize images
- Normalize pixel values
- Prepare data for EfficientNet-B3

### 3. Data Augmentation

Apply transformations such as:

- Rotation
- Zoom
- Horizontal Flip
- Brightness Adjustment

to improve model generalization.

### 4. Transfer Learning

Load pre-trained EfficientNet-B3 weights and fine-tune the network for brain tumor classification.

### 5. Model Training

```python
model.fit(
    train_generator,
    validation_data=validation_generator,
    epochs=20
)
```

### 6. Model Evaluation

Evaluate performance using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

### 7. Prediction

Perform classification on unseen MRI images.

```python
prediction = model.predict(image)
```

The model outputs the predicted tumor category along with confidence scores.

---

## Performance Metrics

The trained model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

These metrics provide a comprehensive assessment of model performance across all tumor classes.

---

## Sample Output

For a given MRI scan, the model predicts:

```text
Predicted Class: Glioma Tumor
Confidence: 98.4%
```

---

## Applications

- Clinical Decision Support Systems
- Medical Image Analysis
- Computer-Aided Diagnosis (CAD)
- Healthcare AI Solutions
- Medical Research

---

## Future Enhancements

- Brain Tumor Segmentation
- Tumor Localization using Object Detection
- Explainable AI (Grad-CAM Visualization)
- Web-Based Diagnostic Interface
- Multi-Modal Medical Imaging Support

---

## Repository Structure

```text
brain-tumor-mri-classification/
│
├── dataset/
├── models/
├── notebooks/
├── results/
├── checkpoints/
├── requirements.txt
└── README.md
```

---

## Educational Outcomes

This project helps students gain practical experience in:

- Medical Image Processing
- Deep Learning for Healthcare
- Transfer Learning
- CNN Architectures
- Model Evaluation
- AI-Assisted Diagnosis Systems

---

## Disclaimer

This project is intended for educational and research purposes only. It is not a substitute for professional medical diagnosis or clinical decision-making.

---

## License

This project is intended for educational and research purposes.
