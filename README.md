# 🛳️ Titanic: Survival Prediction & Model Optimization
**Machine Learning | Ensemble Methods | Overfitting Analysis**

## 📌 Project Overview
This project uses the classic Titanic dataset to predict passenger survival. Beyond basic classification, the primary goal of this repository was to demonstrate the **transition from an overfitted model to a generalized one** using advanced ensemble techniques.

## 🛠️ The Engineering Process
### 1. Data Wrangling & Feature Engineering
* **Missing Value Imputation:** Strategically filled missing `Age` values using the median and `Embarked` using the mode.
* **Feature Encoding:** Transformed categorical variables (Sex, Embarked) into numerical formats for model compatibility.
* **Feature Selection:** Analyzed correlations to prioritize `Pclass`, `Sex`, and `Fare` as primary survival predictors.

### 2. Addressing Overfitting
Initially, a baseline **Random Forest** model was used, which achieved 100% accuracy on training data but failed on the test set. To fix this, I implemented:
* **XGBoost (Extreme Gradient Boosting):** Leveraged boosting to reduce bias and variance.
* **Regularization:** Applied `reg_alpha` and `reg_lambda` to penalize complex models.
* **Hyperparameter Tuning:** Limited `max_depth` to prevent the model from "memorizing" the noise in the data.



## 📊 Key Results
* **Training Accuracy:** Optimized to a realistic level (approx. 85-89%).
* **Test Accuracy:** Improved significantly by reducing the "Generalization Gap."
* **Most Influential Feature:** `Sex` and `Fare` were the strongest indicators of survival.


*Note: The dataset is sourced from the Kaggle Titanic Challenge.*
