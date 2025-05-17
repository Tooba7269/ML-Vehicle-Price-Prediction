# 🚗 Used Car Price Prediction using Machine Learning

### 👤 Author: Tooba Zahid

A complete machine learning pipeline to predict used car prices based on structured advert data. Includes feature engineering, model tuning, cross-validation, and evaluation.

---

## 📦 Dataset

Due to file size limits, the dataset is shared externally:

- 🔗 [Google Sheets (Download as CSV)](https://docs.google.com/spreadsheets/d/1JOq6Is1VLsvQ_LwsqtPUqT3G-j_05k9XzwJSOO1wU4o/edit?usp=sharing)
- 🗜️ `adverts.csv.zip` — included in this repo

Once downloaded, extract and place `adverts.csv` in a folder named `data/`, or upload it directly to Colab:

```python
# For Google Colab
from google.colab import files
uploaded = files.upload()
📁 Project Structure
python
Copy
Edit
ML-Vehicle-Price-Prediction/
├── mlp_code.py                         # Colab-exported Python code
├── adverts.csv.zip                     # Zipped dataset
├── ML-Vehicle-Price-Prediction.Report.pdf
├── README.md
🛠️ Tools Used
Google Colab (Python 3.x)

pandas, numpy

matplotlib, seaborn

scikit-learn (models, GridSearchCV, metrics)

category_encoders (Target Encoding)

🔬 Workflow Summary
1. 🧼 Data Preprocessing
Filled missing values using domain logic (e.g., 2021 for "NEW" cars)

Removed outliers/errors in year_of_registration, mileage, and price

2. 🏗 Feature Engineering
One-Hot Encoding for: condition, fuel_type

Target Encoding for: make, model, body_type, colour

MinMax Scaling applied to numeric features

3. 🧠 Modeling
Trained 3 regression models:

Linear Regression

Decision Tree Regressor (tuned via GridSearchCV)

k-Nearest Neighbors Regressor

Applied Cross-validation to measure generalization

Performance tested on held-out test set

📊 Model Performance
Model	R² Score (Test)	Mean Training R²	Score Difference
Linear Regression	0.7891	0.7919	0.0028
Decision Tree	0.9325	0.9333	0.0008
KNN Regressor	0.8880	0.9111	0.0231

✅ Best Model: Decision Tree Regressor
📉 KNN showed some overfitting (training > test)

▶️ How to Run in Google Colab
Go to Google Colab

Upload mlp_code.py or paste it into a Colab notebook

Upload adverts.csv manually using:

python
Copy
Edit
from google.colab import files
uploaded = files.upload()
Run the cells to execute the full pipeline

🚀 Optional Improvements
Visualize SHAP values for explainability

Try ensemble models like Random Forest or XGBoost

Deploy the model with Streamlit or Gradio

🙋 About
This project was built to practice applied ML techniques with real-world structured data.
It demonstrates the full pipeline from raw data → clean features → trained model → evaluation and insight.

Thanks for visiting! ⭐
