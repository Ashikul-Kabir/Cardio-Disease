# Cardiovascular-Disease-Prediction
This analysis helps predict cardiovascular diseases in human body based on existing healthcare data available at Kaggle. The analysis is divided into the following layers:

1. Problem identification
2. Project goals and business impact
3. Dataset Overview
4. Analysis steps
5. Findings
6. Recommendations

# Problem Identification
- Problems With Inaccurate Predictions:
- Inaccurate heart disease prediction leads to preventable fatalities and increased healthcare burdens.
- Heart disease is a leading cause of mortality; early and accurate prediction can save lives and reduce treatment costs.
- Early detection is key to effective treatment.
- Enhancing predictive precision offers a pathway to alleviate strain on healthcare systems.

# Project Goals and business impact
This project aims to improve heart disease prediction by harnessing advanced machine learning techniques, ultimately saving lives and reducing healthcare costs. The primary goal is to develop an accurate predictive model that can identify heart disease risks earlier and more reliably, thereby assisting healthcare providers in making informed decisions and optimizing patient care. Successful implementation of this project will set new benchmarks in predictive healthcare, leading to more preventative care approaches, optimized healthcare resource management, and improved patient health outcomes.

# Dataset Overview
- Comprises of 70000 rows and 13 columns, representing individual patient records and medical attributes.
- Consists of clinical and physical parameters of patients.
- Output/Target Variable: Presence or absence of cardiovascular disease.

# Analysis Steps
- Data exploration using some descriptive statistics and visualizations.
- Implementing advanced data preprocessing techniques to seamlessly address missing values and categorical variables.
- Feature engineering and hyperparameter tuning to select and enhance model performance.
- Using classification models to predict class probabilities and determine accuracy.
- Selecting final model based on ROC-AUC area.

# Findings
- Random Forest showed improvement after hyperparameter tuning, with noticeable gains in both Precision and ROC-AUC.
- XGBoost also displayed improvement after hyperparameter tuning but to a lesser extent compared to Random Forest.
- LightGBM maintained consistent performance across all rounds, indicating its robustness to the dataset with slight improvement   in precision after hyperparameter tuning.
- Logistic Regression displayed a significant increase in performance after feature engineering, with accuracy increasing from    baseline and remaining stable through to hyperparameter tuning.
- considering the performance metrics across different rounds (Baseline, Post-Feature    
  Engineering, and Post-Hyperparameter Tuning), LightGBM has been elected as the most suitable model having the following key features:
-   Consistently High Performance
-   Slight Improvement with Complexity
-   Efficiency and Scalability
-   Feature Importance and Interpretability
-   Hyperparameter Sensitivity
-   Balanced Precision and ROC-AUC

# Recommendations
- Choosing the Best Model: LightGBM appears to offer the best combination of accuracy and ROC-AUC post-tuning, making it a strong candidate for the final model.
- Further Improvement: A granular hyperparameter tuning for LightGBM or XGBoost might be performed, as they showed the best performance. Advanced feature engineering techniques or ensemble methods may be explored to see if there's a significant performance boost.
- Model Interpretability: The interpretability of the model is a crucial aspect in healthcare applications, Logistic Regression might still be considered due to the ease of understanding its decision process, despite it not having the absolute highest metrics.
