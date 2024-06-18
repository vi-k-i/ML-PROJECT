# ML-PROJECT
Framingham Heart Study - 10-Year CHD Risk Prediction
Project Description:
The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients’ information. It includes over 4,000 records and 15 attributes. Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk factors.
Dataset Information
The dataset consists of the following 15 attributes:
age: Age of the patient.
sex: Gender of the patient (0 = female, 1 = male).
education: Level of education.
currentSmoker: Whether the patient is a current smoker (0 = No, 1 = Yes).
cigsPerDay: Number of cigarettes smoked per day.
BPMeds: Whether the patient is on blood pressure medication (0 = No, 1 = Yes).
prevalentStroke: Whether the patient has had a stroke (0 = No, 1 = Yes).
prevalentHyp: Whether the patient has hypertension (0 = No, 1 = Yes).
diabetes: Whether the patient has diabetes (0 = No, 1 = Yes).
totChol: Total cholesterol level.
sysBP: Systolic blood pressure.
diaBP: Diastolic blood pressure.
BMI: Body Mass Index.
heartRate: Heart rate.
glucose: Glucose level.
The target variable is TenYearCHD, which indicates whether the patient has a 10-year risk of coronary heart disease (0 = No, 1 = Yes).
Business Context:-
Coronary heart disease is a major cause of death worldwide. Early prediction of the risk of developing CHD can help in taking preventive measures and reduce the mortality rate. This model aims to aid healthcare professionals in identifying high-risk individuals and providing them with the necessary interventions.
Dependencies
To run this project, you need the following libraries:
pandas
numpy
matplotlib
seaborn
scikit-learn
imbalanced-learn
xgboost
statsmodels.stats.outliers_influence

Project Workflow
Data Collection: Gather the dataset.
Data Cleaning: Handle missing values, outliers, Exploratory Data Analysis
Cleaning and Manipulating dataset
Univariate Analysis
Bivariate Analysis
Removing Multicolinearity
Model building
Logistic Regression
Naive Bayes Classifier
Support Vector Classifier
Random Forest Classifier
XGBoost Classifier
KNN Classifier

Conclusion
1). If we want to completely avoid any situations where the patient has heart disease, a high recall is desired. Whereas if we want to avoid treating a patient with no heart diseases a high precision is desired.

2). Assuming that in our case the patients who were incorrectly classified as suffering from heart disease are equally important since they could be indicative of some other ailment, so we want a balance between precision and recall and a high f1 score is desired.

3). Since we have added synthetic datapoints to handle the huge class imbalance in training set, the data distribution in train and test are different so the high performance of models in the train set is due to the train-test data distribution mismatch and not due to overfitting.

Best performance of Models on test data based on evaluation metrics for class 1:

Recall - SVC
Precision - Naive Bayes Classifier
F1 Score - Logistic Regression, XGBoost
Accuracy - Naive Bayes Classifier

References
Framingham Heart Study
Imbalanced-learn Documentation
