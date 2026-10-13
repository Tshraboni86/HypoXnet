# HypoXNet: A Clinical Decision Support for Hypothyroid Pregnancy Prediction Using Data-Driven Approach

> **Accepted Paper**  
> _2026 IEEE International Conference on Optics, Machine Learning and Emerging Technology (OMLET)_  
> October 29–31, 2026 | Nairobi, Kenya

---

## 📌 Abstract

Hypothyroidism in pregnancy is associated with miscarriage, premature delivery, low birth weight, and abnormal neurodevelopment in the fetus. Diagnosis remains difficult in resource-poor healthcare facilities where laboratory testing is limited and clinical symptoms overlap with normal pregnancy.

This study introduces **HypoXNet**, a hybrid clinical decision support system for early hypothyroidism detection in pregnancy. Built using structured clinical data gathered from 1,000 pregnant women across two tertiary hospitals in Bangladesh, the framework integrates:

- **Hybrid Architecture:** Combines **XGBoost** and a **Multilayer Perceptron (MLP)** via an adaptive attention-based fusion method for complementary feature learning across tree-based and non-linear patterns.
- **Explainability (XAI):** Employs **SHAP** (SHapley Additive exPlanations) to identify key clinical biomarkers and increase model transparency for healthcare providers.
- **Physician Support:** Integrates a lightweight **Phi-3 Mini** Large Language Model (LLM) to generate physician-oriented clinical recommendations based on prediction outcomes.

---

## 📊 Experimental Setup & Performance

- **Validation Strategy:** Stratified 5-Fold Cross-Validation.
- **Accuracy:** **96.81%** overall predictive accuracy.
- **Baselines Comparison:** Evaluated against baseline algorithms (**RFC, SVC, DTC, KNN, standalone MLP, XGB**) and hybrid variants (**RFC+MLP, SVM+MLP**) to support ablation analysis.
- **Evaluation Metrics:** Accuracy, Precision, Sensitivity, Specificity, F1-score, and ROC-AUC.

---

## 🛠️ Repository File Structure

- `hypo_thyroid.ipynb`: Complete Jupyter Notebook containing data preprocessing, feature engineering, model training, SHAP explainability analysis, and LLM inference.
- `requirements.txt`: Python package dependencies required to reproduce the environment.
- `README.md`: Project summary and conference publication details.
