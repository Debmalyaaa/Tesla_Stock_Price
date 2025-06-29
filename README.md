# 📈 Tesla Stock Price Prediction (2010–2020)

This project focuses on predicting the closing price of **Tesla (TSLA)** stock using historical data from **2010 to 2020**. We applied regression techniques to develop a predictive model using financial indicators like Open, High, Low, Adjusted Close, and Volume.

---

## 📁 Dataset

- **Source**: [Kaggle - Tesla Stock Data from 2010 to 2020](https://www.kaggle.com/datasets)
- **File**: `TSLA.csv`
- **Columns**:
  - `Date`
  - `Open`
  - `High`
  - `Low`
  - `Close`
  - `Adj Close`
  - `Volume`

---

## 📊 Exploratory Data Analysis (EDA)

- Checked for null values and basic statistics using `.info()` and `.describe()`.
- Plotted distributions of `High` and `Low` prices using `sns.histplot`.
- Visualized relationships using:
  - Scatter plots (`High vs Low`, `Close vs Adj Close`)
  - Pairplot to analyze multi-feature relationships

---

## ⚙️ Feature Selection

Selected the following features for training:
- **Independent Variables (X)**: `Open`, `High`, `Low`, `Adj Close`, `Volume`
- **Target Variable (Y)**: `Close`

---

## 🧪 Model Development

### 🔹 Train-Test Split

- Split: 80% training, 20% testing
- Scaled features using `StandardScaler` from `sklearn.preprocessing`

### 🔹 Models Used

#### ✅ Support Vector Regression (SVR)
- Built with `sklearn.svm.SVR`
- Evaluated with:
  - Mean Squared Error
  - R² Score
- Accuracy: ~**89.50%**

#### ✅ Random Forest Regressor
- Built with `RandomForestRegressor(n_estimators=100)`
- Achieved comparable performance to SVR

---

## 📈 Evaluation Metrics

- **Mean Squared Error (MSE)**
- **R² Score**

---

