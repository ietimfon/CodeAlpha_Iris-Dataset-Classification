# CodeAlpha_Iris-Dataset-Classification
In this project, I trained a machine learning model that can learn from the measurements of the iris species and classify them.
___

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Workflow](#workflow)
- [Key Insights](#key-insights)
- [Interpretation](#interpretation)

### Overview
This project demonstrates a machine learning workflow for classifying iris flowers based on their sepal and petal measurements. The project includes data exploration, preprocessing, model training with a Random Forest classifier, and making predictions on new data.

### Dataset
The Iris dataset is a classic dataset in machine learning and statistics. It contains 150 samples of iris flowers, each with four features:

- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

The flowers belong to three species:

- Iris setosa
- Iris versicolor
- Iris virginica

### Requirements
To run this project, you'll need:

- Python 3.6+
- Jupyter Notebook
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

### Workflow

#### 1. Data Exploration:
- Loaded and examined the dataset
- Performed statistical analysis

#### 2. Data Preprocessing:
- Checked for missing values
- Analyzed feature correlations
- Split data into training and test sets

#### 3. Model Training:
- Trained a Random Forest Classifier
- Evaluated model performance
- Examined feature importance

#### 4. Prediction:
- Created sample measurements for prediction
- Used the trained model to predict iris species

### Key Insights

|  Feature  |Importance Score|          Interpretation         |
|-----------|----------------|---------------------------------|
|Petal Length (cm)|0.440 (44.0%)|Most important feature - accounts for nearly half of the classification decision|
|Petal Width (cm)|0.422 (42.2%)|Nearly as important as petal length - combined petal features drive ~86% of predictions|
|Sepal Length (cm)|0.108 (10.8%)|Secondary influence - contributes modestly to classification|
|Sepal Width (cm)|0.030 (3.0%)|Least important - minimal impact on species determination|

### Interpretation
1. Petal Measurements Dominate: Together, petal length and width account for 86.2% of the classification importance, suggesting these are the primary distinguishing characteristics between iris species.
2. Sepal Characteristics Less Informative: The sepal measurements (particularly sepal width) contribute relatively little to the model's decision-making process.
3. Biological Significance: This aligns with botanical knowledge - iris species are typically distinguished more by petal characteristics than sepal features.
