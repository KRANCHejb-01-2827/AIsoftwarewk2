# 🌱 SDG 13: Climate Action — AI Model for Predicting CO₂ Emissions

### 🚗 Project Overview
This project supports **United Nations SDG 13: Climate Action** by using **machine learning** to predict CO₂ emissions from vehicle specifications.  
It demonstrates how AI can guide policymakers, manufacturers, and consumers toward more sustainable choices and reduce carbon footprints globally.

---

### 🧠 Objective
To build a **supervised learning model** that predicts **CO₂ emissions (g/km)** based on vehicle attributes like engine size, fuel type, and fuel consumption rates.

---

### 🧰 Tools & Technologies
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Joblib
- **Environment:** Google Colab / Jupyter Notebook
- **Dataset:** CO2_Emissions.csv (from Government of Canada Open Data)

---

### ⚙️ Workflow
1. **Data Loading & Cleaning**
   - Loaded the dataset and checked for missing or inconsistent data.
2. **Feature Selection**
   - Selected relevant numerical features:
     - `Engine Size(L)`, `Cylinders`,  
       `Fuel Consumption City (L/100 km)`,  
       `Fuel Consumption Hwy (L/100 km)`,  
       `Fuel Consumption Comb (L/100 km)`
3. **Model Training**
   - Compared two models:
     - **Linear Regression**
     - **Random Forest Regressor**
4. **Evaluation Metrics**
   - Mean Absolute Error (MAE)
   - Mean Squared Error (MSE)
   - R² Score

---

### 📊 Results
| Model | MAE | MSE | R² |
|-------|------|------|------|
| Linear Regression | 13.51 | 421.86 | 0.8774 |
| Random Forest | **3.22** | **84.16** | **0.9755** |

✅ The **Random Forest** model outperformed Linear Regression and achieved high prediction accuracy.

---

### 🔍 Key Insights
- Engine size and combined fuel consumption are the top predictors of CO₂ output.  
- Petrol vehicles emit significantly more CO₂ than hybrid or electric options.  
- ML models can help develop **data-driven environmental policies**.

---

### 🧮 Live Prediction Demo
Users can input:


Engine Size(L): 3.5
Cylinders: 6
Fuel Consumption Comb (L/100 km): 10.5
Fuel Consumption Comb (mpg): 27

The model predicts approximate **CO₂ Emissions (g/km)** instantly.

---

### 🌐 Ethical Reflection
Bias in data can influence model predictions if underrepresented vehicle types (e.g., hybrids) are limited.  
Our model encourages sustainable mobility by highlighting **carbon-efficient technologies** and **policy-driven emission reduction**.

---

### 📁 Repository Structure


📂 CO2_Emissions_Project/
│── CO2_Emissions.csv
│── co2_model.py
│── visuals/
│ ├── actual_vs_predicted.png
│ ├── feature_importance.png
│── README.md
│── requirements.txt


---

### 👩🏽‍💻 Contributors
- **Francis Gachoki Karimi**
- PLP Academy — Machine Learning & AI Cohort 2025

---

### 📣 Quote
> “AI can be the bridge between innovation and sustainability.” — UN Tech Envoy
