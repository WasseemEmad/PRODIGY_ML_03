# PRODIGY_ML_03

# **Cat vs Dog Image Classification using SVM**

This project demonstrates image classification using Support Vector Machine (SVM) models to distinguish between images of cats and dogs. The project includes multiple stages, such as data preprocessing, feature extraction, dimensionality reduction, and hyperparameter tuning. Different approaches, including raw pixel data, Principal Component Analysis (PCA), and Histogram of Oriented Gradients (HOG) features, are explored to improve classification accuracy.

# **Project Overview**

## **The goal of this project is to classify images as either "cat" or "dog" using different feature extraction techniques and machine learning algorithms. The approaches explored include:**

Training an SVM classifier on flattened pixel data.
Reducing dimensionality with Principal Component Analysis (PCA).
Extracting Histogram of Oriented Gradients (HOG) features with varying parameters.
Hyperparameter tuning with GridSearchCV to optimize the SVM model.

# **Dataset**

The dataset contains images of cats and dogs stored in a zip file, which needs to be extracted before processing. Each image is labeled based on its filename (cat or dog). The dataset is split into training (80%) and testing (20%) sets.

# **Code Structure**
## **The project is structured into several sections to perform different tasks:**

### **Extracting the Zip File Containing the Images:**
Extracts images for further processing.
### **Loading and Preprocessing Images:**
Resizes images to 64x64 pixels and assigns labels.
### **Normalizing and Flattening the Image Data:**
Converts images to a normalized 1D array.
### **Splitting the Dataset into Training and Testing Sets:**
Divides the dataset for training and evaluation.
### **Training a Support Vector Machine (SVM) Classifier:**
Uses flattened image data for training and testing.
### **Evaluating the SVM Classifier:**
Computes accuracy, classification report, and confusion matrix.
### **Feature Reduction Using PCA:**
Reduces dimensionality to 1000 features.
### **Training and Evaluating SVM After PCA:** 
Trains and evaluates an SVM classifier using reduced features.
### **Hyperparameter Tuning Using GridSearchCV:**
Finds the optimal hyperparameters for the SVM classifier.
### **Extracting HOG Features:**
Uses different pixel-per-cell settings to extract HOG features.
### **Training and Evaluating SVM with HOG Features:**
Trains and evaluates SVM with HOG features using different parameters.

# **Results**

## **The performance of the SVM classifier is evaluated using various approaches:**

Flattened Pixel Data: Basic approach without feature extraction.
PCA: Dimensionality reduction helps improve training speed and potentially accuracy.
HOG Features: Different configurations (32x32, 16x18, and 8x8 pixels per cell) are tested.
Results are presented in terms of accuracy, precision, recall, F1-score, and confusion matrix for each approach.
