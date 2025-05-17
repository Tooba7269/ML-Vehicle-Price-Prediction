# 🚗 Used Car Price Prediction using Machine Learning

### 👤 Author: Tooba Zahid  
A complete machine learning pipeline to predict used car prices based on structured advert data, including feature engineering, model tuning, evaluation, and comparison.

---

## 📦 Dataset

Due to size limitations, the dataset is not directly included in this repository.

- 🔗 [Google Sheets Link (Download as CSV)](https://docs.google.com/spreadsheets/d/1JOq6Is1VLsvQ_LwsqtPUqT3G-j_05k9XzwJSOO1wU4o/edit?usp=sharing)
- 🗜️ `adverts.csv.zip` file included for reference

Once downloaded, place `adverts.csv` in a folder called `data/`, or upload it directly to your Colab session.

```python
# For Google Colab:
from google.colab import files
uploaded = files.upload()
📁 Project Structure
python
Copy
Edit
ML-Vehicle-Price-Prediction/
├── mlp_code.py                     # Core Colab-exported code
├── adverts.csv.zip                 # Zipped dataset
├── ML-Vehicle-Price-Prediction.Report.pdf
├── README.md
🛠️ Tools & Libraries
Google Colab (Python)

pandas, numpy

matplotlib, seaborn

scikit-learn (models, evaluation, GridSearchCV)

category_encoders (hotencoding, Target Encoding)

🔬 Workflow Summary
1. 🧼 Data Preprocessing
Filled missing values using domain-aware logic (e.g., 2021 for "NEW" cars)

Removed outliers and errors in year_of_registration, price, mileage

2. 🏗️ Feature Engineering
One-hot encoding for low-cardinality fields: condition, fuel_type

Target encoding for high-cardinality: make, model, body_type, colour

Rescaling using MinMaxScaler (for numeric features)

3. 🔍 Modeling Approach
Models used:

Linear Regression

Decision Tree Regressor (tuned with GridSearchCV)

k-Nearest Neighbors (KNN)

Cross-validation used to avoid overfitting

Split: 80% train → 10% val + 10% test

📊 Model Performance
Model	               R² Score (Test)	 Mean Training R²	 Score Difference
Linear Regression	   0.7891	           0.7919	            0.0028
Decision Tree	       0.9325	           0.9333	            0.0008
KNN Regressor	       0.8880	           0.9111	            0.0231

✅ Best Model: Decision Tree Regressor (lowest error, least overfitting)
📉 KNN showed slight overfitting compared to others.

📈 Key Visualizations
Correlation heatmap of features

Price distribution (log scale)

Mileage vs Price (log-log scatter)

Residual plots and prediction accuracy

Feature importance from model coefficients

See code or notebook for charts and explanation.

▶️ How to Run in Google Colab
Open Google Colab

Upload mlp_code.py or paste into a new notebook

Upload the dataset via:

python
Copy
Edit
from google.colab import files
uploaded = files.upload()
Run each block in sequence to reproduce results

🔧 Optional Enhancements
Add SHAP for explainable ML

Deploy via Streamlit for interactive prediction

Explore ensemble models like XGBoost or Random Forest

🙋 About
This project was developed for academic coursework focused on real-world machine learning challenges. It demonstrates end-to-end model development, with emphasis on clean feature engineering, evaluation methodology, and visual insight.

Thank you for visiting!
