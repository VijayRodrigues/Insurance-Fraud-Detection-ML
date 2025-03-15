# 🚗 Insurance Claims Fraud Detection  

## 📌 Problem Statement  
Insurance fraud is a major challenge in the industry, leading to **billions of dollars in losses** every year. Fraudulent claims not only **increase operational costs** but also impact **honest policyholders**. Identifying fraud accurately is crucial for insurers to **minimize risks and optimize claim processing**.  

This project aims to develop a **Machine Learning model** that can predict **fraudulent insurance claims** based on **customer details, policy information, and accident reports**.  

---

## 🎯 Objectives  
✔️ Perform **Exploratory Data Analysis (EDA)** to understand fraud trends  
✔️ Apply **Feature Engineering** to improve model accuracy  
✔️ Train and evaluate **Machine Learning models** for fraud detection  
✔️ Interpret results and generate insights for insurers  

---

## 📂 Dataset  
We will be using an **auto insurance dataset** that contains:  
- **Customer Details** (Age, Gender, etc.)  
- **Policy Information** (Coverage, Vehicle Type, etc.)  
- **Accident Reports** (Cause, Severity, etc.)  
- **Claim Details** (Amount, Status: Fraud/Legit)  

📥 **Download Dataset**: [Automobile Insurance Fraud Data](https://github.com/dsrscientist/Data-Science-ML-Capstone-Projects/blob/master/Automobile_insurance_fraud.csv)  

---

## 🛠️ Technologies Used  
- **Python** 🐍  
- **Pandas & NumPy** 📊 – Data Manipulation  
- **Matplotlib & Seaborn** 📈 – Data Visualization  
- **Scikit-learn** 🤖 – Machine Learning  
- **XGBoost & Random Forest** 🌲 – Advanced ML models  

---

## 📊 Expected Outcomes  
✅ Identify **patterns and key factors** in fraudulent claims  
✅ Develop a **predictive model** to classify claims as **fraudulent or legitimate**  
✅ Provide **data-driven insights** to help insurers reduce fraud  
✅ Optimize **claim processing workflows** to improve efficiency  

---

## 📜 Project Structure  
```bash
Insurance-Fraud-Detection/
│
├── data/
│   ├── raw/
│   │   └── insurance_fraud.csv      # Original dataset
│   ├── processed/
│   │   └── cleaned_data.csv         # Processed and cleaned dataset
│
├── notebooks/
│   ├── EDA.ipynb                    # Exploratory Data Analysis
│   ├── Model_Training.ipynb         # Model training and evaluation
│   └── Feature_Engineering.ipynb    # Feature selection and engineering
│
├── models/
│   └── fraud_detection_model.pkl    # Trained Machine Learning model
│
├── src/
│   ├── data_preprocessing.py        # Data cleaning and preprocessing
│   ├── model_training.py            # Model training and evaluation
│   ├── utils.py                     # Utility functions
│
├── results/
│   ├── feature_importance.png       # Feature importance visualization
│   ├── fraud_detection_report.txt   # Final model evaluation report
│
├── tests/
│   ├── test_data_preprocessing.py   # Unit tests for data preprocessing
│   └── test_model_training.py       # Unit tests for model training
│
├── README.md                        # Project documentation
├── requirements.txt                 # Dependencies
├── LICENSE                          # License file
└── .gitignore                       # Files to ignore in Git

```

## 🔍 Model Selection & Evaluation  

To detect fraudulent insurance claims, I evaluated multiple machine learning models using **Receiver Operating Characteristic (ROC) curves** and **Area Under the Curve (AUC) scores** to compare their effectiveness. The models I tested include:  

✔️ **Decision Tree Classifier**  
✔️ **Random Forest Classifier**  
✔️ **Gradient Boosting Classifier**  
✔️ **AdaBoost Classifier**  
✔️ **Extra Trees Classifier**  

### **📊 Model Performance Insights**  

- **AUC Scores:** Higher AUC indicates better discrimination between fraudulent and genuine claims.  
- **Top Performers:** **Extra Trees Classifier** & **Random Forest Classifier** showed the best results with an AUC score of **0.95**, making them the most effective models for fraud detection.  
- **Lowest Performer:** **Decision Tree Classifier** had the lowest AUC (**0.79**), indicating weaker predictive power.  
- **Visual Comparison:** ROC curves provide a graphical representation of True Positive Rate (TPR) vs. False Positive Rate (FPR) for each model.  

### **🛠 Model Implementation**  
I used **scikit-learn** to implement these models and evaluate their performance using:  

🔹 `plot_roc_curve` – For visualizing model comparisons.  
🔹 `confusion_matrix`, `precision`, `recall`, `F1-score` – For detailed performance metrics.  

By leveraging **ensemble models like Random Forest and Extra Trees**, I improved the accuracy and robustness of fraud detection.  
