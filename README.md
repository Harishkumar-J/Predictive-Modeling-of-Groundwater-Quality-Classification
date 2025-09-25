# 🌊 Groundwater Quality Prediction & Risk Assessment (India)

# Project Timeline

- **Project Name:** Groundwater Quality Classification and Risk Assessment  
- **Duration:** 01 July 2024 → 13 September 2024 (~10 weeks)  
- **Role:** Student Researcher (Self-initiated Academic Project)  
- **Location:** UK (MSc Data Science dissertation)  
- **Outcome:** Machine learning framework for groundwater risk classification with 97.13% accuracy (XGBoost).
- **Code Link:** https://colab.research.google.com/github/Harishkumar-J/Predictive-Modeling-of-Groundwater-Quality-Classification/blob/main/Project_Code_(ground_water).ipynb

This is an academic/portfolio repository. It documents **learning, roles, and process**.  
No proprietary or sensitive data/IP is included.

## 🚀 Overview
This project applies **machine learning** to classify and predict groundwater quality across India, using key parameters:

- **pH**
- **Temperature**
- **Conductivity**

Also developed a **risk scoring framework** (Water Quality Index – WQI) to categorize water into:

- Excellent  
- Good  
- Moderate  
- Poor  

The study compares **Logistic Regression, Support Vector Machine (SVM), Random Forest, and XGBoost**, with **XGBoost achieving the highest accuracy of 97.1%**.

---

## 📂 Project Structure
├── Project Code (ground water).ipynb # Jupyter notebook (EDA → Models → Evaluation)

├── GROUND.csv # Groundwater dataset (2012–2021, CPCB India)

├── states_india.geojson # Geospatial file for state-wise mapping

├── images/ # Exported charts/plots for README

└── README.md # Project documentation


---

## 🔎 Key Steps

### 1. Data Cleaning
- Removed rows with missing or inconsistent values (reduced dataset from 7872 to 7043 rows).  
- Standardized state names, handled duplicates.  
- Imputed missing values using **state + year medians** for pH, temperature, conductivity.  
- Outliers capped using domain knowledge (pH trimmed to 6–9; conductivity capped).  

### 2. Feature Engineering
- Computed **average pH, temperature, conductivity** per station.  
- Derived **Water Quality Index (WQI)** to simplify classification.  
- Encoded categorical state column via one-hot encoding.  

### 3. Geospatial Integration
- Merged dataset with **states_india.geojson**.  
- Built choropleth maps showing groundwater quality distribution across Indian states.  

### 4. Modeling
- **Logistic Regression** → 87.7% accuracy  
- **SVM (RBF kernel)** → 88.8% accuracy  
- **Random Forest** → 96.3% accuracy  
- **XGBoost** → 97.1% accuracy (best model)  

---

## 📊 Results

| Model               | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 87.7%    | 0.88      | 0.88   | 0.88     |
| SVM (RBF)           | 88.8%    | 0.89      | 0.88   | 0.88     |
| Random Forest       | 96.3%    | 0.96      | 0.96   | 0.96     |
| XGBoost             | 97.1%    | 0.97      | 0.97   | 0.97     |

➡️ **XGBoost consistently outperformed other models, especially for “Moderate” and “Poor” water quality classes.**

---

## 📸 Visual Insights


- Confusion matrix - logistic Regression
<p align="center">
  <img src="https://github.com/Harishkumar-J/Predictive-Modeling-of-Groundwater-Quality-Classification/blob/0505b8b044240e33cd8b447888b51421ea5726d8/CM%20-%20Log%20Reg.png" width="500"/>
</p>

- Heat Map - SVM
<p align="center">
  <img src="https://github.com/Harishkumar-J/Predictive-Modeling-of-Groundwater-Quality-Classification/blob/0e589b32b703a23447f1a007a28a0819e8276cc4/SVM-%20heatMap.png" alt="XGBoost Confusion Matrix"/>
</p>

- Precision-Recall curves (Random Forest & XGBoost)  

<p align="center">
  <img src="https://github.com/Harishkumar-J/Predictive-Modeling-of-Groundwater-Quality-Classification/blob/f607ef91ef006a6293df48fd2777d1b3f11d19b8/precision-recallCurve%20.png" width="500" alt="XGBoost Confusion Matrix"/>
</p>

- Choropleth maps of groundwater quality across India  
<p align="center">
  <img src="https://github.com/Harishkumar-J/Predictive-Modeling-of-Groundwater-Quality-Classification/blob/566801ed4133d2fecd590c58f3977b3703ae7ac4/Water%20Quality%20of%20States%20in%20India.png" width="500"/>
</p>

## 🛠️ Tech Stack

- Python (pandas, numpy, scikit-learn, xgboost)
- Matplotlib & Seaborn (visualization)
- GeoPandas & Folium (geospatial mapping)
- Jupyter Notebook
---

## 🚀 Quickstart

Clone the repo and set up environment:

# clone repo
git clone https://github.com/Harishkumar-J/Predictive-Modeling-of-Groundwater-Quality-Classification.git

# install dependencies
pip install -r requirements.txt

# run notebook
jupyter notebook "Project Code.ipynb"
