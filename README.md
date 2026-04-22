# 🌲 Deforestation Prediction using Random Forest

## 📌 Overview

This project uses a **Random Forest Regressor** to analyze and predict deforestation trends between **2015–2020** based on historical forest area and land data.

The model also identifies key factors contributing to deforestation using feature importance analysis.

---

## 📊 Dataset

The dataset (`Forest_Area.csv`) includes:

* Forest area (1990, 2000, 2010, 2015)
* Total land area (2020)
* Forest area as % of total land (2020)
* Country-level data
* Target variable: **Deforestation (2015–2020)**

---

## ⚙️ Methodology

### 1. Data Preprocessing

* Converted relevant columns to numeric
* Removed invalid/missing values
* Excluded aggregate rows (e.g., "WORLD")

### 2. Feature Selection

Features used:

* Historical forest area (1990–2015)
* Total land area (2020)
* Forest proportion (2020)
* Country (one-hot encoded)

### 3. Model

* Algorithm: **Random Forest Regressor**
* Train-test split: 80% / 20%
* Trees: 100 estimators

### 4. Evaluation Metrics

* **R² Score** → measures model accuracy
* **RMSE (Root Mean Squared Error)** → measures prediction error

---

## 📈 Results

Example outputs:

* R² Score: *(your value here)*
* RMSE: *(your value here)*

---

## 🔍 Key Insights

* Identifies top features influencing deforestation
* Helps understand how historical forest trends relate to recent loss
* Country-specific patterns play a significant role

---

## ⚠️ Limitations

* One-hot encoding of countries may lead to overfitting
* Limited feature set (no economic, climate, or policy data)
* Model may not generalize well to unseen regions

---

## 🚀 How to Run

### Install dependencies

```bash
pip install pandas numpy scikit-learn
```

### Run the script

```bash
python your_script_name.py
```

---

## 📁 Project Structure

```
├── Forest_Area.csv
├── model.py
└── README.md
```

---

## 🔮 Future Improvements

* Add environmental and economic variables
* Try other models (XGBoost, Linear Regression)
* Perform hyperparameter tuning
* Improve generalization by removing country encoding

---

## 🤝 Contributing

Feel free to fork the project and submit improvements.

---

## 📜 License

This project is open-source and available under the MIT License.
