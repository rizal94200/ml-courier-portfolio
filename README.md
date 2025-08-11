# 📦 ML Courier SLA Prediction

[![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Completed-success.svg)]()

Machine Learning project for **courier SLA prediction** using EDA, feature engineering, and Random Forest model — complete with **business insights** and **recommendations**.

---

## 🚀 Project Overview
This project predicts whether courier deliveries will be **In SLA** or **Out of SLA** based on historical delivery data.

It includes:
- 🧹 **Data Cleaning & Preprocessing**
- 📊 **Exploratory Data Analysis (EDA)**
- ⚙️ **Feature Engineering**
- 🤖 **Model Training & Evaluation** (Random Forest)
- 💡 **Insights & Business Recommendations**

---
## 📂 Dataset
All datasets are stored in the [`data/`](data/) folder:

| File Name | Description |
|-----------|-------------|
| `courier_dim.csv` | Courier master data |
| `customer_dim.csv` | Customer master data |
| `location_dim.csv` | Location master data |
| `order_fact.csv` | Main order transaction data |
| `features_for_model.csv` | Processed features used for ML model |


---


## 📂 Project Structure
notebooks/
├── 01_EDA.ipynb
├── 02_Feature_Engineering.ipynb
├── 03_Model_Training.ipynb
requirements.txt
.gitignore

---


🧠 Machine Learning Models
1. Logistic Regression
ROC AUC: 0.85 (example value, replace with your actual result)
Strengths: Simple, fast, and easy to interpret.
Limitations: Less effective for capturing complex non-linear relationships.

2. Random Forest
ROC AUC: 0.92 (example value, replace with your actual result)
Strengths: Handles non-linear relationships and interactions between features well.
Limitations: Less interpretable compared to Logistic Regression.

🔍 Top 5 Important Features (Random Forest)
Delivery distance
Courier average SLA performance
Package weight
Origin province
Destination province



---

## ⚙️ Installation
1. **Clone the repository**
   ```bash
   git clone https://github.com/rizal94200/ml-courier-portfolio.git
   cd ml-courier-portfolio
2. Create virtual environment (optional but recommended)
   python -m venv .venv
  source .venv/bin/activate  # MacOS/Linux
  .venv\Scripts\activate     # Windows
3. Install dependencies
   pip install -r requirements.txt

▶️ How to Run
Open Jupyter Notebook or VS Code.
Run the notebooks in order:
01_EDA.ipynb
02_Feature_Engineering.ipynb
03_Model_Training.ipynb
Check model performance metrics and generated insights.


📌 Key Insights
🚚 Courier performance varies significantly between logistic partners.
🌍 Geographic origin & destination strongly impact SLA performance.
🏢 Customer company patterns influence delivery timelines.
💼 Recommendations focus on partner selection & operational efficiency.


📜 License
This project is licensed under the MIT License — feel free to use and adapt it.


🌟 Future Improvements
Try alternative ML models (XGBoost, LightGBM)
Deploy as API or web dashboard
Real-time SLA prediction integration

✉️ Author: Syamsul Rizal
📌 GitHub: rizal94200




## 📊 Exploratory Data Analysis (EDA)

![Delivery SLA Distribution](image/Delivery%20SLA%20Distribution.png)  
![Top 10 Logistics Providers](image/Top%2010%20Logistics%20Providers.png)  
![Top 10 Service Type](image/Top%2010%20Service%20Type.png)  

---

## 📈 Model Performance

![Logistic Regression - ROC curve](image/Logistic%20Regression%20-%20ROC%20curve.png)  
![Logistic Regression - Confusion Matrix](image/Logistic%20Regression-Confusion%20Matrix.png)  
![Permutation Importance (TOP 15) - Original Features](image/Permutation%20Importance%20(TOP%2015)%20-%20Original%20Features.png)  
![Random Forest - Confussion Matrix](image/Random%20Forest%20-%20Confussion%20Matrix.png)  
![Random Forest - ROC Curve](image/Random%20Forest%20-%20ROC%20Curve.png)  



