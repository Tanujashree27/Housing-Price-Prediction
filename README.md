# 📊 Housing Price Prediction using Linear Regression

This project demonstrates a simple **Linear Regression** model to predict **median house values** based on **median income** using the California housing dataset.

## 🔍 Objective

To analyze the relationship between **median income** and **median house value**, and to evaluate how well a linear model performs with this single feature.

---

## 🗂️ Dataset

**File:** `housing.csv`
**Source:** California Housing dataset (can be obtained from Kaggle or similar sources)

**Features used:**

* `median_income` — Independent variable
* `median_house_value` — Dependent variable (target)

---

## 📈 Tools and Libraries

* **Pandas**: Data manipulation
* **Matplotlib**: Data visualization
* **Scikit-learn**: Machine learning model and evaluation
* **NumPy**: Numerical computations

---

## 🧠 Model Overview

```python
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X, y)
```

* Model is trained on a single feature: `median_income`
* Predicts `median_house_value`

---

## 📉 Visualization

A scatter plot shows actual data, and the red regression line indicates model predictions:

![Regression Plot](#) *(Run the script to generate and view this plot)*

---

## 📊 Evaluation Metrics

| Metric       | Value       | Interpretation                                 |
| ------------ | ----------- | ---------------------------------------------- |
| **MAE**      | \$62,625.93 | On average, predictions are off by \$62K       |
| **RMSE**     | \$83,733.57 | Larger errors have a higher impact             |
| **R² Score** | 0.4734      | \~47% of price variance is explained by income |

---

## 🧾 Interpretation

* **MAE**: Indicates the average absolute error between predicted and actual values
* **RMSE**: Emphasizes larger errors due to squaring
* **R² Score**: Shows a moderate linear relationship. Median income alone does not fully explain house prices, indicating the need for a multivariate model for better accuracy.

---

## 🚀 How to Run

1. Ensure Python is installed (`>=3.7`)
2. Install dependencies:

   ```bash
   pip install pandas matplotlib scikit-learn numpy
   ```
3. Place `housing.csv` in the same directory.
4. Run the script:

   ```bash
   python linear_regression_housing.py
   ```

---

## 📌 Future Improvements

* Use multiple features for multivariate regression.
* Handle outliers and scale features.
* Explore non-linear models for better accuracy.
