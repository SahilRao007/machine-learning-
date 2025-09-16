
# Placement Predictor 🎓

This project is a **machine learning model** that predicts whether a student is likely to get placed based on their **CGPA** and **IQ** scores. It demonstrates a complete ML pipeline: data preprocessing, exploratory data analysis (EDA), and model training using **Logistic Regression**.

---

## 🚀 Features

* Loads and cleans placement dataset (`modified_placement_data.csv`).
* Handles:

  * **Missing values** (fills CGPA nulls with mean).
  * **Duplicate records**.
  * **Categorical encoding** (placement → Yes/No).
* Exploratory Data Analysis (scatter plots of CGPA vs IQ).
* Trains a **Logistic Regression classifier** to predict placement outcomes.
* Evaluates performance with **accuracy score**.

---

## 📂 Dataset

The dataset used is **`modified_placement_data.csv`**.

* **Features**:

  * `cgpa` – Student’s Cumulative Grade Point Average.
  * `iq` – Student’s IQ level.
* **Target**:

  * `placement` – Whether the student got placed (`Yes` / `No`).

---

## 🛠️ Tech Stack

* **Python 3**
* **Pandas** – Data handling & preprocessing
* **NumPy** – Numerical computations
* **Matplotlib** – Data visualization
* **Scikit-learn** – Model training & evaluation

---

## 📊 Model Training

* **Algorithm**: Logistic Regression
* **Train-test split**: 80% training / 20% testing
* **Evaluation metric**: Accuracy

---

## 📈 Results

The Logistic Regression model achieves an accuracy of around:

```
Logistic Regression model accuracy: 95.00%
```




Developed as a **beginner-friendly ML project** to demonstrate how to build and evaluate a simple classification model.

---
