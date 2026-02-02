# Predicting Car Insurance Claims with Cloud-Based Machine Learning on AWS

This repository showcases a cloud-based machine learning solution to predict **car insurance claim occurrence and cost** using a two-stage modeling framework.  

---

## Project Overview  

### Objective  
The goal of this project is to build a **scalable and automated machine learning pipeline on AWS** that:
- Predicts whether a customer will file a claim  
- Estimates the expected claim amount when a claim is predicted  

This approach mimics real insurance workflows and improves efficiency through conditional model execution.

---

## Key Features  

- **Two-Stage Prediction:**  
  Claim occurrence (classification) → Claim cost (regression)  

- **Cloud-Based Architecture:**  
  Data storage, preprocessing, training, and deployment on AWS  

- **Conditional Execution:**  
  Cost model runs only when a claim is predicted, reducing compute usage  

- **Imbalance Handling:**  
  SMOTE applied to improve detection of risky customers  

- **Explainability:**  
  SHAP used to identify key risk drivers  

---

## Problem Statement  

Insurance companies collect large volumes of customer and policy data but struggle to:
- Accurately predict claims  
- Estimate financial risk  
- Scale analytics systems efficiently  

This project addresses these challenges by combining **prediction, cost estimation, and cloud deployment** into a single automated workflow.

---

## Dataset  

- **Source:** Car Insurance Claim Dataset (Kaggle)  
- **Records:** 10,302  
- **Targets:** Claim flag (yes/no), Claim amount  
- Includes customer, vehicle, and driving history features

---

## Models Used  

- **Claim Prediction:** Logistic Regression, Random Forest  
- **Claim Cost Estimation:** Random Forest Regressor  

---

## Results Summary  

- Claim prediction model achieved **strong discrimination (ROC-AUC ≈ 0.81)**  
- Cost estimation captured overall claim trends despite high variability  
- Two-stage pipeline enables policy-level expected loss estimation  

---

## Business Impact  

- **Improved Risk Assessment:** Helps insurance teams identify customers who are more likely to file claims, supporting better pricing and risk decisions.  

- **Cost Efficiency:** Runs the claim cost model only when needed, reducing unnecessary system usage and saving cloud resources.  

- **Operational Scalability:** Built on AWS, making it easy to scale across large datasets and real-world business environments.  

- **Transparent Insights:** Uses explainable methods to show which factors influence risk and cost, increasing trust in the predictions.

---

## Technologies Used  

- **Cloud:** AWS S3, AWS SageMaker  
- **ML:** Scikit-learn, Random Forest, Logistic Regression  
- **Explainability:** SHAP  
- **Visualization:** Matplotlib, Seaborn  

---

## Getting Started  

You can download the notebook files from this repository and run them locally using Jupyter Notebook.

---
