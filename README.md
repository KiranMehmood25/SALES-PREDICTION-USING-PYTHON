# Sales Prediction Using Machine Learning

## Project Overview

This project focuses on predicting product sales using Machine Learning techniques based on advertising expenditure across different media platforms such as TV, Radio, and Newspaper.

The main goal of the project is to analyze how advertising investments influence product sales and build a predictive model capable of estimating future sales performance.

The project demonstrates the complete Machine Learning workflow including:

* Data preprocessing
* Exploratory Data Analysis (EDA)
* Correlation analysis
* Data visualization
* Model training and evaluation
* Sales prediction using Linear Regression
* Residual analysis and performance evaluation

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

# Project Structure

```text
sales-prediction-ml/
│
├── assets/
│   ├── dataset-preview.png
│   ├── correlation-heatmap.png
│   ├── pairplot.png
│   ├── histogram.png
│   ├── residual-analysis.png
│   └── prediction-results.png
│
├── Task 4 Codsoft.ipynb
├── Sales Prediction codsoft.csv
├── README.md
```

---

# Dataset Description

The dataset contains advertising budgets allocated across multiple marketing channels:

* TV Advertising
* Radio Advertising
* Newspaper Advertising

The target variable is:

* Sales

The project analyzes how advertising expenditure impacts sales generation and uses machine learning algorithms to make predictions.

---

# Machine Learning Workflow

## 1. Data Loading

The dataset was loaded using Pandas for data analysis and preprocessing.

```python
import pandas as pd

dfs = pd.read_csv('Sales Prediction codsoft.csv')
```

---

## 2. Data Exploration

Basic data exploration techniques were performed to:

* Check missing values
* Understand data structure
* Analyze statistical information
* Identify feature relationships

---

## 3. Correlation Analysis

A correlation heatmap was created to understand relationships between advertising channels and sales.

### Correlation Heatmap

<img width="515" height="435" alt="sales prediction codsoft Correlation Heatmap" src="https://github.com/user-attachments/assets/5f7350fb-964c-49e5-bf71-ce2f23ed2b56" />


#### What This Graph Shows

The correlation heatmap visualizes the relationship between advertising channels and product sales using correlation coefficients.

* Darker colors represent stronger relationships.
* Lighter colors represent weaker relationships.
* Positive values indicate that increasing advertising budget increases sales.
* Negative values indicate an inverse relationship.

#### Key Insights

* TV advertising shows the strongest positive correlation with sales.
* Radio advertising also contributes positively to sales performance.
* Newspaper advertising has comparatively lower impact.
* The heatmap helps identify which advertising channel influences sales the most.

This visualization helps in feature selection and understanding data relationships before training the machine learning model.

---

## 4. Data Visualization

Different visualizations were used to better understand the dataset and advertising trends.

### Pair Plot Analysis

<img width="1035" height="518" alt="sales prediction codsoft pair plot" src="https://github.com/user-attachments/assets/6eb238ec-76e3-45ca-bd17-38aa558344c4" />
<img width="986" height="986" alt="sales prediction codsoft pair plot 2" src="https://github.com/user-attachments/assets/ccc09b87-93f7-424f-90c1-f30c21f8df8f" />


#### What This Graph Shows

The pair plot displays scatter plots and distributions between all numerical variables in the dataset.

It visualizes relationships between:

* TV advertising and Sales
* Radio advertising and Sales
* Newspaper advertising and Sales

#### Key Insights

* TV advertising shows a strong linear relationship with sales.
* Radio advertising also demonstrates a positive trend.
* Newspaper advertising appears less correlated with sales.
* The diagonal plots display feature distributions.

This graph helps identify trends, patterns, and possible correlations within the dataset.

---

### Dataset Distribution

<img width="822" height="682" alt="sales prediction codsoft histogram" src="https://github.com/user-attachments/assets/69f04bdd-641b-403e-a2e4-f0c4cee7737b" />


#### What This Graph Shows

The histogram visualizes the frequency distribution of advertising budgets and sales values.

#### Key Insights

* Shows how data points are distributed across different ranges.
* Helps identify skewness and concentration of data.
* Useful for understanding whether the dataset is balanced.
* Helps detect outliers or unusual values.

This visualization improves understanding of overall dataset behavior before model training.

---

## 5. Model Training

A Linear Regression model was implemented to predict sales based on advertising budgets.
<img width="577" height="455" alt="sales prediction codsoft Linear Regression" src="https://github.com/user-attachments/assets/024b1ea4-5f70-4bf9-8b34-c34bceb4053c" />


### Features Used

* TV
* Radio
* Newspaper

### Target Variable

* Sales

---

## 6. Model Evaluation

The model performance was evaluated using:

* Mean Squared Error (MSE)
* Residual Analysis
* Prediction Visualization

### Prediction Results

<img width="576" height="455" alt="sales prediction codsoft Results" src="https://github.com/user-attachments/assets/72d4a25a-3030-4a59-8d6f-ab27c19a98c0" />


#### What This Graph Shows

This graph compares actual sales values with predicted sales values generated by the Linear Regression model.

#### Key Insights

* The prediction line closely follows the actual data points.
* Indicates that the model performs effectively on the dataset.
* Demonstrates the relationship between advertising expenditure and sales prediction.
* Helps evaluate how accurately the model predicts future sales.

This visualization highlights the overall performance and prediction capability of the machine learning model.

---

### Residual Analysis

<img width="572" height="455" alt="sales prediction codsoft Residual plot" src="https://github.com/user-attachments/assets/bde4d26e-1ac2-4dc0-b4fe-e791495d0672" />


#### What This Graph Shows

Residual analysis visualizes the difference between actual values and predicted values.

Residual = Actual Value - Predicted Value

#### Key Insights

* Points scattered randomly around zero indicate a good model fit.
* Helps detect prediction errors and model bias.
* Identifies whether the regression assumptions are satisfied.
* A random residual pattern suggests the model performs well.

Residual analysis is important for validating the reliability and performance of regression models.

---

# Installation Guide

## Clone Repository

```bash
git clone https://github.com/your-username/sales-prediction-ml.git
```

## Move Into Project Folder

```bash
cd sales-prediction-ml
```

## Create Virtual Environment

```bash
py -3.10 -m venv mlenv
```

## Activate Environment

```bash
.\mlenv\Scripts\Activate.ps1
```

## Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Run Jupyter Notebook

```bash
jupyter notebook
```

---

# Key Insights

* TV advertising has the highest impact on product sales.
* Radio advertising also contributes positively to sales performance.
* Newspaper advertising shows comparatively lower influence.
* Linear Regression effectively models the relationship between advertising budgets and sales.

---

# Future Improvements

This project can be further improved by:

* Implementing multiple regression models
* Using advanced algorithms such as Random Forest or XGBoost
* Building a Streamlit dashboard for real-time prediction
* Deploying the model as a web application
* Performing hyperparameter tuning for better accuracy

---

# Skills Demonstrated

This project demonstrates practical skills in:

* Data Analysis
* Data Visualization
* Machine Learning
* Predictive Modeling
* Feature Engineering
* Exploratory Data Analysis
* Python Programming

---

# Author

## Kiran

Machine Learning & Data Science Enthusiast

---

# GitHub Repository Description

Machine Learning project for predicting product sales using advertising data and Linear Regression with Python, Pandas, Seaborn, and Scikit-learn.
