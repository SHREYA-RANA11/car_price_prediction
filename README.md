# Car Price Prediction using Machine Learning

## Project Overview

This project predicts car prices using Machine Learning techniques.  
The dataset contains information about different cars such as:

- Model
- Year
- Mileage
- Transmission Type
- Fuel Type
- Engine Size
- MPG
- Tax

The goal of this project is to build a regression model that can accurately predict car prices and compare different encoding techniques.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

 Machine Learning Workflow

 1. Data Collection
- Imported dataset using Pandas.

 2. Data Cleaning
- Checked null values
- Removed unnecessary data
- Handled categorical columns

 3. Exploratory Data Analysis (EDA)
- Visualized distributions
- Checked correlations
- Detected outliers

 4. Feature Engineering
- Created useful features
- Applied Label Encoding on categorical columns
- Applied One-Hot Encoding for comparison
- Compared the performance of both encoding techniques

 5. Data Preprocessing
- Applied StandardScaler on numerical columns:
  - year
  - mileage
  - tax
  - mpg
  - engineSize
- Performed Train-Test Split

6. Outlier Handling
- Detected and removed outliers using the IQR method.

 7. Model Training
Models used:
- Linear Regression
- Random Forest Regressor

 8. Model Evaluation
Evaluation metrics:
- R² Score
- Adjusted R² Score

---

## Results

| Encoding Method | Accuracy (R² Score) |
|-----------------|--------------------|
| Label Encoding | 73% |
| One-Hot Encoding | 83% |

### Observations
- One-Hot Encoding performed better than Label Encoding.
- Outlier removal slightly improved model performance.
- Random Forest performed better than Linear Regression.

---

## Key Learnings

- One-Hot Encoding works better for categorical data in regression problems.
- Label Encoding may create false numerical relationships between categories.
- Outliers can negatively affect model performance.
- Feature engineering and preprocessing improve accuracy.
- Random Forest handles complex relationships better than Linear Regression.

---
## Dataset

Dataset Source: Kaggle

Link: https://www.kaggle.com/datasets/adhurimquku/ford-car-price-prediction

## Project Structure

```bash
car-price-prediction/
│
├── car_price_prediction.ipynb
├── README.md

