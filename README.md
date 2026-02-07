# Customer Churn Prediction using Backward Probability and XGBoost

> **Predicting churn with clarity:** Backward probability–based feature selection combined with XGBoost for interpretable and efficient customer retention insights.

---

## 📖 Abstract

Customer churn is a critical challenge for subscription-based businesses. This project uses the **Telco Customer Churn dataset** to predict customer churn by combining **backward probability feature selection** with **XGBoost** modeling.

Backward probability helps identify features that repeatedly contribute to churn prediction across iterations, improving both **model interpretability** and **computational efficiency**. The final model achieves a **ROC-AUC of approximately 0.77**, while highlighting key churn drivers such as **contract type**, **tenure**, **payment method**, and **monthly charges**.

---

### Dataset
This project uses the **Telco Customer Churn dataset** provided by IBM.  
The dataset is loaded directly from the following link:

[Telco Customer Churn dataset (IBM)](https://raw.githubusercontent.com/blastchar/telco-churn/master/WA_Fn-UseC_-Telco-Customer-Churn.csv)

No local dataset file is provided


## 📂 Repository Structure

```
customer-churn-ml/
│
├── README.md
├── requirements.txt
└── Customer_churn.ipynb
```

---

## 🛠️ Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/rb577/customer-churn-ml.git
cd customer-churn-ml
```

### 2️⃣ Install Dependencies

Ensure you have **Python 3.9+** installed. Then install the required packages:

```bash
pip install -r requirements.txt
```

### 3️⃣ Launch Jupyter Notebook

```bash
jupyter notebook Customer_churn.ipynb
```

### 4️⃣ Run the Notebook

Execute the notebook cells sequentially:

1. Data Preprocessing  
2. Feature Selection (Backward Probability)  
3. Model Training  
4. Evaluation  
5. Business Insights  

---

## 📊 Results

| Model / Approach                              | ROC-AUC | Precision        | Recall          | F1-score | Notes                               |
|---------------------------------------------|---------|------------------|-----------------|----------|-------------------------------------|
| Logistic Regression                          | ~0.77   | Moderate         | Moderate        | Balanced | High interpretability               |
| Random Forest                               | ~0.77   | Higher precision | Lower recall    | Balanced | Captures nonlinearities             |
| XGBoost (all features)                      | ~0.76–0.77 | Similar to RF | Similar to RF   | Balanced | Computationally heavier             |
| **XGBoost (backward probability features)** | **~0.77+** | Slightly lower | Improved recall | Balanced | Efficient and interpretable         |

---

## 💡 Business Recommendations

- **Month-to-month contracts** → Offer loyalty programs or long-term discounts  
- **Short-tenure customers** → Improve onboarding and early engagement  
- **Electronic check payments** → Incentivize auto-pay or credit card usage  
- **High monthly charges** → Introduce tiered pricing or bundle offers  

---

## 🚀 Key Takeaways

- Backward probability feature selection improves interpretability without performance loss  
- XGBoost performs strongly even with a reduced feature set  
- Insights are directly actionable for churn reduction strategies  

---

## 📌 Future Improvements

- Hyperparameter tuning with Bayesian optimization  
- SHAP-based explainability  
- Model deployment using Streamlit or FastAPI  
- Cost-sensitive churn modeling  

---

📚 References
Telco Customer Churn dataset (IBM Sample Data)

Chen & Guestrin (2016). XGBoost: A Scalable Tree Boosting System.  
EOF


## 📜 License

This project is intended for **educational and portfolio purposes**.
