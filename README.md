# Samsung Sales Prediction Using Machine Learning

## 1. Project Overview

This project focuses on analyzing Samsung smartphone sales data and predicting the number of units sold using Machine Learning techniques.

The main objective is to understand sales-related factors such as revenue, region, market share, 5G capability, product models, and year to predict smartphone sales.

## 2. Project Objectives

- Analyze Samsung smartphone sales data.
- Understand the relationship between sales and other features.
- Check and handle missing values.
- Clean and preprocess the dataset.
- Convert categorical data into numerical format.
- Apply feature scaling.
- Build a Machine Learning model to predict units sold.
- Evaluate model performance using evaluation metrics.

## 3. Dataset Information

The dataset contains 1,000 records and 12 columns.

### Dataset Columns

| Column Name | Description |
|---|---|
| Year | Sales year |
| Quarter | Sales quarter |
| Product Model | Samsung smartphone model |
| 5G Capability | 5G availability |
| Units Sold | Number of units sold |
| Revenue ($) | Total revenue |
| Market Share (%) | Market share percentage |
| Regional 5G Coverage (%) | Regional 5G coverage |
| 5G Subscribers (millions) | Number of 5G subscribers |
| Avg 5G Speed (Mbps) | Average 5G speed |
| Preference for 5G (%) | Customer preference for 5G |
| Region | Sales region |

## 4. Tools and Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

## 5. Project Workflow

### Step 1: Data Loading
Loaded the Samsung sales dataset using Pandas.

### Step 2: Data Cleaning
- Checked the dataset using `head()`.
- Checked minimum and maximum units sold.
- Checked missing values using `isnull().sum()`.
- Selected relevant columns for model building.

**Missing Values:** No missing values were found in the dataset.

### Step 3: Feature Selection

Selected the following columns:

- Year
- Units Sold
- Revenue ($)
- Region
- Market Share (%)
- 5G Capability
- Product Model

### Step 4: Data Encoding

Used `LabelEncoder` from Scikit-learn to convert categorical columns into numerical values.

Columns encoded:
- Region
- 5G Capability
- Product Model

### Step 5: Feature and Target Selection

**Target Variable (Y):**
- Units Sold

**Features (X):**
- Year
- Revenue ($)
- Region
- Market Share (%)
- 5G Capability
- Product Model

### Step 6: Train-Test Split

Used `train_test_split()` to divide the dataset:

- Training Data: 80% (800 records)
- Testing Data: 20% (200 records)

Used `random_state=42` for reproducibility.

### Step 7: Feature Scaling

Applied `StandardScaler` to scale the training and testing features.

- `fit_transform()` was applied to training data.
- `transform()` was applied to testing data.

### Step 8: Model Building

Used **Linear Regression**, a supervised Machine Learning algorithm, because the target variable (Units Sold) is numerical.

Trained the model using the training dataset and generated predictions on the testing dataset.

## 6. Model Evaluation

The model was evaluated using two performance metrics.

| Evaluation Metric | Score |
|---|---:|
| R² Score | 0.11 |
| Mean Squared Error (MSE) | 234,632,333.27 |

### Performance Analysis

- **R² Score: 0.11** – The model explains approximately 11% of the variation in units sold on the test data.
- **Mean Squared Error: 234,632,333.27** – This represents the average squared difference between actual and predicted sales values.

The current model has limited predictive performance and can be improved through better feature selection, feature engineering, and model experimentation.

## 7. Conclusion

This project demonstrates the use of Python and Machine Learning for Samsung smartphone sales prediction.

The dataset was explored, missing values were checked, relevant features were selected, categorical variables were encoded, and feature scaling was applied.

A Linear Regression model was trained to predict the number of units sold.

The model achieved an R² score of 0.11. This indicates that there is scope for further improvement in prediction accuracy.

## 8. Author

**Tiya Khuar**
GitHub: [@tiyakhuar11-creator](https://github.com/tiyakhuar11-creator)
