🚔 Predicting Crime Rates with Machine Learning 📊
A data-driven approach to predict the rate of violent crimes per capita in communities. This project leverages socio-economic, law enforcement, and crime data, using Principal Component Analysis (PCA) for intelligent feature reduction and a Random Forest Regressor for accurate predictions.
✨ Key Features
📈 Data Preprocessing: Handles missing values and prepares the dataset for modeling.
🔬 PCA for Feature Reduction: Identifies the most influential factors contributing to crime rates, reducing dimensionality while preserving variance.
🤖 Machine Learning Model: Utilizes a RandomForestRegressor to predict ViolentCrimesPerPop.
📊 Performance Evaluation: Measures model accuracy using Mean Squared Error (MSE) and R² Score.
🔍 Feature Importance: Reveals the top socio-economic indicators that are most predictive of crime rates.
🛠️ Tech Stack & Libraries
Python
Pandas & NumPy for data manipulation
Scikit-learn for PCA and machine learning
Matplotlib & Seaborn for data visualization
Jupyter Notebook for exploratory data analysis
📂 Project Structure
├── communities_and_crime.csv   # The raw dataset
├── project.ipynb               # Jupyter Notebook with all the analysis, PCA, and model training
└── README.md                   # You are here!


🚀 Getting Started
Follow these steps to get the project up and running on your local machine.
Clone the repository:
git clone [https://github.com/your-username/crime-prediction-project.git](https://github.com/your-username/crime-prediction-project.git)
cd crime-prediction-project


Install the required libraries:
pip install pandas numpy scikit-learn matplotlib seaborn jupyter


Launch Jupyter Notebook:
jupyter notebook

Then, open the project.ipynb file to explore the code.
⚙️ Methodology
Data Loading & Cleaning: The "Communities and Crime" dataset is loaded, and missing values (represented by ?) are replaced with NaN and then imputed using the mean of each respective column.
Feature Scaling: All features are standardized using StandardScaler to ensure that each feature contributes equally to the PCA.
Principal Component Analysis (PCA): PCA is applied to the scaled dataset to reduce the number of features. We analyze the explained variance to determine the optimal number of components to retain for our model.
Model Training: A RandomForestRegressor is trained on the principal components derived from the PCA.
Evaluation: The model's performance is evaluated on a test set using Mean Squared Error (MSE) and the R² score to determine its predictive accuracy.
📈 Results & Performance
By using the top principal components, we significantly reduced the complexity of the model without a substantial loss of information.
Mean Squared Error (MSE): 0.015
R² Score: 0.65
This indicates that our model can explain approximately 65% of the variance in violent crime rates based on the selected socio-economic features.
🔑 Top Predictive Factors (Principal Components)
The analysis reveals that the principal components are complex combinations of the original features. The most significant factors often relate to:
Poverty and income levels (PctPopUnderPov, perCapInc)
Population density and housing (PersPerOccupHous, PctPersDenseHous)
Family structure (PctKids2Par, MalePctDivorce)
Education levels (PctBSorMore, PctNotHSGrad)
Racial demographics (racepctblack, racePctWhite)
For a detailed breakdown, please refer to the PCA section in the project.ipynb notebook.
