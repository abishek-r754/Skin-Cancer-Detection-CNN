# Skin Cancer Detection using Deep Learning (CNN)

## Project Overview
This project focuses on building a deep learning model to classify different types of skin cancer using image data. The goal is to assist in early detection of skin diseases by leveraging Convolutional Neural Networks (CNN).

The model is trained to classify images into 7 different categories of skin lesions using the HAM10000 dataset.

---

## Problem Statement
Skin cancer is one of the most common types of cancer worldwide. Early detection is critical for effective treatment. Manual diagnosis can be time-consuming and requires expert knowledge.

This project aims to develop an automated system that can classify skin lesions using deep learning techniques.

---

## Dataset
- Dataset: HAM10000 (Human Against Machine with 10000 training images)
- Format used: Skin Cancer MNIST (28x28 RGB version)
- Total classes: 7

### Classes:
1. Melanocytic nevi  
2. Melanoma  
3. Benign keratosis-like lesions  
4. Basal cell carcinoma  
5. Actinic keratoses  
6. Vascular lesions  
7. Dermatofibroma  

---

## Project Workflow

### 1. Data Loading
The dataset was loaded from a CSV file containing pixel values of images and corresponding labels.

### 2. Data Preprocessing
- Converted data into NumPy arrays  
- Normalized pixel values (0–255 → 0–1)  
- Reshaped data into image format (28x28x3)  
- Split into training and testing datasets  

### 3. Model Building
A Convolutional Neural Network (CNN) was built using TensorFlow/Keras with the following layers:

- Conv2D (feature extraction)  
- MaxPooling (downsampling)  
- Flatten (convert to vector)  
- Dense layers (classification)  
- Dropout (reduce overfitting)  

### 4. Model Training
- Optimizer: Adam  
- Loss function: Sparse Categorical Crossentropy  
- Epochs: 10  
- Batch size: 32  

### 5. Model Evaluation
The model performance was evaluated using:
- Accuracy  
- Confusion Matrix  
- Classification Report (Precision, Recall, F1-score)  

### 6. Prediction
The trained model was used to predict the class of unseen test images.

---

## Results
- Training Accuracy: ~72%  
- Validation Accuracy: ~72%  

The model performed well on dominant classes but struggled with minority classes due to dataset imbalance.

---

## Key Observations
- Class imbalance significantly affects prediction performance  
- Majority class dominates accuracy  
- Some classes have very low recall  

---

## Limitations
- Low-resolution images (28x28) reduce feature quality  
- No data augmentation applied  
- Basic CNN architecture used  
- Model struggles with minority classes  

---

## Future Improvements
- Use high-resolution image dataset  
- Apply data augmentation techniques  
- Use transfer learning (ResNet, MobileNet, VGG16)  
- Handle class imbalance (SMOTE, class weights)  
- Improve model accuracy beyond 80%  

---

## Technologies Used
- Python  
- TensorFlow / Keras  
- NumPy  
- Pandas  
- Matplotlib  
- Scikit-learn  

---

## How to Run the Project

1. Install required libraries:




2. Run the Jupyter Notebook:



3. Open the notebook file and execute all cells.

---

## Project Duration
This project was developed over a period of 4 months (January – April) as part of an academic final-year project.

---

## Conclusion
This project demonstrates the use of deep learning in medical image classification. While the model achieves moderate accuracy, it highlights the importance of data quality and model optimization in real-world applications.

---

## Author
Abishek R
