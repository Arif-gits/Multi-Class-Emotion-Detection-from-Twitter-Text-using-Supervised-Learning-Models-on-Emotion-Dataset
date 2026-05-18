# Multi-Class-Emotion-Detection-from-Twitter-Text-using-Supervised-Learning-Models-on-Emotion-Dataset

A machine learning-based emotion classification project developed for the course CSE422: Artificial Intelligence. This project focuses on detecting human emotions from English-language Twitter messages using multiple supervised learning algorithms.

## Project Overview

The project uses the **Emotion Dataset for Emotion Recognition Tasks**, where tweets are classified into six emotion categories:

* Anger
* Fear
* Joy
* Love
* Sadness
* Surprise

The primary objective was to compare the performance of different machine learning models for multi-class emotion classification and analyze their effectiveness on textual data.

## Dataset Information

Dataset Source:
[Emotion Dataset for Emotion Recognition Tasks](https://www.kaggle.com/datasets/parulpandey/emotion-dataset?utm_source=chatgpt.com)

Reference Paper:
CARER: Contextualized Affect Representations for Emotion Recognition

### Dataset Structure

The dataset contains:

| Subset     | Size   |
| ---------- | ------ |
| Training   | 16,000 |
| Validation | 2,000  |
| Test       | 2,000  |

Total dataset size: **20,000 tweets**

### Features

* **Text** → Twitter message/text snippet
* **Label** → Numerical emotion category (0–5)

## Project Workflow

### 1. Data Preprocessing

* Combined training, validation, and test datasets
* Removed duplicate entries
* Checked for missing values
* Prepared dataset for model training

### 2. Feature Scaling & Balancing

* Addressed class imbalance using oversampling techniques
* Used resampling methods to improve model fairness and stability

### 3. Dataset Splitting

Final dataset split ratio:

* 70% Training
* 20% Testing
* 5% Validation

## Machine Learning Models Used

The following classification algorithms were implemented and evaluated:

* Logistic Regression
* Decision Tree
* Naive Bayes
* K-Nearest Neighbors (KNN)
* Neural Network

Each model was evaluated using:

* Accuracy
* Precision
* Recall
* Confusion Matrix

## Observations

### Logistic Regression

* Produced balanced and consistent performance
* Strong baseline classifier for text classification tasks

### Decision Tree

* Comparable performance to Logistic Regression
* Risk of overfitting depending on tree depth

### Naive Bayes

* Slightly lower performance
* Independence assumptions may not align fully with textual features

### KNN

* Lower overall performance
* Likely affected by high-dimensional text data

### Neural Network

* Strong predictive performance
* Suitable for scalable and complex datasets

## Conclusion

For this dataset, **Logistic Regression** and **Decision Tree** models provided the best balance between simplicity, interpretability, and performance. Neural Networks also performed well and offer better scalability for larger or more complex datasets.

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## Authors

* Arif Bin Islam
* Tahmid Uddin Protim

## Course Information

* Course: CSE422: Artificial Intelligence
* Submission Date: January 2024
