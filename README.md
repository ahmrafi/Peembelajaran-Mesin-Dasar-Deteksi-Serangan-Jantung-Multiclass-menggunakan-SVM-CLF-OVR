# Heart Disease Classification Project

This project focuses on early detection, risk management, and diagnosis optimization of heart disease using data science techniques. The study utilizes various support vector machine (SVM) classification methods to achieve high accuracy in heart disease diagnosis, ensuring that healthcare resources are efficiently utilized.

## Background

Heart disease is a major health concern worldwide, requiring accurate and timely diagnosis to prevent serious outcomes such as heart attacks and heart failure. This project aims to:

- Improve early detection and diagnosis to reduce misdiagnosis and prevent inappropriate treatments.
- Develop long-term prevention and management strategies to reduce the risk of severe cardiovascular conditions.
- Optimize healthcare resources by aligning treatments with precise diagnoses.

## Data Preparation

The dataset consists of 922 records with 16 features, which include:

- **Patient Details**: `id`, `age`, `sex`, `origin`
- **Clinical Measurements**: `cp` (chest pain type), `tr`, `estbps` (resting blood pressure), `chol` (serum cholesterol), `fbs` (fasting blood sugar), `restecg` (electrocardiographic results), `thalach` (max heart rate achieved), `exang` (exercise-induced angina), `oldpeak` (ST depression), `slope` (ST segment slope), `ca` (major vessels count), `thal`
- **Target Variable**: `num` (predicted heart disease attribute)

### Data Processing Steps

1. **Data Preparation**:
   - Categorical and numerical variables were analyzed.
   - A correlation matrix was created to understand feature relationships.
   
2. **Resampling**:
   - The `num` target class was balanced through resampling to improve model training.

3. **Preprocessing**:
   - Labels were assigned to classes.
   - Standardization was applied to ensure consistency across features.

## Methods

Two primary SVM classification approaches were used:

1. **Chi-square Feature Selection with SVM**:
   - Kernel RBF: Accuracy of 64%
   - Kernel Poly: Accuracy of 71%

2. **Variance Threshold Feature Selection with SVM**:
   - Classifiers: One-vs-One (OVO) and One-vs-Rest (OVR)
   - Achieved the highest accuracy of 93% with consistent precision and recall across categories.

## Conclusion

The results indicate that the Variance Threshold method with SVM CLF classifiers (both OVO and OVR) yields the highest accuracy at 93%. This method outperformed the Chi-square SVM approaches and demonstrated reliable precision and recall, making it the most effective approach for heart disease classification in this study.

## References

Further reading and resources can be found in the original presentation.

---

**Developed by**: Claudia Alves
