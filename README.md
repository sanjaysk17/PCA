🚔 Predicting Crime Rates with Machine Learning 📊

A data-driven approach to predict violent crime rates per capita in U.S. communities.

This project leverages socio-economic, law enforcement, and crime data, applying Principal Component Analysis (PCA) for feature reduction and a Random Forest Regressor for predictive modeling.

✨ Key Features

📈 Data Preprocessing: Handles missing values and prepares the dataset for modeling.

🔬 PCA for Feature Reduction: Identifies influential factors, reducing dimensionality while preserving variance.

🤖 Machine Learning Model: Uses RandomForestRegressor to predict ViolentCrimesPerPop.

📊 Performance Evaluation: Assessed with Mean Squared Error (MSE) and R² Score.

🔍 Feature Importance: Highlights socio-economic indicators most predictive of crime.

🛠️ Tech Stack

Python

Pandas & NumPy → Data manipulation

Scikit-learn → PCA & machine learning

Matplotlib & Seaborn → Data visualization

Jupyter Notebook → Exploratory analysis

📂 Project Structure
├── communities_and_crime.csv   # Raw dataset
├── project.ipynb               # Jupyter Notebook with EDA, PCA, and model training
└── README.md                   # Project documentation

🚀 Getting Started
1️⃣ Clone the repository
git clone <your-repo-link>
cd crime-prediction-project

2️⃣ Install dependencies
pip install pandas numpy scikit-learn matplotlib seaborn jupyter

3️⃣ Launch Jupyter Notebook
jupyter notebook


Then open project.ipynb to explore the code.

⚙️ Methodology

Data Loading & Cleaning

Load Communities and Crime dataset.

Replace ? with NaN, then impute with column mean.

Feature Scaling

Standardize features with StandardScaler.

Principal Component Analysis (PCA)

Apply PCA to reduce dimensionality.

Choose components based on explained variance ratio.

Model Training

Train RandomForestRegressor on top principal components.

Evaluation

Evaluate with MSE and R² score.

📈 Results & Performance

Mean Squared Error (MSE): 0.015

R² Score: 0.65

➡️ The model explains ~65% of the variance in violent crime rates.

🔑 Top Predictive Factors

Although PCA transforms features, the most influential underlying factors are:

Poverty & Income → PctPopUnderPov, perCapInc

Population & Housing → PersPerOccupHous, PctPersDenseHous

Family Structure → PctKids2Par, MalePctDivorce

Education → PctBSorMore, PctNotHSGrad

Race Demographics → racepctblack, racePctWhite

📌 Future Improvements

Test Gradient Boosting and XGBoost for higher accuracy.

Hyperparameter tuning with GridSearchCV.

Build a Flask/Streamlit dashboard for interactive predictions.
