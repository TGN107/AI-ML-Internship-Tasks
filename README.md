# **AI-ML-Internship-Tasks**
##**DevelopersHub Corporation AI/ML Engineering Internship Tasks**

###A collection of machine learning projects completed during my internship, covering classification, regression, and time-series forecasting with real-world datasets.

##  Task 1: Exploratory Data Analysis – Iris Dataset  
**Objective**: Understand data structure, distribution, and species-separating features.  
**Dataset**: Iris (150 samples, 4 features, 3 species)  
**Key Findings**:  
- Petal measurements are far more discriminative than sepal features.  
- *Setosa* is linearly separable; *Versicolor* and *Virginica* overlap in sepal space.  
- Visualizations (scatter, histogram, box plots) confirmed feature importance and outliers.


##  Task 3: Heart Disease Prediction  
**Objective**: Predict presence of heart disease using clinical indicators.  
**Dataset**: UCI Heart Disease (297 patients, clean, balanced)  
**Models**: Logistic Regression, Decision Tree  
**Results**:  
- **Logistic Regression**: **80% accuracy**, **AUC 0.80**  
- Top predictors: `thal`, `ca`, `exang`, `oldpeak` — *not* cholesterol or blood sugar.  
- Model aligns with clinical logic: symptom-based features > traditional biomarkers.



##  Task 6: California House Price Prediction  
**Objective**: Predict median house value using census data.  
**Dataset**: California Housing (20,640 block groups)  
**Models**: Linear Regression, Gradient Boosting (GBR)  
**Results**:  
- **GBR MAE: $33,220** vs LR MAE: $47,259  
- Key drivers: **location** (coastal premium), **median income**, **room count**  
- Data cleaned (capped outliers, log-transformed skewed features) → major accuracy gain.



##  Task 2: Apple (AAPL) Stock Price Forecasting  
**Objective**: Predict next-day closing price using daily OHLCV data.  
**Dataset**: Yahoo Finance (2020–2025, 1,479 rows)  
**Models**: Linear Regression, Random Forest  
**Results**:  
- **Linear Regression MAE: $3.10**, RMSE: $4.53  
- **RF underperformed** (MAE: $9.91) — data is highly autocorrelated (r = 0.998).  
- Simple linear model captures dominant trend: *“Tomorrow ≈ Today”*.

---

## 💡 Final Insights  
- **Simpler models often win** when data has strong linear/trend patterns.  
- **Data quality > model complexity**: Cleaning and feature understanding drove success.  
- All projects include reproducible notebooks and emphasize **real-world interpretability**.
