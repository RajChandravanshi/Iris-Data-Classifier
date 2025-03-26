<!DOCTYPE html>
<html lang="en">
    
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
    
<body>

<h1 style="text-align:center;">🌸 Iris Dataset Classification using AdaBoost & ANN 🌸</h1>

<p style="text-align:center;">By <strong>Raj Chandravanshi</strong></p>

<h2>📌 Introduction</h2>
<p>
This project applies the <strong>AdaBoost Algorithm</strong> and <strong>Artificial Neural Network (ANN)</strong> to classify the famous <strong>Iris Dataset</strong>. 
It includes data preprocessing, exploratory data analysis, feature engineering, model training, and evaluation.
</p>

<h2>📖 Table of Contents</h2>
<ul>
    <li><a href="#dataset-description">Dataset Description</a></li>
    <li><a href="#eda">Exploratory Data Analysis (EDA)</a></li>
    <li><a href="#feature-engineering">Feature Engineering</a></li>
    <li><a href="#model-training">Model Training</a></li>
    <li><a href="#model-evaluation">Model Evaluation</a></li>
    <li><a href="#custom-adaboost">Custom AdaBoost Implementation</a></li>
    <li><a href="#ann-model">Artificial Neural Network (ANN) Model</a></li>
    <li><a href="#results">Results</a></li>
</ul>

<h2 id="dataset-description">📂 Dataset Description</h2>
<p>
The <strong>Iris dataset</strong> consists of 150 samples from three species of Iris flowers:
<ul>
    <li><em>Iris Setosa</em></li>
    <li><em>Iris Versicolor</em></li>
    <li><em>Iris Virginica</em></li>
</ul>
Each sample contains the following features:
<ul>
    <li><strong>SepalLengthCm</strong></li>
    <li><strong>SepalWidthCm</strong></li>
    <li><strong>PetalLengthCm</strong></li>
    <li><strong>PetalWidthCm</strong></li>
    <li><strong>Species</strong> (Target Variable)</li>
</ul>
</p>

<h2 id="eda">📊 Exploratory Data Analysis (EDA)</h2>
<p>Several visualizations were performed, including:</p>
<ul>
    <li>Histograms & Pairplots</li>
    <li>Correlation Heatmap</li>
    <li>Boxplots & Violin plots</li>
    <li>PCA for dimensionality reduction</li>
</ul>
<p>Here is an example of the PCA visualization:</p>
<img src="pca_plot.png" alt="PCA Projection of the Iris Dataset" width="600"/>

<h2 id="feature-engineering">⚙️ Feature Engineering</h2>
<p>The dataset is preprocessed using:</p>
<ul>
    <li>Label Encoding for the target variable</li>
    <li>Standardization using <code>StandardScaler</code></li>
    <li>Splitting into training and testing sets</li>
</ul>

<h2 id="model-training">🚀 Model Training</h2>
<p>The following models were trained:</p>
<ul>
    <li><strong>AdaBoost Classifier</strong> with <em>DecisionTreeClassifier (max_depth=1)</em></li>
    <li><strong>Custom AdaBoost Implementation</strong> (Built from scratch)</li>
    <li><strong>Artificial Neural Network (ANN)</strong> with multiple Dense layers</li>
</ul>

<h2 id="model-evaluation">📈 Model Evaluation</h2>
<p>Each model was evaluated using:</p>
<ul>
    <li>Accuracy Score</li>
    <li>Confusion Matrix</li>
    <li>Loss & Accuracy Curves (For ANN)</li>
</ul>

<h2 id="custom-adaboost">🛠️ Custom AdaBoost Implementation</h2>
<p>A custom implementation of AdaBoost was developed using Python & NumPy.</p>

<h2 id="ann-model">🔬 Artificial Neural Network (ANN) Model</h2>
<p>The ANN model architecture:</p>
<ul>
    <li>Dense Layers with <code>ReLU</code> Activation</li>
    <li>Batch Normalization & Dropout</li>
    <li>Final Softmax Layer for Classification</li>
</ul>
<p><img src="ann_accuracy_plot.png" alt="ANN Accuracy Plot" width="600"/></p>

<h2 id="results">📊 Results</h2>
<table border="1">
    <tr>
        <th>Model</th>
        <th>Accuracy</th>
    </tr>
    <tr>
        <td>AdaBoost (Sklearn)</td>
        <td>93.33%</td>
    </tr>
    <tr>
        <td>Custom AdaBoost</td>
        <td>93.33%</td>
    </tr>
    <tr>
        <td>ANN Model</td>
        <td>96.67%</td>
    </tr>
</table>
