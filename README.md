# 🏡 House Price Prediction using Linear Regression

This project demonstrates how to predict house prices using linear regression. It includes data exploration, visualization, training, and evaluation using a real-world dataset.

---

## 📁 Dataset

- **File Used:** `USA_Housing.csv`
- **Rows:** 5000
- **Columns:**
  - Avg. Area Income  
  - Avg. Area House Age  
  - Avg. Area Number of Rooms  
  - Avg. Area Number of Bedrooms  
  - Area Population  
  - Price (Target Variable)  
  - Address (Dropped during modeling)

---

## 📦 Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn import metrics


## 📊 Exploratory Data Analysis

- Viewed first 5 rows and structure of the dataset using `data.head()` and `data.info()`
- Summary statistics using `data.describe()`

### 🔍 Visualizations

- ✅ Pairplot to see relationships between variables
- ✅ Correlation heatmap to examine multicollinearity
- ✅ Scatter plot: Avg. Area Income vs Price

---

## ⚙️ Model Building

- Dropped `Address` column (non-numeric)
- **Features Used:** All except `Price` (target) and `Address`
- **Data Split:**
  - Training set: 70%
  - Testing set: 30%
- **Model Used:** `LinearRegression` from `scikit-learn`

---

## 📈 Model Coefficients

| Feature                       | Coefficient     |
|------------------------------|-----------------|
| Avg. Area Income             | 21.64           |
| Avg. Area House Age          | 165729.21       |
| Avg. Area Number of Rooms    | 120958.35       |
| Avg. Area Number of Bedrooms | 1949.09         |
| Area Population              | 15.23           |

**Intercept:** `-2,645,289.86`

---

## 🧪 Model Evaluation

| Metric                         | Value            |
|--------------------------------|------------------|
| MAE (Mean Absolute Error)      | 82,746           |
| MSE (Mean Squared Error)       | 10,567,448,570   |
| RMSE (Root Mean Squared Error) | 102,798          |

---

## 📉 Prediction Result

- ✅ Compared actual vs predicted house prices
- ✅ Plotted both for visual comparison
- ✅ Observed low residual error and good fit

---

## ✅ How to Run

1. **Clone this repository:**
   ```bash
   git clone https://github.com/Ankit5009/ML-Projects.git
   cd ML-Projects

