# 🏠 Housing Price Prediction using XGBoost

## 📌 Project Overview
This project focuses on predicting housing prices using the **California Housing dataset** from `sklearn.datasets`.  
A regression model was built to predict median house values based on multiple socioeconomic and geographic features.

---

## 📊 Dataset
- Source: `sklearn.datasets.fetch_california_housing()`
- Type: Regression dataset
- Target Variable: **Median House Value**
- Features:
  - MedInc (Median Income)
  - HouseAge
  - AveRooms
  - AveBedrms
  - Population
  - AveOccup
  - Latitude
  - Longitude

---

## 🔍 Exploratory Data Analysis (EDA)
- Computed the **correlation matrix** between all features and the target variable
- Analyzed relationships among features to understand their impact on housing prices
- Identified strong correlations with median income and location-based features

---

## 🔀 Train-Test Split
- Training data: **80%**
- Testing data: **20%**
- Data split was performed to evaluate the model’s ability to generalize to unseen data

---

## 🧠 Model Used
- **XGBRegressor (Extreme Gradient Boosting)**
- Chosen because:
  - Performs well on structured/tabular data
  - Handles non-linear relationships efficiently
  - Provides strong predictive accuracy

---

## 🏗️ Model Workflow
1. Load dataset using `fetch_california_housing()`
2. Convert dataset into a Pandas DataFrame
3. Perform correlation analysis
4. Split data into training and testing sets (80/20)
5. Train the XGBRegressor model
6. Generate predictions
7. Evaluate model performance

---

## 📈 Evaluation Metrics
The following metrics were used to assess model performance:

- **R² Score (Coefficient of Determination)**  
  Indicates how well the model explains the variance in housing prices.

- **Mean Absolute Error (MAE)**  
  Measures the average absolute difference between predicted and actual values.

---

## 🧪 Model Performance

### 🔹 Training Data
- **R² Score:** `0.9436`
- **Mean Absolute Error:** `0.1933`

### 🔹 Test Data
- **R² Score:** `0.8338`
- **Mean Absolute Error:** `0.3109`

✅ The model performs very well on training data and generalizes effectively to test data, with a reasonable drop in performance indicating **controlled overfitting**.

---

## 🛠️ Technologies Used
- Python
- NumPy
- Pandas
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn

---

## 🚀 How to Run the Project
Install required dependencies:

```bash
pip install numpy pandas scikit-learn xgboost matplotlib seaborn
