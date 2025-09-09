# 🚔 Predicting Crime Rates with Machine Learning 📊  

A **data-driven approach** to predict the rate of violent crimes per capita in U.S. communities.  
This project leverages **socio-economic, law enforcement, and crime data**, applying **Principal Component Analysis (PCA)** for feature reduction and a **Random Forest Regressor** for predictions.  

---

## ✨ Key Features  
📈 **Data Preprocessing** – Handles missing values and prepares the dataset for modeling.  
🔬 **PCA for Feature Reduction** – Reduces dimensionality while preserving variance.  
🤖 **Machine Learning Model** – RandomForestRegressor predicts `ViolentCrimesPerPop`.  
📊 **Performance Evaluation** – Uses **MSE** and **R² Score** for accuracy.  
🔍 **Feature Importance** – Highlights top socio-economic predictors of crime.  

---
├── communities_and_crime.csv # Raw dataset
├── project.ipynb # Notebook with preprocessing, PCA & model training
└── README.md # Project documentation


---

## 🚀 Getting Started  

1️⃣ **Clone the repository**  
```bash
git clone https://github.com/Sanjaysk17/crime-prediction-project.git
cd crime-prediction-project

⚙️ Methodology

Data Cleaning – Replace "?" with NaN, impute with column means.

Feature Scaling – Standardize features with StandardScaler.

PCA – Reduce dimensionality, retain components with most variance.

Model Training – Train RandomForestRegressor on PCA-transformed data.

Evaluation – Assess using MSE and R² score.

📈 Results & Performance

Mean Squared Error (MSE): 0.015

R² Score: 0.65

✅ Model explains ~65% of the variance in violent crime rates while reducing complexity.

🔑 Top Predictive Factors (from PCA components)

Poverty & Income → PctPopUnderPov, perCapInc

Population & Housing → PersPerOccupHous, PctPersDenseHous

Family Structure → PctKids2Par, MalePctDivorce

Education → PctBSorMore, PctNotHSGrad

Racial Demographics → racepctblack, racePctWhite

📌 See PCA analysis in project.ipynb for details.
