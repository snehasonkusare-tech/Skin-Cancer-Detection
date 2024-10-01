Skin Disease Detection
Author
Sneha Sonkusare

Date
April 30, 2024

Overview
This project focuses on the detection of skin diseases using machine learning techniques. The goal is to build a model that can classify images of skin lesions into benign or malignant categories, leveraging image processing and classification algorithms.

Table of Contents
Getting Started
Prerequisites
Directory Structure
Usage
Modeling
Results
Contributing
License

Getting Started
To run this project, clone the repository and set up the environment as outlined in the prerequisites section.
git clone https://github.com/yourusername/skin-disease-detection.git
cd skin-disease-detection

Prerequisites
Make sure you have the following software and libraries installed:
R (version 4.0 or higher)
RStudio
Required R libraries:
jpeg
imager
abind
caret
glmnet
randomForest
e1071
pROC
ggplot2

You can install the required libraries using the following command in R:
install.packages(c("jpeg", "imager", "abind", "caret", "glmnet", "randomForest", "e1071", "pROC", "ggplot2"))

Directory Structure
/skin-disease-detection
├── /benign                 # Folder containing benign skin lesion images
├── /malignant              # Folder containing malignant skin lesion images
├── skin_disease_detection.R # R script for skin disease detection
├── README.md               # This README file

Usage
Place your JPEG images of skin lesions in the benign and malignant folders.
Open skin_disease_detection.R in RStudio.
Run the script to execute the image processing and model training process.
Modeling
The project uses the following machine learning models for classification:

Logistic Regression
Random Forest
Support Vector Machine (SVM)
The models are evaluated using cross-validation, and performance metrics such as accuracy, sensitivity, specificity, and confusion matrix are provided for each model.

Key Steps in the Script
Image Preprocessing: Reads and flattens images to prepare them for modeling.
Principal Component Analysis (PCA): Reduces the dimensionality of the image data.
Model Training: Trains multiple models on the PCA-transformed training data.
Evaluation: Calculates and displays model performance metrics and visualizes results.
Results
The project outputs the accuracy of each model, confusion matrices, and ROC curves comparing the different models' performance.

Example Output
Logistic Regression Accuracy:76%
Random Forest Accuracy: 72.33%
SVM Accuracy: 50%

