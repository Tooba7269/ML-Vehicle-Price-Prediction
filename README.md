# 🚗 Car Price Prediction Using Machine Learning

### 👤 By Tooba Zahid

This project demonstrates an end-to-end machine learning pipeline to predict used car prices based on structured automotive listing data. It covers data preprocessing, feature engineering, model selection, evaluation, and visual analysis.

---

## 📦 Dataset Access

The dataset used in this project is available in two formats:

- 🔗 [View on Google Sheets](https://docs.google.com/spreadsheets/d/1JOq6Is1VLsvQ_LwsqtPUqT3G-j_05k9XzwJSOO1wU4o/edit?usp=sharing)  
  *(Download as CSV: File → Download → .csv)*

- 🗜️ `adverts.csv.zip` — included in this GitHub repository

➡️ After downloading, place `adverts.csv` into a `data/` folder on your Google Drive, or upload it directly to your Colab session.

In code:
```python
from google.colab import files
uploaded = files.upload()

📁 Project Structure
bash
Copy
Edit
ML-Vehicle-Price-Prediction/
├── data/ (optional — upload in Colab instead)
├── mlp_code.py                 # Python script
├── README.md                   # This file
├── ML-Vehicle-Price-Prediction.Report.pdf
🛠️ Tools Used
Google Colab (Python)

pandas, numpy

matplotlib, seaborn

scikit-learn

category_encoders

🔬 Workflow Overview
Load and explore the dataset

Clean and preprocess data

Encode categorical features (OHE + Target Encoding)

Split into training, validation, and test sets

Train models:

Linear Regression

Decision Tree Regressor (with GridSearchCV)

k-Nearest Neighbors

Evaluate model performance (R², MAE, MSE)

Visualize and compare results

📊 Sample Results
Model	R² (Test)	MAE	MSE
Linear Regression	~0.67	~2100	~1.8M
Decision Tree	~0.70	~1800	~1.5M
KNN Regressor	~0.65	~2300	~2.0M

✅ Best Performing Model: Decision Tree Regressor (tuned with GridSearchCV)

▶️ How to Run in Google Colab
Go to Google Colab

Click File → Upload Notebook

Upload your .ipynb or .py file

Upload the adverts.csv file using:

python
Copy
Edit
from google.colab import files
uploaded = files.upload()
Run the code cells in sequence

🚀 Future Improvements
Convert into an interactive web app with Streamlit or Gradio

Try ensemble models (Random Forest, XGBoost)

Add visual explainability (e.g., SHAP)

🙋‍♀️ About the Author
I'm Tooba Zahid, exploring real-world data problems and applying practical machine learning techniques.
This project showcases the full ML lifecycle — from raw data to results and evaluation — using Google Colab.

Thanks for visiting!
