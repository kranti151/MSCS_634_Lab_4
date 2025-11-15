# Regression Analysis Lab (MSCS 634)

## Overview

This lab explores a variety of regression techniques using the **Diabetes Dataset** from `sklearn`. The goal is to understand how different regression models behave, how regularization improves model generalization, and how to properly evaluate model performance using common metrics.

You will implement:

* Simple Linear Regression
* Multiple Linear Regression
* Polynomial Regression
* Ridge Regression
* Lasso Regression

The lab also walks through training/testing, visual interpretation, and comparing model performance.

---

## Purpose of This Lab

The purpose of this lab is to help you:

* Build intuition around different regression approaches.
* Understand the balance between **underfitting vs overfitting**.
* See how **regularization (Ridge/Lasso)** stabilizes models.
* Practice evaluation using **MAE**, **MSE**, **RMSE**, and **R²**.
* Strengthen your data science workflow from preprocessing to visualization.

---

## 📊 Key Insights Gained

### **1. Linear Regression Behavior**

* Simple Linear Regression performs decently but is limited because health outcomes often depend on multiple factors.
* With only one feature, the model is more prone to bias and underfitting.

### **2. Multiple Regression Improvements**

* Using all features provides a more realistic representation of the dataset.
* Performance improves significantly compared to simple linear regression.

### **3. Polynomial Regression**

* Adding polynomial features captures nonlinear patterns.
* Low-degree polynomials may improve accuracy; however, **higher degrees can lead to strong overfitting**.

### **4. Regularization (Ridge & Lasso)**

* Ridge reduces the impact of large coefficients, making the model more stable.
* Lasso can shrink some coefficients to zero, helping with feature selection.
* Regularization especially helps when polynomial features increase model complexity.

### **5. Model Comparison**

* Simple Linear Regression → high bias, lower accuracy.
* Multiple Regression → more accurate and balanced.
* Polynomial Regression → good fit at low degree but risky at high degree.
* Ridge Regression → best stability and generalization.
* Lasso Regression → helpful for identifying key features.

In general, **Ridge usually gives the most balanced performance for the Diabetes dataset**.

---

##  Challenges Encountered

* Choosing the right polynomial degree required experimentation.
* Regularization strength (`alpha`) needed tuning to balance bias and variance.
* Visualization of high-degree polynomials can become messy and misleading.

---

## Repository Contents

Your GitHub repository should include:

* `Lab4_Regression.ipynb` – All code, visualizations, and explanations.
* `README.md` – This summary document.

---

## How to Run

1. Open the notebook in Google Colab or Jupyter.
2. Install any missing libraries (if necessary).
3. Run cells in order to reproduce the full analysis.

---

## Final Notes

This lab provides a strong foundation in regression modeling. By comparing simple, multiple, polynomial, and regularized models, you get a clear sense of how model complexity and regularization affect real-world prediction accuracy.

If you continue exploring machine learning, this workflow becomes the backbone for more complex models in future assignments.
