# 🌍 CO₂ Emission Reduction Prediction using Machine Learning

## 📌 Overview

This project develops machine learning models to predict **monthly CO₂ emission reductions (in tons)** based on organisational sustainability, financial, and operational factors.
The objective is to identify key drivers of emission reduction and support **data-driven sustainability decision-making**.

---

## 📊 Dataset

* Features include:

  * Sustainability Budget
  * Renewable Energy Usage (%)
  * Green Certification (binary)
  * Sustainable Suppliers (%)
  * Employee Training Hours
  * Waste Recycled (%)
  * Company Size, Revenue, Profit Margin
  * Temporal variable (Month)
* Target variable:

  * **CO2_Reduction_Tons**

---

## ⚙️ Methodology

### Data Preprocessing

* Missing value handling using **mean and mode imputation**
* Categorical encoding using **One-Hot Encoding**
* Feature selection using:

  * **Correlation analysis**
  * **ANOVA testing**
* Train-test split: **80% training / 20% testing**
* Feature scaling applied for models sensitive to scale (e.g., SVR)

---

## 🤖 Models Implemented

* Multiple Linear Regression
* Support Vector Regression (SVR)
* Decision Tree Regressor
* Random Forest Regressor

---

## 📈 Model Performance

| Model                  | R² Score | MSE   |
| ---------------------- | -------- | ----- |
| Linear Regression      | 0.77     | 26.20 |
| Random Forest          | 0.66     | 40.27 |
| Support Vector Machine | 0.49     | 60.48 |
| Decision Tree          | 0.41     | 69.76 |

✅ **Best Model:** Linear Regression

* Achieved highest R² and lowest prediction error
* Indicates strong linear relationships between sustainability inputs and CO₂ reduction outcomes

---

## 🔍 Key Insights

* **Sustainability budget** and **renewable energy usage** are strong predictors of emission reduction
* Simpler models (Linear Regression) outperformed complex models, suggesting **dominant linear relationships in the dataset**
* Feature selection (ANOVA) helped remove weak predictors, improving model efficiency

---

## 💼 Business Impact

* Enables organisations to **optimise sustainability investments**
* Helps identify **high-impact actions** for reducing emissions
* Supports **ESG strategy and regulatory compliance planning**
* Provides a predictive framework for **forecasting environmental performance**

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn
* SciPy

---

## 📂 Project Structure

```
├── notebooks/
│   └── co2_emission_prediction.ipynb
├── data/
├── images/
├── README.md
├── requirements.txt
```

---

## 🚀 Future Improvements

* Apply **advanced models (Gradient Boosting, XGBoost)**
* Explore **non-linear feature interactions**
* Deploy as a **Streamlit web application**
* Validate results on **external datasets**

---

## 👤 Author

MSc Business Analytics Student
University of Greenwich
