# Predicting Mental Health Treatment from Workplace Factors

This project builds a machine learning model to predict whether an employee seeks mental health treatment based on workplace-related factors.

---

## 📊 Overview

The goal is to understand how workplace conditions relate to treatment-seeking behavior.

The project focuses on:

- data preprocessing and feature engineering  
- classification models  
- model evaluation and threshold tuning  
- extracting insights from the model


---


## 🗂 Data

This project uses the *Mental Health in Tech Survey (2014)* dataset.

Source: https://www.kaggle.com/datasets/osmi/mental-health-in-tech-survey

A small sample of the dataset is included in `data_sample/sample.csv`.


---


## ⚙️ Methodology

- Data cleaning and preprocessing (missing values, categorical encoding)  
- Feature selection focused on workplace-related variables  
- Models:
  - Logistic Regression  
  - Random Forest  
- Handling class imbalance with SMOTE  
- Evaluation using ROC AUC, precision, and recall  
- Threshold tuning to increase recall for the positive class  
  

---

## 📈 Pipeline Overview

The following diagram summarizes the full pipeline using in this project:

![Pipeline](images/project_architecture.png)


---


## 📈 Results

- Logistic Regression performed best on the test set  
- ROC AUC ≈ 0.80  

Key observations:

- mental health interfering with work is the strongest signal  
- access to care options and benefits matters  
- workplace openness also plays a role

  
---


## ▶️ How to Run

Install dependencies:

```bash
pip install -r requirements.txt
```


---


## 📝 Notes

- Data comes from self-reported survey responses  
- The model shows relationships, not cause and effect  
- Results may not generalize beyond the tech industry  


---


## 🚀 Next Steps

- test additional models  
- include more features  
- validate results on other datasets  
- deploy the model as an API  
