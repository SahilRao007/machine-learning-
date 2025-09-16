
# 🏠 House Rent Prediction

This project predicts **house rental prices in Indian cities** using **machine learning**. It covers end-to-end steps: data exploration, feature engineering, and model building, with a focus on comparing **Random Forest Regressor** vs **Linear Regression**.

---

## 🚀 Features

* **Data preprocessing**:

  * Date conversion (`Posted On` → datetime)
  * Handling categorical variables (`City`, `Furnishing Status`, `Tenant Preferred`, `Area Type`)
  * Feature creation:

    * `Rent/Size` (₹ per sqft)
    * `month` (from posting date)
    * Mean rent mapping for each `Area Locality`
  * One-hot & label encoding

* **Exploratory Data Analysis (EDA)**:

  * Rent distribution & outliers
  * City vs rent comparison
  * BHK vs rent analysis (per city)
  * Insights on affordability & city-level differences

* **Modeling**:

  * **Random Forest Regressor** (best performer)
  * **Linear Regression** (baseline model)
  * Train/test split for fair evaluation

* **Evaluation Metrics**:

  * R² Score
  * MAE (Mean Absolute Error)
  * RMSE (Root Mean Squared Error)

---

## 📂 Dataset

* **File**: `House_Rent_Dataset.csv`
* **Glossary**: `Dataset Glossary.txt`
* **Columns**:

  * `Posted On` – Listing date
  * `BHK` – Number of bedrooms
  * `Size` – Area in sqft
  * `Rent` – Rent amount (target)
  * `City` – City name
  * `Furnishing Status` – Furnished/Semi-Furnished/Unfurnished
  * `Tenant Preferred` – Family/Bachelor/Company
  * `Area Locality`, `Area Type`, `Floor`, `Point of Contact`

---

## 📊 Key Insights from EDA

* **Rent distribution is right-skewed** (mean ≈ ₹35k, median ≈ ₹16k).
* **Mumbai** has the highest median rents (\~₹52k), while **Kolkata** is the cheapest (\~₹6k for 1BHK).
* **Higher BHKs** (4BHK, 5BHK, 6BHK) show exponential rent increases in metros like Mumbai and Delhi.
* **6BHKs** are rare, indicating low demand or supply.
* Random Forest captures **non-linear city & BHK patterns** better than Linear Regression.

---

## 🛠️ Tech Stack

* **Python 3**
* **Pandas / NumPy** – Data preprocessing
* **Matplotlib / Seaborn** – Visualization
* **Scikit-learn** – ML models & metrics

---

## 📈 Results

| Model             | R² Score  | MAE (₹)   | RMSE (₹)   |
| ----------------- | --------- | --------- | ---------- |
| Random Forest     | **0.864** | **3,660** | **23,260** |
| Linear Regression | 0.645     | 14,169    | 37,630     |

➡️ **Random Forest outperformed Linear Regression** across all metrics.



## ✨ Author

Developed as an **end-to-end ML regression project** to understand how real estate rental prices can be modeled with data-driven approaches.

