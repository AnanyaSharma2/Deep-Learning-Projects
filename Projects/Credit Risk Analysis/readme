# 💳 Credit Risk Prediction & Loan Approval Classification

## 📌 Project Overview

This project focuses on building a **machine learning model** to predict **loan approval priority levels (P1–P4)** based on a customer’s **credit behavior, financial history, and demographic details**.

The system integrates data from **two different sources (internal + external credit bureau data)** and applies **feature engineering + machine learning (XGBoost)** to classify applicants into risk categories.

---

## 🎯 Objective

The main goal of this project is to:

* Analyze customer creditworthiness
* Predict loan approval categories (**P1, P2, P3, P4**)
* Reduce financial risk for lenders
* Use both behavioral and financial indicators for decision-making

---

## 📊 Dataset Description

The dataset is divided into **two case studies**:

---

## 🏦 Case Study 1: Internal Bureau Data

This dataset contains **account-level credit information** of customers.

### 🔹 Key Feature Groups:

### 1. Account Summary

* `Total_TL` → Total accounts
* `Tot_Active_TL` → Active accounts
* `Tot_Closed_TL` → Closed accounts

### 2. Recent Activity (Last 6 / 12 Months)

* `Total_TL_opened_L6M`, `Total_TL_opened_L12M`
* `Tot_TL_closed_L6M`, `Tot_TL_closed_L12M`
* Percent features showing activity trends

👉 Helps identify **recent borrowing behavior**

---

### 3. Account Type Distribution

* `Auto_TL`, `CC_TL`, `PL_TL`, `Home_TL`, `Gold_TL`
* `Secured_TL` vs `Unsecured_TL`

👉 Indicates **credit mix and exposure**

---

### 4. Risk Indicators

* `Tot_Missed_Pmnt` → Missed payments
* `Age_Oldest_TL`, `Age_Newest_TL`

👉 Measures **credit history length and reliability**

---

## 🌐 Case Study 2: External / CIBIL Data

This dataset captures **credit bureau behavior + demographics + enquiries**

---

### 🔹 Key Feature Groups:

### 1. Delinquency & Payment Behavior

* `num_times_delinquent`
* `max_delinquency_level`
* `num_deliq_6mts`, `num_deliq_12mts`
* `num_times_30p_dpd`, `num_times_60p_dpd`

👉 Measures **repayment discipline**

---

### 2. Payment Quality Classification

* `num_std` → Standard payments
* `num_sub` → Sub-standard
* `num_dbt` → Doubtful
* `num_lss` → Loss accounts

👉 Indicates **loan repayment quality**

---

### 3. Enquiry Behavior

* `tot_enq`, `CC_enq`, `PL_enq`
* `enq_L3m`, `enq_L6m`, `enq_L12m`

👉 High enquiries = **credit hungry behavior**

---

### 4. Demographics & Financial Info

* `AGE`, `GENDER`, `MARITALSTATUS`
* `EDUCATION`, `NETMONTHLYINCOME`
* `Time_With_Curr_Empr`

👉 Helps assess **financial stability**

---

### 5. Utilization & Exposure

* `CC_utilization`, `PL_utilization`
* `max_unsec_exposure_inPct`

👉 Indicates **debt burden**

---

### 6. Target Variable

* `Approved_Flag` → Output label:

  * **P1** → Low Risk
  * **P2** → Moderate Risk
  * **P3** → High Risk
  * **P4** → Very High Risk

---

## 🔄 Data Processing Pipeline

### 1. Data Cleaning

* Removed invalid values (`-99999`)
* Dropped highly corrupted columns
* Ensured no missing values

👉 Improved data reliability 

---

### 2. Dataset Merging

* Combined internal + external datasets using `PROSPECTID`
* Final dataset: **~51,296 records with 79 features** 

---

### 3. Feature Engineering

* Statistical testing:

  * **Chi-Square** → categorical features
  * **ANOVA** → numerical features
* Removed multicollinearity using **VIF**

👉 Reduced features from **72 → 37 important features** 

---

### 4. Encoding

* Converted categorical variables into numerical format
* Applied one-hot encoding for model compatibility

---

## 🤖 Model Used

### 🚀 XGBoost Classifier

* Multi-class classification model
* Objective: `multi:softmax`
* Classes: 4 (P1–P4)

---

## 📈 Model Performance

* ✅ **Accuracy: ~99%**
* Strong precision & recall across all classes

Example:

* P1 → ~97% F1 Score
* P2 → Perfect classification
* P3 → ~98% F1 Score
* P4 → Perfect classification 

---

## 💡 Key Insights

* Credit behavior features (delinquency, missed payments) are **highly predictive**
* Recent activity (last 6 months) strongly impacts risk classification
* Feature selection significantly improves model performance
* Combining internal + external data gives **better prediction power**

---

## 🚀 Applications

* Loan approval systems
* Credit scoring engines
* Risk management in banks
* Financial fraud detection
* Customer segmentation

---

## 🔮 Future Improvements

* Use deep learning models (ANN)
* Explainability using SHAP
* Real-time scoring system
* Deployment as API

---

