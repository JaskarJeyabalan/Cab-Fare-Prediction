# Cab Fare Prediction System

An end-to-end Machine Learning project to predict cab ride fares based on historical ride data, such as pickup/dropoff coordinates, timestamp, and passenger count.

## Project Overview

A cab rental startup completed a pilot project and aims to launch its services nationwide. To optimize pricing strategies, this project builds a predictive analytics pipeline using machine learning regression models to accurately forecast cab fare amounts before a ride is taken.

---

## Dataset Overview

The project uses historical pilot dataset split into training and testing sets:

| Dataset | Total Records | Key Features |
| :--- | :--- | :--- |
| **`train_cab.csv`** | ~16,067 rows | `fare_amount`, `pickup_datetime`, `pickup_longitude`, `pickup_latitude`, `dropoff_longitude`, `dropoff_latitude`, `passenger_count` |
| **`test_cab.csv`** | ~9,914 rows | Same features as training data (excluding target variable `fare_amount`) |

---

## Technical Stack & Libraries Used

- **Language:** Python
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib`, `seaborn`
- **Machine Learning Models:**
  - `LinearRegression`
  - `DecisionTreeRegressor`
  - `RandomForestRegressor`
  - `GradientBoostingRegressor`
- **Hyperparameter Tuning:** `GridSearchCV`, `RandomizedSearchCV`
- **Metrics:** Mean Squared Error (MSE), R-squared Score ($R^2$)

---

## Project Structure

```text
├── train_cab.csv           # Historical training data with target fare amount
├── test_cab.csv            # Unlabeled test data for evaluation
├── Cab_Fare_Prediction.ipynb # Jupyter Notebook containing complete pipeline
└── README.md               # Project documentation
