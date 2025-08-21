# 🪪 Credit Card Default Risk Prediction

A complete **Machine Learning pipeline** to predict the likelihood of a credit card customer defaulting on their next month’s payment.  
The aim is to deliver an **accurate**, **interpretable**, and **deployable** solution for **binary classification** — **Default (Yes)** or **No Default (No)**.  

---

## 📂 Dataset  
📌 **Source:** [UCI Machine Learning Repository – Default of Credit Card Clients](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients)  
📌 **Samples:** `30,000` customers  
📌 **Features Include:**  
- 👤 **Demographics:** Age, Gender, Education, Marital Status  
- 💰 **Credit Usage:** Credit limit, Bill amounts (last 6 months), Payments  
- 📅 **Repayment Status:** Delay codes for past 6 months  
- 🎯 **Target:** `Default Payment Next Month` → (1 = Yes, 0 = No)  

---

## 🎯 Objective  
> Build a predictive model to **classify** whether a client is likely to default in the upcoming month, enabling **financial institutions** to take **proactive risk control measures**.  

---

## 📊 Exploratory Data Analysis (EDA)  
🔍 **Key Insights:**  
- 📈 **Right-skewed** distribution in bill and payment amounts  
- 🔗 Correlation between repayment delays & default likelihood  
- 💳 Higher credit limit customers tend to default less frequently  

📌 **Visualizations Used:**  
- Count Plots, Pie Charts, Histograms  
- Correlation Heatmaps  
- Distribution & Box Plots for Outlier Detection  

---

## 🧹 Data Preprocessing  
✅ Column renaming for clarity (`PAY_0` → `SEP_PAY`)  
✅ One-hot encoding for categorical variables  
✅ Outlier handling with **IQR method**  
✅ Feature scaling with **StandardScaler**  
✅ Target encoding: Yes → `1`, No → `0`  

---

## 🤖 Model Performance  

| 🧠 Model              | 🎯 Accuracy | 🎯 Precision | 🔄 Recall | 📊 F1 Score |
|----------------------|------------|-------------|----------|------------|
| Logistic Regression  | 0.68       | 0.69        | 0.68     | 0.68       |
| Decision Tree        | 0.82       | 0.81        | 0.83     | 0.82       |
| **Random Forest** ✅ | **0.88**   | **0.93**    | **0.83** | **0.88**   |
| AdaBoost             | 0.86       | 0.93        | 0.78     | 0.85       |
| Gradient Boosting    | 0.87       | 0.94        | 0.80     | 0.86       |

🏆 **Best Model:** Random Forest after **GridSearchCV Hyperparameter Tuning**  

---

## 🚀 Deployment  
- 📦 Final pipeline saved using **Joblib**  
- 🔄 Reloadable for **real-time predictions** on new customer data  

---

## 🛠 Tech Stack  

**📌 Languages & Libraries:**  
- 🐍 Python  
- 🔢 NumPy, 📊 Pandas  
- 📈 Matplotlib, 🖌️ Seaborn  
- ⚖️ imbalanced-learn (**SMOTE**)  
- 🤖 Scikit-learn  
- 💾 Joblib  

**📌 Machine Learning Workflow:**  
- Classification Models: Logistic Regression, Decision Tree, Random Forest, AdaBoost, Gradient Boosting  
- Data Scaling: StandardScaler  
- Resampling: SMOTE  
- Model Evaluation: Accuracy, Precision, Recall, F1-Score, ROC-AUC, Confusion Matrix  

**📌 Tools & Environment:**  
- 📝 Jupyter Notebook  
- 💻 VS Code  
- 🔗 Git & GitHub  

---

## 📌 Conclusion  
This project shows how **machine learning** can be applied in **financial risk prediction**.  
It can be scaled for **banking systems**, **risk dashboards**, and **credit scoring applications**.  

---

## 📬 Contact  
🔗 **LinkedIn:**(https://www.linkedin.com/in/drjithapnair/)  
