# **Credit Lending Risk Classification using Machine Learning**

This project builds a **multi-class credit risk model** to classify customers into 4 risk categories (P1, P2, P3, P4) using their credit behavior, loan history, enquiries, and delinquency patterns.

The goal is to help financial institutions identify the likelihood of customer default and make better lending decisions.

---

## ✅ **Project Highlights**

* Performed **data cleaning**, missing value handling, feature engineering, and EDA.
* Built and compared multiple models:
  ✔ Decision Trre
  ✔ Random Forest
  ✔ LightGBM
  ✔ XGBoost
  ✔ CatBoost
* Final model selected: **CatBoostClassifier**
* Achieved **Test Accuracy: ~78.3%**, higher than the reference benchmark.
* Analyzed **feature importances** to understand which credit factors contribute most to risk.

---

## ✅ **Dataset Description**

The dataset contains customer credit history features such as:

* Total credit lines (open/closed)
* Delinquency history
* Enquiry behavior (CC, PL, HL)
* Time since last payment
* Income, employment time
* Loan flags (CC_Flag, PL_Flag, HL_Flag, etc.)
* CIBIL score–related features

Dataset is included train and test set as:
`tarin.csv`

---

## ✅ **Models Trained**

| Model                    | Train Accuracy | Test Accuracy |
| ------------------------ | -------------- | ------------- |
| Decision Tree            | -              | 71.0%         |
| Random Forest            | -              | 77.4%         |
| LightGBM                 | 82.4%          | 78.2%         |
| XGBoost                  | 83.7%          | 77.7%         |
| **CatBoost (Final)**     | **79.8%**      | **78.29%**    |

CatBoost was selected because:

✅ Best generalization
✅ Most stable test accuracy
✅ Handles categorical features well
✅ No heavy preprocessing required

---

## ✅ **Feature Importance (CatBoost)**

Top 5 influential factors in credit risk prediction (sorted by importance) :

| Rank  | Feature                | Importance |
| ----- | ---------------------- | ---------- |
| **1** | **Age_Oldest_TL**      | **22.57**  |
| **2** | enq_L3m                | 20.49      |
| **3** | pct_PL_enq_L6m_of_ever | 6.04       |
| **4** | recent_level_of_deliq  | 4.54       |
| **5** | time_since_recent_enq  | 9.52       |


These features help explain how customer behavior impacts loan default probability.

---

## ✅ **Project Structure**

```
.
├── Data-Cleaning-Model-Building.ipynb
├── model.pkl
├── train.csv
├── README.md
└── requirements.txt
```

---

## ✅ **How to Run**

1. Clone the repo:

```
git clone https://github.com/<your-username>/<repo-name>.git
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Open notebooks:

```
jupyter notebook
```

---

---

## ✅ **Author**

**Aniket**, Data Science & AI Student
📍 Mumbai, India
📧 aniket.yadav52005@gmail.com 
