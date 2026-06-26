# Student Placement Prediction using Logistic Regression

Predicting student placement using **Machine Learning** based on **CGPA** and **IQ**. This project demonstrates a complete binary classification workflow using **Logistic Regression**, including data preprocessing, visualization, model training, and performance evaluation.

# Project Overview

This project aims to predict whether a student will be **placed or not placed** based on two key academic attributes:

*  **CGPA**
*  **IQ**

# Features

* Data loading using Pandas
* Exploratory Data Analysis (EDA)
* Feature selection
* Data preprocessing
* Train-Test Split
* Feature Scaling using StandardScaler
* Logistic Regression model training
* Prediction on unseen data
* Model performance evaluation
* Decision boundary visualization
# Project Structure
Student-Placement-Prediction
├── Toy_Project.ipynb          # Complete Machine Learning notebook
├── placement.csv              # Dataset
├── README.md                  # Project documentation
└── requirements.txt           # Python dependencies
# Dataset
The dataset contains information about students with the following attributes:

Feature   | Description                                  
 --------- | -------------------------------------------- 
 CGPA      | Student's cumulative grade point average     
 IQ        | Intelligence Quotient score                  
 Placement | Target variable (0 = Not Placed, 1 = Placed) 
# Technologies Used
* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Jupyter Notebook
# Machine Learning Workflow

# 1. Import Required Libraries

python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
# 2. Load the Dataset
df = pd.read_csv("placement.csv")
# 3. Exploratory Data Analysis
* Inspect the dataset
* Check data types
* Understand feature distributions
* Visualize placement categories
# 4. Data Preprocessing
* Select relevant features
* Separate input and output variables
* Prepare data for training
# 5. Train-Test Split
The dataset is divided into training and testing datasets to evaluate model performance on unseen data.

# 6. Feature Scaling
Since Logistic Regression performs better on standardized data, the features are scaled using **StandardScaler**.
python
from sklearn.preprocessing import StandardScaler.
# 7. Model Training
A Logistic Regression classifier is trained using the processed training dataset.

python
from sklearn.linear_model import LogisticRegression

model = LogisticRegression()
model.fit(X_train, y_train)
# 8. Prediction

Predictions are generated for the testing dataset.

python
y_pred = model.predict(X_test)
# 9. Model Evaluation
The model performance is evaluated using:
* Accuracy Score
  python
from sklearn.metrics import accuracy_score

accuracy_score(y_test, y_pred)
# Visualization
The project includes visualizations such as:
* Scatter plot of CGPA vs IQ
* Placement distribution
* Decision boundary of Logistic Regression
These visualizations help in understanding how the model separates the two classes.
# Results
The Logistic Regression model successfully classifies students as **Placed** or **Not Placed** based on their CGPA and IQ.
The notebook evaluates the model using the **Accuracy Score**, demonstrating the effectiveness of Logistic Regression for binary classification problems.

# Learning Outcomes
This project demonstrates:
* Data preprocessing
* Exploratory Data Analysis
* Feature engineering
* Data visualization
* Feature scaling
* Logistic Regression
* Binary Classification
* Model evaluation using Scikit-learn
# Future Improvements

* Add more student-related features
* Perform feature engineering
* Try advanced classification models such as:
  * Decision Tree
  * Random Forest
  * Support Vector Machine (SVM)
  * K-Nearest Neighbors (KNN)
* Hyperparameter tuning
* Cross-validation
* Deploy the model using Streamlit or Flask
# Contributing
Contributions are welcome!
If you'd like to improve this project:
1. Fork the repository
2. Create a new branch
3. Make your changes
4. Commit your changes
5. Open a Pull Request

# Author
**Piu**
Production & Industrial Engineering
National Institute of Technology Jamshedpur

