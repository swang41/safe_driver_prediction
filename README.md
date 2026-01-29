# Safe Driver Prediction: Insurance Risk Modeling

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![LightGBM](https://img.shields.io/badge/Model-LightGBM-green)
![SHAP](https://img.shields.io/badge/Interpretability-SHAP-orange)

## 📌 Overview
This project builds a predictive insurance risk model using a public auto insurance dataset to identify high-risk drivers. The core objective is to demonstrate how statistical machine learning—specifically Gradient Boosting—can be translated into actionable intervention segments and targeted risk-mitigation strategies.

## 📊 Dataset
* **Source:** [Porto Seguro Safe Driver Prediction (Kaggle)](https://www.kaggle.com/c/porto-seguro-safe-driver-prediction)
* **Description:** A tabular dataset featuring anonymized driver, vehicle, and policy-related features.
* **Problem Type:** Binary classification (predicting the probability of a claim).

## 🛠 Approach

### 1. Data Exploration & Preparation
* Managed missing values and sparse categorical features.
* Conducted feature screening and applied basic transformations to optimize model input.

### 2. Modeling & Evaluation
* **Baseline:** Logistic Regression.
* **Primary Model:** **LightGBM** (Gradient Boosted Decision Trees) to capture complex, non-linear relationships.
* **Metrics:** Focused on **AUC** and **Lift-by-Decile** analysis to evaluate how effectively the model ranks high-risk policyholders.



### 3. Interpretability & Intervention
* **XAI:** Leveraged **SHAP values** to identify key risk drivers at both a global and segment level.
* **Risk Tiering:** Segmented the population into Low, Medium, and High-risk tiers.
* **Simulation:** Conducted "what-if" scenarios to estimate the potential reduction in claim frequency through targeted safety interventions in the top risk deciles.

## 📈 Key Results
* **Ranking Performance:** LightGBM significantly outperformed the logistic baseline in identifying high-risk drivers.
* **Risk Concentration:** Lift analysis showed a strong concentration of actual claims within the top-predicted deciles.
* **Stakeholder Communication:** SHAP analysis provided a transparent view of the features driving risk, making the "black box" model explainable for business stakeholders.

## 💻 Tech Stack
* **Languages:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn
* **ML Frameworks:** LightGBM, SHAP
* **Visualization:** Matplotlib, Seaborn

## 💼 Resume Impact
* **Insurance Risk Modeling:** Built a gradient boosted model (LightGBM) using public auto insurance data, employing lift and decile analysis to identify high-risk policyholder segments.
* **Actionable Analytics:** Applied SHAP-based interpretability and risk tiering to translate model outputs into actionable intervention strategies for data-driven decision-making.