# Diabetes Risk Prediction Project

## Introduction
Diabetes is a serious chronic disease that affects the body's ability to regulate blood glucose levels, leading to complications such as heart disease, vision loss, amputations, and kidney disease. Early diagnosis and timely intervention can significantly reduce the impact of this disease. The goal of this project is to build a prediction model for diabetes risk based on the 2015 health survey dataset of 253,680 U.S. citizens.

## Dataset Description
The dataset used in this project is provided in the file `diabetes_012_health_indicators_BRFSS2015.csv` and contains 22 important variables, including:
- `Diabetes_012`: Diabetes status (0: no diabetes, 1: pre-diabetes, 2: diabetes).
- `HighBP`: Hypertension status (0/1).
- `HighChol`: High cholesterol status (0/1).
- `CholCheck`: Cholesterol check within the last 5 years (0/1).
- `BMI`: Body Mass Index.
- `Smoker`: Whether the individual has smoked at least 100 cigarettes in their lifetime (0/1).
- `Stroker`: Whether the individual has had a stroke (0/1).
- `HeartDiseaseorAttack`: Whether the individual has heart disease or a heart attack (0/1).
- `PhysActivity`: Physical activity in the last 30 days (0/1).
- `Sex`: Gender (0: female, 1: male).
- And several other health-related and demographic variables.

## Analysis Goals
1. **Analyze the Impact of Health Conditions on Diabetes Status**: Investigate the relationship between diabetes and various factors such as high blood pressure, high cholesterol, stroke, and lifestyle.
2. **Build a Diabetes Risk Prediction Model**: Develop classification models using algorithms such as Naive Bayes, Logistic Regression, LDA, and QDA to predict the likelihood of diabetes.
3. **Analyze Factors Affecting BMI**: Build a linear regression model to identify the factors influencing BMI, a crucial determinant for diabetes risk.

## Methods
1. **Data Preprocessing**:
   - Handle data imbalance using SMOTE and under/over-sampling methods.
   - Process outliers in quantitative variables.
   - Convert categorical variables to factors.

2. **Prediction Model Building**:
   - Implement classification models including Naive Bayes, Logistic Regression, LDA, and QDA.
   - Evaluate models using metrics like ROC curve, AUC, Confusion Matrix, F1-Score, Precision, and Recall.

3. **BMI Regression Analysis**:
   - Build a linear regression model to analyze the factors affecting BMI.
   - Check for multicollinearity and use Mallows' Cp to select the optimal model.

## Results
- The classification models showed that diabetes risk prediction has an accuracy of 52.5% on the test dataset.
- The BMI regression model identified significant factors such as high blood pressure, cholesterol, and smoking habits that affect BMI.

## Conclusion
This project provides valuable insights into the factors that influence diabetes risk and BMI. The results can support early intervention strategies and raise awareness about diabetes prevention in the community.

## References
- [CDC BRFSS Codebook 2015](https://www.cdc.gov/brfss/annual_data/2015/pdf/codebook15_llcp.pdf)
- [Diabetes Health Indicators Dataset on Kaggle](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset?select=diabetes_012_health_indicators_BRFSS2015.csv)
