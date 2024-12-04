# Iris Dataset Classification using AdaBoost

## Introduction
This project demonstrates the application of the **AdaBoost algorithm** to classify the famous **Iris dataset**. The study includes two implementations:  
1. **Scikit-learn's AdaBoost Classifier**  
2. **Custom-built AdaBoost Classifier**  

Both models achieved an impressive accuracy of **93%**, showcasing the power of ensemble learning for classification tasks.

---

## Table of Contents
- [Dataset Description](#dataset-description)  
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)  
- [Feature Engineering](#feature-engineering)  
- [Model Training](#model-training)  
- [Model Evaluation](#model-evaluation)  
- [Custom AdaBoost Implementation](#custom-adaboost-implementation)  
- [Results](#results)  
- [Technologies Used](#technologies-used)  
- [How to Run the Project](#how-to-run-the-project)  
- [References](#references)

---

## Dataset Description
The Iris dataset is a popular dataset in machine learning and statistics, consisting of **150 samples** of iris flowers. Each sample has:  
### Features
- **Sepal Length (cm)**  
- **Sepal Width (cm)**  
- **Petal Length (cm)**  
- **Petal Width (cm)**  

### Target Variable
- **Species** (*Iris-setosa*, *Iris-versicolor*, *Iris-virginica*)  

This dataset is widely used for classification tasks due to its simplicity and balanced classes.

---

## Exploratory Data Analysis (EDA)
### Key Insights
- Summary statistics and data types were explored to understand the structure of the dataset.  
- Visualization techniques were used to identify relationships and distributions.

### Visualizations
- **Pairplots**: Explored feature correlations.  
- **Heatmaps**: Highlighted the strength of feature correlations.  
- **Boxplots and Violin Plots**: Examined data distribution.  
- **Scatterplots**: Helped in outlier detection.  

---

## Feature Engineering
### Steps Taken
1. Split the dataset into **training (80%)** and **testing (20%)** sets.  
2. Applied **Label Encoding** to convert categorical target labels into numeric form.  
3. Standardized numerical features using **StandardScaler** to improve model performance.

---

## Model Training
### Approaches
1. **Scikit-learn AdaBoost Classifier**:
   - **Base Estimator**: DecisionTreeClassifier (max_depth=1)  
   - **Number of Estimators**: 50  

2. **Custom AdaBoost Implementation**:
   - Built from scratch.  
   - Designed to handle multiclass classification using a **one-vs-all strategy**.

---

## Model Evaluation
### Metrics Used
- **Accuracy Score**  
- **Classification Report** (Precision, Recall, F1-Score)  

### Results
- **Scikit-learn AdaBoost Classifier**: 93% accuracy  
- **Custom AdaBoost Classifier**: 93% accuracy  

---

## Custom AdaBoost Implementation
### Features
- Uses **DecisionTreeClassifier** as the base learner.  
- Handles multiclass classification via **one-vs-all encoding**.  
- Updates sample weights based on misclassification.

### Implementation Steps
1. Initialize sample weights equally.  
2. Train weak learners iteratively.  
3. Calculate classifier weight (**alpha**) based on the error rate.  
4. Update sample weights to focus more on misclassified samples.  
5. Combine all weak learners to form a strong classifier.

---

## Results
- Both implementations achieved **93% accuracy**, demonstrating the robustness of AdaBoost.  
- **Key Insight**: Petal dimensions are the most important features for classification.

---

## Technologies Used
- **Python Libraries**: Scikit-learn, Pandas, Numpy, Matplotlib, Seaborn.  

---
