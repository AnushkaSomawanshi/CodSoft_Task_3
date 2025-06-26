# CODSOFT Internship Projects

This repository includes the work I completed as part of the CODSOFT Data Science Internship.  
Throughout this internship, I worked on multiple machine learning tasks that improved my understanding of data preprocessing, model building, and classification techniques using Python.

This README describes **Task 3: Iris Flower Classification**.

---

# Task 3: Iris Flower Classification

## Project Overview

The objective of this project is to build a classification model that accurately predicts the species of Iris flowers based on their sepal and petal measurements.  
The Iris dataset is a classic, beginner-friendly dataset used widely in machine learning and statistics.

There are three species in the dataset:
- Iris Setosa  
- Iris Versicolor  
- Iris Virginica  

Each flower sample includes four features:
- Sepal Length (cm)  
- Sepal Width (cm)  
- Petal Length (cm)  
- Petal Width (cm)

---

## What I Did

- Loaded the Iris dataset using Scikit-learn  
- Explored the data through visualizations and pairplots  
- Checked for missing values and ensured the data was clean  
- Encoded the target labels for classification  
- Trained and evaluated multiple classification models, including:
  - Logistic Regression  
  - Support Vector Machine (SVM)  
  - Random Forest Classifier  
- Compared model accuracies and selected the best-performing one  
- Built a sample input interface to predict species based on new flower measurements  

---

## What I Observed

- The dataset is well-balanced and clean, with no missing values  
- Petal length and petal width are strong indicators of species  
- SVM and Random Forest models performed best in terms of accuracy  
- Setosa is the easiest to classify due to its distinct petal measurements  
- Versicolor and Virginica overlap slightly but can still be separated using proper boundaries  

---

## Dataset Description

Each entry in the Iris dataset contains the following:

- Sepal Length (float)  
- Sepal Width (float)  
- Petal Length (float)  
- Petal Width (float)  
- Species (target class: Setosa, Versicolor, Virginica)

---

## Key Steps in the Project

### 1. Data Preprocessing

- Loaded dataset and converted it into a DataFrame  
- Verified feature scales and label distribution  
- Performed label encoding for species names if needed

### 2. Exploratory Data Analysis (EDA)

- Created scatter plots, histograms, and pairplots using seaborn  
- Checked feature correlations and distribution across species  

### 3. Model Training

- Split the data into training and test sets using `train_test_split`  
- Trained the following models:
  - Logistic Regression  
  - SVM  
  - Random Forest  
- Evaluated performance using accuracy score and confusion matrix  

### 4. Sample Prediction

```python
# Sample flower data
sample = [[5.1, 3.5, 1.4, 0.2]]  # Example of Iris-setosa measurements

# Predict species
prediction = model.predict(sample)
print("Predicted Iris Species:", prediction[0])
