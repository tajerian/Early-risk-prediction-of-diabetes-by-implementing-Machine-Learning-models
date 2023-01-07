# DM_Dx: diabetes early prediction 

This study intends to develop Machine learning algorithms to predict diabetes risk and compare ML models with conventional statistical methods like Logistic Regression to find the superior technique for diabetes prediction.
the best way to use these models for diabetes prediction is to use its coresponding [web applicaton](https://github.com/tajerian/DM_Dx-APP).

### requirements:

    !pip install tensorflow
    !pip install scikit-learn
    !pip install xgboost
    !pip install joblib

### preprosesing
for all models except the Decision tree, you need to preprocess data using the scalar model.

    from joblib import load
    scaler = load('.../scaler.joblib') 
    x_scaled = scaler.transform(x)


### data entry array
the instances variables should be given to the models in this order:
[[Age, PF, BMI, Insulin level, Skin Thickness, Blood Pressure, Glucose level, number of Pregnancies]]


### models comparison
![enter image description here](https://github.com/tajerian/diabetes_Dx_ML/blob/main/Figure%205,ROC.png?raw=true)
