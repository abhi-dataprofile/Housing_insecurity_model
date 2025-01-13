# Housing_insecurity_model

# Project Description: Predictive Model for Housing Insecurity in Medicare Members

## **Objective**  
To build a predictive model to identify Medicare members most likely to experience housing insecurity, a significant Health-Related Social Need (HRSN), and provide actionable insights for targeted interventions to improve overall health outcomes.

---

## **Methodology**

### 1. Data Exploration and Preprocessing
- Performed Exploratory Data Analysis (EDA) to understand demographic and behavioral attributes contributing to housing insecurity.
- Applied class-balancing techniques, such as SMOTE, to address data imbalance (~4.4% positive cases).
- Created derived features, including healthcare cost burden and urgent care utilization.
- Supplemented dataset with external socioeconomic indicators (e.g., neighborhood income).

### 2. Model Development
- Trained multiple supervised learning models: **Random Forest**, **XGBoost**, and **Logistic Regression**.
- Applied hyperparameter tuning and cross-validation for robust performance.
- Evaluated performance using accuracy, precision, recall, F1-score, and AUC-ROC.

### 3. Explainability and Interpretability
- Used **SHAP** (SHapley Additive exPlanations) to visualize contributing features, ensuring model transparency.
- Highlighted key drivers of housing insecurity: `cons_homstat`, age, and low-income status.

---

## **Key Insights**
- Higher housing insecurity was observed among members living alone, lower-income categories, and older adults.
- Increased medical and urgent care claims correlated with higher housing insecurity.
- The **XGBoost** model demonstrated superior performance (**AUC-ROC: 0.74**), indicating its suitability for predictions.


---

## **Next Steps**
1. **Production Deployment:**
   - Deploy the model within internal Medicare support systems.
2. **Feedback Collection:**
   - Collect feedback from case managers and iterate to improve prediction accuracy.
