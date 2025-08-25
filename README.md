# Loan Approval Prediction 🏦

## 📌 Project Overview
This project predicts whether a loan application will be **Approved** or **Rejected** using machine learning techniques.  
We use the **Loan Approval Prediction dataset (Kaggle)** and apply data preprocessing, feature encoding, model training, and evaluation with focus on imbalanced data.

---

## ⚙️ Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib / Seaborn  

---

## 📂 Dataset
- Source: [Loan Approval Prediction Dataset (Kaggle)](https://www.kaggle.com/datasets/trinipoor/loan-approval-prediction-dataset)  
- Rows: 4269  
- Columns: 13 (features + target)  
- Target: `loan_status` → **Approved** / **Rejected**

---

## 🛠️ Steps
1. **Data Loading & Exploration**
   - Loaded dataset
   - Checked shape, column types, missing values
   - Examined class imbalance in `loan_status`

2. **Preprocessing**
   - Handled missing values
   - Encoded categorical variables (`education`, `self_employed`)
   - Scaled numeric features

3. **Model Training**
   - Logistic Regression
   - Decision Tree
   - Random Forest

4. **Evaluation**
   - Accuracy, Precision, Recall, F1-score
   - Confusion Matrix
   - Feature Importance (for tree-based models)

5. **Imbalance Handling**
   - Used **SMOTE** to oversample minority class

---

## 📊 Results
- **Best performing model:** Random Forest  
- Good balance between **Recall (Approved loans)** and **Precision**  
- Demonstrated effect of SMOTE on imbalanced classes  

---

## 🚀 How to Run
### In Google Colab
1. Upload this notebook (`loan_approval_prediction.ipynb`) to your Colab environment  
2. Run all cells sequentially  
3. Results (confusion matrix, classification report, feature importance) will be displayed  

### Locally
```bash
git clone https://github.com/<your-username>/loan-approval-prediction.git
cd loan-approval-prediction
pip install -r requirements.txt
jupyter notebook loan_approval_prediction.ipynb
