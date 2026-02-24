# 🚀 Production-Grade Feature Engineering using PySpark

## 📌 Project Overview

This project demonstrates how to build a production-ready Machine Learning dataset using PySpark in Databricks.

The goal was to transform raw user event data into an ML-ready dataset by performing feature engineering, label creation, and dataset splitting.

---

## 🧠 Problem Statement

Given user interaction event data, create a binary classification dataset to predict whether a user made a purchase.

---

## ⚙️ Steps Performed

### 1️⃣ Created Binary Target Label

* Assigned `1` if a user made at least one purchase
* Assigned `0` otherwise
* Used PySpark `groupBy` and conditional aggregation

### 2️⃣ Feature Engineering

Aggregated behavioral features such as:

* Average session time
* Total number of events
* User demographics (age, country)

### 3️⃣ Joined Features and Label

Combined engineered features with the target label to create a final training dataset.

### 4️⃣ Train-Test Split

* 80% Training data
* 20% Testing data
* Used `randomSplit()` with seed for reproducibility

### 5️⃣ Validated Class Distribution

Checked for class imbalance using groupBy count.

---

## 📊 Final Dataset Structure

| Column           | Description            |
| ---------------- | ---------------------- |
| user_id          | Unique user identifier |
| age              | User age               |
| country          | User country           |
| avg_session_time | Average session time   |
| total_events     | Total user events      |
| purchased        | Target variable (0/1)  |

---

## 🛠 Tech Stack

* PySpark
* Databricks
* Spark SQL
* GitHub

---

## 📈 Key Learning Outcomes

* Production-level feature engineering
* Target variable creation in Spark
* Aggregation using groupBy
* Handling class imbalance
* Preparing ML-ready datasets
* Working in Unity Catalog environment

---

## 🎯 Future Improvements

* Train Logistic Regression model
* Apply Random Forest classifier
* Perform feature scaling
* Handle class imbalance using sampling techniques
* Deploy model

---

## 👩‍💻 Author

Nandini Wadile
Artificial Intelligence & Data Science Student

---

