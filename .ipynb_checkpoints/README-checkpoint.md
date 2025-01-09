# Thyroid Risk Prediction Project

## Project Overview

The Thyroid Risk Prediction project aims to investigate the factors influencing thyroid disorders by analyzing a dataset of clinical and demographic features. Utilizing advanced statistical and machine learning methods, the project seeks to develop predictive models that accurately assess the risk of thyroid disorders in individuals. This initiative is crucial for improving early detection and risk stratification, ultimately enhancing patient outcomes and optimizing healthcare resources.

## Project Understanding

Thyroid disorders are prevalent globally, affecting a significant portion of the population. Early detection and intervention are critical to preventing severe health complications associated with these disorders. The project addresses the gap in utilizing data-driven approaches for predicting thyroid disorders, focusing on developing robust statistical models and machine learning algorithms.

## Problem Statement

Thyroid disorders affect approximately 3.05% of the population with hypothyroidism and 0.75% with hyperthyroidism, while around 6.71% remain undiagnosed (American Thyroid Association, 2020). Women are five to eight times more likely to develop thyroid problems compared to men, and one in eight women will develop a thyroid disorder during her lifetime (American Thyroid Association, 2020).  Despite advances in medical diagnostics, there remains a gap in utilizing data-driven approaches for predicting thyroid disorders. Existing research primarily focuses on clinical evaluations and biochemical tests. This project addresses this gap by developing robust statistical models and machine learning algorithms to predict thyroid risk levels using a comprehensive sample dataset.

## Stakeholders

- Healthcare Providers: Endocrinologists and general practitioners who diagnose and treat thyroid disorders.
- Researchers: Medical researchers and data scientists focused on endocrinology and predictive modeling.
- Patients: Individuals at risk of thyroid disorders who would benefit from early detection and intervention.
- Healthcare Organizations: Hospitals, clinics, and public health departments interested in improving thyroid disorder management.

## Data Description

The dataset comprises various clinical and demographic features, including:

- Age: Recorded in years.
- Gender: Denoted as 1 for male and 0 for female.
- Pregnancy Status: Indicated by 1 if pregnant and 0 otherwise.
- Family History of Thyroid Disorders: Noted with 1 for yes and 0 for no.
- Presence of Goiter: Marked as 1 for yes and 0 for no.
- Symptoms: Fatigue, weight changes, hair loss, heart rate changes, sensitivity to cold or heat, increased sweating, muscle weakness, constipation or more bowel movements, depression or anxiety, difficulty concentrating or memory problems, dry or itchy skin.
- Thyroid Risk Level: Classified as 0 for no risk, 1 for moderate risk, and 2 for high risk.

The dataset is structured in a tabular format with binary (0/1) and integer values, containing 10,506 rows and 17 columns.

## Objectives

### Main Objectives

- To develop and validate predictive models for assessing thyroid disorder risk using demographic and clinical features.

- To identify the most significant predictors of thyroid disorders and evaluate the performance of various machine learning algorithms.

### Other Objectives

- To analyze the dataset for significant clinical and demographic features that influence thyroid disorders.

- To compare the performance of different machine learning algorithms in predicting thyroid disorder risk.

## Research Questions

1. What demographic and clinical features are most predictive of thyroid disorders?

2. How do different machine learning algorithms compare in terms of accuracy and reliability for predicting thyroid disorders?

3. What is the impact of early detection on patient outcomes in thyroid disorder cases?

4. How can predictive modeling be integrated into clinical practice for better management of thyroid disorders?

## Methodology

The project employs a combination of statistical analysis and machine learning techniques, including:

- Data Preprocessing: Cleaning and preparing the dataset for analysis.
- Exploratory Data Analysis (EDA): Conducting univariate, bivariate, and multivariate analyses to understand the relationships between features and the target variable.
- Feature Selection: Identifying the most important predictors of thyroid disorders.
- Model Development: Implementing various machine learning algorithms, including Logistic Regression, Decision Trees, Random Forest, Support Vector Machines, K-Nearest Neighbors, Neural Networks, AdaBoost, Gradient Boosting, and XGBoost.
- Model Evaluation: Assessing model performance using metrics such as accuracy, precision, recall, and F1-score.

## Results and Findings

### Univariate Analysis

- Analysis of individual features to understand their distribution and significance in predicting thyroid disorders.

<img src="Data/UN3.png" alt="Mean, Mode and Median of Age" height="800" width="600">

The average age for males is 53, while for females it is 54. The most common age (mode) for males is 73, whereas for females it is 80. The median age for males is 53, and for females, it is 54. 

<img src="Data/UN1.png" alt="Thyroid Risk Levels Based on Features" height="2000" width="1600">

The highest count is in the 51-60 age group, while the youngest (11-20) and oldest (91-100) age groups have the lowest counts.
Females slightly outnumber males in terms of gender distribution. A slightly higher number of individuals do not have a family history of thyroid issues, goitre, fatigue, weight changes, hair loss, heart rate changes, temperature sensitivity, increased sweating, muscle weakness, bowel movement changes, depression/anxiety, concentration/memory issues, and dry itchy skin compared to those who do.

<img src="Data/UN2.png" alt="Thyroid Risk Levels Based on Features" height="800" width="600">

According to pregnancy distribution, 2818 females are not pregnant while 2517 are pregnant. 
    
### Bivariate Analysis

- Examination of relationships between pairs of features and their impact on thyroid risk levels.

<img src="Data/BA3.png" alt="Thyroid Risk Levels Based on Age Group" height="800" width="600">   

In the No Risk category, the 71-80 age group has the highest count, followed by the 51-60 age group. The 91-100 and 11-20 age groups have the lowest counts. In the Moderate Risk category, the 81-90 age group has the highest count, followed by the 61-70 age group, with the 91-100 and 11-20 age groups having the lowest counts. In the High Risk category, the 41-50 age group has the slightly highest count, followed by the 21-30 age group, while the 91-100 and 11-20 age groups have the lowest counts
                                                
<img src="Data/BA1.png" alt="Thyroid Risk Levels Based on Features" height="2000" width="1600">                                                

Females have higher counts in both the Moderate and No Risk categories, while males have slightly higher counts in the High Risk category, suggesting females might be more prone to thyroid issues or are diagnosed more frequently. Individuals without a family history of thyroid issues are more common in the "No Risk" and "Moderate Risk" categories, whereas those with a family history are more prevalent in the High Risk category, indicating a significant correlation. The absence of goiter corresponds to the highest counts in the "No Risk" category, while its presence is linked to higher counts in the Moderate and High Risk categories. Fatigue, weight changes, hair loss, heart rate changes, temperature sensitivity, increased sweating, muscle weakness, bowel movement changes, depression/anxiety, concentration/memory issues, and dry itchy skin all show strong associations with increased thyroid risk levels, as their absence is typically found in the lower risk categories, while their presence is more common in the higher risk categories.

<img src="Data/BA2.png" alt="Thyroid Risk Levels Based on Pregnancy" height="800" width="600">    

Pregnant females have a higher count in the Moderate Risk category and a slightly higher count in the No Risk category. Non-pregnant females have a slightly higher, yet similar count to pregnant females, in the High Risk category.
        
### Multivariate Analysis

- Exploration of interactions among multiple features to identify complex relationships influencing thyroid disorders.
                                            
<img src="Data/MA.png" alt="Multivariate Analysis" height="1000" width="800">

The presence of goiter, fatigue, significant weight changes, hair loss, heart rate changes, sensitivity to temperature, increased sweating, muscle weakness, bowel movement changes, depression/anxiety, concentration/memory issues, and dry itchy skin are strongly correlated with higher thyroid risk levels. These symptoms suggest various physiological and psychological implications of thyroid disorders. Conversely, a slight negative correlation is observed with gender, indicating males are less likely to have thyroid issues compared to females, and pregnancy, which suggests it may not be a significant standalone risk factor for thyroid issues.

## Machine Learning Models
                                                
Performance metrics for various models:
                                                
<img src="Data/ML.png" alt="Machine Learning Models" height="1000" width="800">

- K-Nearest Neighbors: Accuracy: 0.7005, Precision: 0.7033, Recall: 0.7005, F1-Score: 0.6939.

- Neural Networks: Accuracy: 0.6865, Precision: 0.7079, Recall: 0.6865, F1-Score: 0.6867.

- Logistic Regression: Accuracy: 0.6688, Precision: 0.6645, Recall: 0.6688, F1-Score: 0.6657.

- AdaBoost: Accuracy: 0.6507, Precision: 0.6444, Recall: 0.6507, F1-Score: 0.6467.

- Support Vector Machines: Accuracy: 0.6136, Precision: 0.6120, Recall: 0.6136, F1-Score: 0.6109.

- Naive Bayes: Accuracy: 0.5765, Precision: 0.6336, Recall: 0.5765, F1-Score: 0.5260.

## Conclusion

The project successfully developed predictive models for assessing thyroid disorder risk using demographic and clinical features. The findings underscore the importance of early detection and the potential of machine learning in improving healthcare outcomes for individuals at risk of thyroid disorders.

### Insights

- Symptoms such as fatigue, weight changes, and hair loss are strongly correlated with thyroid risk levels, indicating their significance in early detection.

### Model Performance

The models demonstrated varying levels of performance, with K-Nearest Neighbors achieving the highest accuracy among the tested algorithms. However, all models showed potential for further refinement and optimization.

### Recommendations

- Implement predictive modeling tools in clinical practice to enhance early detection and risk stratification of thyroid disorders.

- Educate healthcare providers on the significance of demographic and clinical features in assessing thyroid risk.

### Limitations

- The dataset may not encompass all relevant clinical and lifestyle factors influencing thyroid disorders.

- The models may require further validation with larger and more diverse datasets to improve robustness.

### Future Work

1. Expand Dataset: Collect more comprehensive data from diverse populations to improve model robustness.

2. Longitudinal Studies: Conduct longitudinal studies to track thyroid risk over time and refine predictive models.

3. Explore Additional Features: Investigate additional clinical and lifestyle factors that may influence thyroid disorders.

4. Real-World Application: Test the predictive models in real-world clinical settings to evaluate their practical utility.

5. Patient Education Programs: Develop educational programs for patients and healthcare providers on the importance of recognizing thyroid disorder symptoms and risk factors.

This README provides a comprehensive overview of the Thyroid Risk Prediction project, detailing its objectives, methodology, findings, and future directions. For further inquiries or collaboration opportunities, please contact the project team.