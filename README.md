# Enron Email Dataset Analysis and Classification

### This repository contains code for cleaning, analyzing, and training machine learning models on the Enron Email Dataset. The dataset comprises over 500k emails exchanged among Enron employees and management.

## Data Cleaning
### The initial exploration revealed that email details such as time, sender, and receiver were stored in one column. To address this, we parsed the emails using Python's email library and extracted relevant details into separate columns. This was achieved using the provided code snippet.

## Clustering and Labeling
### To define labels, we employed K-means clustering. Initially, we converted text data into TF-IDF vectors and applied K-means clustering. Dimensionality reduction using PCA facilitated visualization, and the clusters were plotted on a graph. We assigned names to each cluster, resulting in a labeled dataset.

## Model Training and Evaluation
### The dataset was split, and stop words were removed before training the following models:
### - Naive Bayes
### - Support Vector Machine (SVM)
### - Random Forest
### - Logistic Regression

### Model accuracies were as follows:
### - Naive Bayes: 0.773
### - SVM: 0.982
### - Random Forest: 0.978
### - Logistic Regression: 0.985

### We also checked for overfitting through cross-validation:
### - Naive Bayes: Mean CV accuracy: 0.958, Std CV accuracy: 0.023
### - SVM: Mean CV accuracy: 0.958, Std CV accuracy: 0.023
### - Random Forest: Mean CV accuracy: 0.958, Std CV accuracy: 0.023
### - Logistic Regression: Mean CV accuracy: 0.958, Std CV accuracy: 0.023

## Conclusion
### This project demonstrates a pipeline for cleaning, analyzing, and classifying emails from the Enron dataset. The provided code and analysis serve as a foundation for email classification tasks, particularly in contexts like the Barclays Hack O Hire technical track.
