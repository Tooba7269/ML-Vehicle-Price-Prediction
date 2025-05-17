🚗 Vehicle Price Prediction using Machine Learning

Welcome to the repository for my Machine Learning coursework project for **Unit 6G7V0015 – Machine Learning Concepts** at MMU. This end-to-end solution tackles a **real-world regression task**: predicting the selling price of vehicles based on historical car advertisement data provided by **AutoTrader**.

---

## 📁 Project Structure

├── mlp_code.py # Complete ML pipeline (Python script version)
├── adverts.csv.zip # Zipped dataset (large size; alternative access provided)
├── report.pdf # Final structured coursework report
├── README.md # You're here!

yaml
Copy
Edit

---

## 📊 Project Overview

### 🎯 Objective
Develop, evaluate, and compare predictive models for vehicle pricing using historical ad data. The task simulates the work of machine learning engineers at AutoTrader, enhancing user pricing transparency.

### 🧠 Techniques Used
- **Exploratory Data Analysis (EDA)**
- **Feature Engineering & Encoding**
- **Data Cleaning & Outlier Handling**
- **Model Training & Tuning**
- **Validation, Testing, & Residual Analysis**
- **Model Comparison & Feature Importance**

---

## 🔍 Dataset Description

- ~400,000 anonymized car adverts
- Key features: `make`, `model`, `mileage`, `fuel type`, `year of registration`, `vehicle condition`, `price`, etc.
- Available via:
  - ✅ [Google Sheet Backup](https://docs.google.com/spreadsheets/d/1JOq6Is1VLsvQ_LwsqtPUqT3G-j_05k9XzwJSOO1wU4o/edit?usp=sharing)
  - ✅ `adverts.csv.zip` file (in repo)

> **Disclaimer:** This dataset is licensed for academic use **only** as part of the MMU coursework. Do not redistribute.

---

## 🧪 Models Implemented

| Model               | Techniques Used                        | Tools & Metrics |
|--------------------|-----------------------------------------|-----------------|
| 📈 Linear Regression | Feature scaling, residuals analysis     | R², MAE, MSE     |
| 🌲 Decision Tree     | GridSearchCV tuning, feature importance | R², MAE, MSE     |
| 🤖 K-Nearest Neighbors | Distance-based, sampling optimization   | R², MAE, MSE     |

✅ All models are evaluated on **training**, **validation**, and **test sets**, with CV analysis included.

---

## 📉 Results Summary

- **Best performance**: Decision Tree with tuned hyperparameters
- Included:
  - Actual vs Predicted plots
  - Residual distributions
  - Feature importances (tree & regression coefficients)
  - Visual model comparison using bar and line plots

---

## 🛠 Tech Stack

- `Python 3.10+`
- `Pandas`, `NumPy`, `Seaborn`, `Matplotlib`
- `Scikit-Learn`, `category_encoders`
- Google Colab / Jupyter Notebook

---

## 📎 How to Reproduce

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/vehicle-price-prediction.git
   cd vehicle-price-prediction
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Load the notebook or run mlp_code.py:

bash
Copy
Edit
python mlp_code.py
⚠️ Note: If using Google Colab, ensure you mount your Drive and place adverts.csv appropriately.

📚 Report & Evaluation
The full PDF report is included in this repo, containing:

Code snippets + outputs

Explanations per spec requirement

Model evaluation

Visualizations

Reflections
