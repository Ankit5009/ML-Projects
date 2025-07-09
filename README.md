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
