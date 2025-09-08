# AIML Codex

This repository contains two Machine Learning projects with interactive Gradio interfaces.  
The projects demonstrate how regression and classification models can be trained, evaluated, and deployed with simple user interfaces.

## Projects Overview

### 1. House Price Prediction
Predicts the median value of houses using the Boston Housing dataset (HousingData.csv).

Objective: Estimate house prices based on multiple housing and environmental features.  
Approach:
- Missing values are filled using column mean.  
- Features are normalized using StandardScaler.  
- Data is split into training and testing sets (80/20).  
- Linear Regression model is trained and evaluated.  

Evaluation Metrics:
- Mean Squared Error (MSE)  
- Mean Absolute Error (MAE)  
- Coefficient of Determination (R²)  

Extended Feature: Predictions are also classified into categories (Low, Medium, High).  
Interface: Gradio interface allows users to input housing features and view the predicted price along with the category.

### 2. Spam Mail Detection
Classifies email messages as Spam or Ham using the Spam/Ham dataset (spam_ham_dataset.csv).

Objective: Automatically identify spam messages.  
Approach:
- Text data is preprocessed using TF-IDF with the top 3000 features.  
- Labels are encoded to numeric values.  
- Naive Bayes (MultinomialNB) is used for classification.  

Evaluation Metrics:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix and Classification Report  

Interface: Gradio interface provides a textbox where users can enter a message and instantly see whether it is spam or ham.

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/aiml-codex.git
   cd aiml-codex
