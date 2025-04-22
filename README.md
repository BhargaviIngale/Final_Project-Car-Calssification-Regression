# 🚗 Car Modeling Projects: Classification & Price Prediction

This repository contains two end-to-end machine learning projects focused on the automotive domain:

1. **Car Classification** – Predict the class of a car (e.g., bus, van) using geometric features.
2. **Car Price Prediction** – Predict the market price of a car based on its specifications.

Both projects involve data preprocessing, EDA, model building, evaluation, and feature importance analysis.

---

## 📁 Project 1: Car Classification (Multi-Class)

### 🧾 Dataset Details

- **Dataset file**: `cars_class.csv`
- **Type**: Multi-class Classification
- **Samples**: 719
- **Features**: 18 numerical
- **Target variable**: `Class`  
  - 0: Bus  
  - 1: Opel Manta  
  - 2: Saab  
  - 3: Van

### 📊 Features

- Comp: Compactness
- Circ: Circularity
- D.Circ: Distance Circularity
- Rad.Ra: Radius ratio
- Pr.Axis.Ra: pr.axis aspect ratio
- Max.L.Ra: max.length aspect ratio
- Scat.Ra: scatter ratio
- Elong: elongatedness
- Pr.Axis.Rect: pr.axis rectangularity
- Max.L.Rect: max.length rectangularity
- Sc.Var.Maxis: scaled variance along major axis
- Sc.Var.maxis: scaled variance along minor axis
- Ra.Gyr: scaled radius of gyration
- Skew.Maxis: skewness about major axis
- Skew.maxis: skewness about minor axis
- Kurt.maxis: kurtosis about minor axis
- Kurt.Maxis: kurtosis about major axis
- Holl.Ra: hollows ratio

### 🛠️ Steps Performed

- Loaded and explored dataset
- Preprocessing:
  - Checked missing values
  - Feature scaling using StandardScaler
- Data Splitting: 80% training, 20% testing
- Applied multiple models:
  - Logistic Regression
  - Random Forest
  - XGBoost
- Hyperparameter tuning using GridSearchCV
- Final model saved as `final_model`
- Evaluated using:
  - Accuracy
  - F1-score
  - Confusion matrix


### ✅ Evaluation Metrics (on test data)

- **Accuracy**
- **F1-Score**
- **Confusion Matrix**
- **Feature Importance**

---

## 📁 Project 2: Car Price Prediction (Regression)

### 🧾 Dataset Details

- **Dataset file**: `cars_price.csv`
- **Type**: Regression
- **Samples**: 206
- **Features**: 25
- **Target variable**: `price`

### 📊 Features

| Type         | Features |
|--------------|----------|
| Categorical  | make, fuel-type, aspiration, num-of-doors, body-style, drive-wheels, engine-location, engine-type, num-of-cylinders, fuel-system |
| Numerical    | symboling, normalized-losses, wheel-base, length, width, height, curb-weight, engine-size, bore, stroke, compression-ratio, horsepower, peak-rpm, city-mpg, highway-mpg |

### 🛠️ Steps Performed

- Loaded dataset and identified data types
- Preprocessing:
  - Handled missing values
  - Encoded categorical variables (OneHotEncoding/LabelEncoding)
  - Feature scaling using StandardScaler
- Data Splitting: 80% training, 20% testing
- Applied multiple regression models:
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor
  - Ridge and Lasso
- Hyperparameter tuning using GridSearchCV
- Final model saved as `final_model`
- Evaluated using:
  - MSE
  - MAE
  - R² Score
- Visualized actual vs predicted prices and feature importances

### ✅ Evaluation Metrics (on test data)

- **MSE (Mean Squared Error)**
- **MAE (Mean Absolute Error)**
- **R² Score**

---

## 🔧 Tools & Technologies Used

- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook
- Pickle (for model saving)

---
<!--## 🗃️ Project Links

- 📎Dataset Link: *[Insert your GitHub repo or data link here]*.
- Demo link:*[Insert your linkedin here]*. -->


