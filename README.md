# ✅ **Credit Lending Risk Classification using Machine Learning**

This project develops a **multi-class credit risk classification model** that categorizes customers into 4 risk buckets — **P1, P2, P3, P4** — based on credit history, delinquency behavior, and loan enquiry patterns.

The objective is to help lenders make **smarter and data-driven lending decisions.**

---

## ✅ **Project Highlights**

* Completed full **data cleaning**, preprocessing, and feature engineering.
* Built and compared multiple ML models:

  * ✅ Decision Tree
  * ✅ Random Forest
  * ✅ LightGBM
  * ✅ XGBoost
  * ✅ **CatBoost (Final Selected Model)**
* Final model achieved **~78.3% test accuracy**, outperforming baseline benchmarks.
* Conducted **feature importance analysis** to understand key credit risk drivers.

---

## ✅ **Dataset Overview**

The dataset includes customer credit profile indicators such as:

* Open/closed credit lines
* Delinquency counts (6–12 months)
* Loan enquiries: CC, PL, HL
* Income & employment duration
* Time since recent payment
* Secured/Unsecured trade lines
* Product enquiry history
* Various CIBIL-style behavioral metrics

Training dataset used: **train.csv**

---

## ✅ **Model Comparison**

| Model                      | Train Accuracy | Test Accuracy |
| -------------------------- | -------------- | ------------- |
| Decision Tree              | –              | 71.0%         |
| Random Forest              | –              | 76.3% – 77.4% |
| LightGBM                   | 82.4%          | 78.2%         |
| XGBoost                    | 83.7%          | 77.7%         |
| **CatBoost (Final Model)** | **79.8%**      | **78.29%**    |

### ✅ Why CatBoost Was Selected

* More stable test accuracy
* Handles categorical features natively
* Works well with noisy/tabular credit data
* Best balance of bias–variance
* Avoids overfitting better than other boosting models

---

## ✅ **Top 5 Influential Features (CatBoost)**

Sorted by importance:

| Rank  | Feature                | Importance |
| ----- | ---------------------- | ---------- |
| **1** | **Age_Oldest_TL**      | **22.57**  |
| **2** | enq_L3m                | 20.49      |
| **3** | pct_PL_enq_L6m_of_ever | 6.04       |
| **4** | time_since_recent_enq  | 9.52       |
| **5** | recent_level_of_deliq  | 4.54       |

✅ These show that **older trade lines**, **recent enquiry behavior**, and **delinquency levels** are strong predictors of loan risk.

---

## ✅ **Project Structure**

```
.
├── Data-Cleaning-Model-Building.ipynb   # Full workflow: Cleaning → EDA → Modeling
├── model.pkl                            # Saved CatBoost model
├── train.csv                             # Dataset can be used as train and test set
├── requirements.txt
└── README.md
```

---

## ✅ **How to Run the Project**

### 1. Clone the repository

```
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

### 2. Install requirements

```
pip install -r requirements.txt
```

### 3. Open Jupyter Notebook

```
jupyter notebook
```

---

## ✅ **Author**

**Aniket**
Data Science & AI Student
📍 Mumbai, India
📧 *[aniket.yadav52005@gmail.com](mailto:aniket.yadav52005@gmail.com)*
