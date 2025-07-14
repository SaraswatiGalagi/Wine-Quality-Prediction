🍷 Wine Quality Prediction – Machine Learning
This project applies machine learning techniques to predict the quality of wine based on physicochemical features. It uses logistic regression to classify wine samples as high or low quality.

📁 Project Overview
The objective of this notebook is to:

Load and preprocess a wine quality dataset (white and red wines).

Perform exploratory data analysis (EDA) to understand data distribution and correlations.

Build a binary classification model to predict whether the wine quality is above average.

Evaluate model performance using ROC AUC score.

📂 Dataset
Filename: wine-quality-white-and-red.csv

Source: Assumed to be manually combined from red and white wine quality datasets.

Target Variable: quality (converted into binary: >5 as 1 – good quality, ≤5 as 0 – lower quality)

🧪 Features
Key features include:

Fixed acidity

Volatile acidity

Citric acid

Residual sugar

Chlorides

Free sulfur dioxide

Density

pH

Sulphates

Alcohol

Type (white/red)

Note: The total sulfur dioxide column was removed due to high correlation with other features.

🔧 Requirements
This code was built to run in Google Colab and relies on the following libraries:

bash
Copy
Edit
numpy
pandas
matplotlib
seaborn
scikit-learn
xgboost
🚀 How to Run
Mount Google Drive:

python
Copy
Edit
from google.colab import drive
drive.mount('/content/drive')
Load dataset from your Google Drive path:

python
Copy
Edit
path_wine = '/content/drive/MyDrive/Machine Learning/wine-quality-white-and-red.csv'
Run all cells in sequence to perform:

Data loading

Null value handling

Histogram plotting and heatmaps

Feature engineering (best quality)

Data normalization

Model training and evaluation

🧠 Model
Logistic Regression is used as the classification model.

Performance is measured using ROC AUC Score.

📊 Results
Output includes:

ROC AUC Score for both training and test sets

Feature histograms and correlation heatmaps

📌 Notes
The target variable is converted into a binary label (best quality) for simplified classification.

Only logistic regression is used in this version; code is structured to add more models easily.
