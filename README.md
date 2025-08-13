# Customer-Churn-Prediction-Bank-Customers-
## 📝 Project Description Customer churn is a major challenge in the banking industry, as retaining existing customers is often more cost-effective than acquiring new ones.   This project uses **machine learning** to predict whether a customer is likely to leave the bank based on demographic details, account information, and transaction history.  

# Customer Churn Prediction (Bank Customers)

## 📌 Objective
The goal of this project is to **predict which bank customers are likely to leave (churn)** based on historical data.  
By identifying churn-prone customers, banks can take proactive measures to improve retention.



## 📂 Dataset
**Name:** Churn Modelling Dataset  
**Description:** Contains customer demographic, account, and transaction details, along with a churn indicator (`Exited`).


## 🚀 Approach

### 1. Data Preparation
- **Data Cleaning:** Removed unnecessary columns and handled missing values (if any).
- **Encoding Categorical Features:**
  - **Label Encoding:** Applied to binary categories like `Gender`.
  - **One-Hot Encoding:** Applied to multi-class features like `Geography`.

### 2. Model Development
- Split dataset into **training** and **testing** sets.
- Trained multiple classification models:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting (XGBoost / LightGBM)
- Selected the **best-performing model** based on accuracy, precision, recall, and F1-score.

### 3. Feature Importance Analysis
- For tree-based models, extracted feature importances to understand key factors influencing churn.
- Top features included:
  - Credit Score
  - Age
  - Tenure
  - Balance
  - Number of Products
  - Geography



## 📊 Results & Insights

| Model              | Accuracy | Precision | Recall | F1-Score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression| 0.81     | 0.70      | 0.54   | 0.61     |
| Random Forest      | 0.86     | 0.77      | 0.64   | 0.70     |
| Gradient Boosting  | **0.87** | **0.79**  | **0.66**| **0.72** |

### Key Insights:
- **Age** and **Credit Score** are strong predictors of churn.
- Customers with **low tenure** and **low balance** tend to leave more often.
- Geography impacts churn — customers from certain regions have higher churn rates.
- Personalized retention strategies can be designed targeting these high-risk profiles.


## 🛠️ Skills Used
- Data Preprocessing (Pandas, NumPy)
- Categorical Encoding (Label Encoding, One-Hot Encoding)
- Model Training & Evaluation (Scikit-learn, XGBoost)
- Feature Importance Analysis
- Data Visualization (Matplotlib, Seaborn)

