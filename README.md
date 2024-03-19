# Heart_Failure_Prediction_Project

## [Input CSV file](heart_.csv)

This project involves the prediction of heart failure using 11 features which are:
------------------------------------------------------------------------------
- `Age`: age of the patient [years],
-`Sex`: sex of the patient [M: Male, F: Female],
-`ChestPainType`: chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic],
-`RestingBP`: resting blood pressure [mm Hg],
-`Cholesterol`: serum cholesterol [mm/dl],
-`FastingBS`: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise],
-`RestingECG`: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST: elevation or depression of > 0.05 mV), 
- `LVH`: showing probable or definite left ventricular hypertrophy by Estes' criteria],
-`MaxHR`: maximum heart rate achieved [Numeric value between 60 and 202],
-`ExerciseAngina`: exercise-induced angina [Y: Yes, N: No],
-`Oldpeak`: oldpeak = ST [Numeric value measured in depression],
-`ST_Slope`: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping],
-`HeartDisease`: output class [1: heart disease, 0: Normal]
-------------------------------------------------------------------------------

# Algorithm used for classification the heart failure prediction
## [1)Logistic regression](https://github.com/NANDHAKUMAR-PERIYANNAN/Heart_Failure_Prediction_Project/blob/main/Logisticregression_model.ipynb)
Logistic regression is a statistical method used for binary classification tasks, such as predicting whether an event will occur or not.
In the context of heart failure prediction, logistic regression analyzes patient data (features like age, sex, cholesterol levels, etc.) to calculate the probability of the patient experiencing heart failure.
It estimates the probability using a logistic function, which maps input features to a value between 0 and 1, representing the probability of the positive class (heart failure).
Logistic regression learns the relationship between input features and the binary outcome (heart failure or no heart failure) by adjusting coefficients during training.
During prediction, logistic regression classifies patients as either having a high or low risk of heart failure based on the calculated probability threshold.

## [2)RandomForestClassifier](Randomforestclassifier_model.ipynb)
Random forest classifier is an ensemble learning method based on decision trees.It works by creating multiple decision trees during training, each based on a random subset of the input features and data samples.Each decision tree independently predicts the outcome (heart failure or no heart failure) based on the input features.During prediction, the random forest aggregates the predictions from all decision trees to make a final prediction. It typically uses voting or averaging to determine the majority prediction.Random forest classifier is robust to overfitting and can handle large datasets with high dimensionality effectively.It's capable of capturing complex relationships between input features and the target variable, making it suitable for heart failure prediction tasks



# Sample Datasets given to test both model
![sample_Input](https://github.com/NANDHAKUMAR-PERIYANNAN/Heart_Failure_Prediction_Project/assets/93268682/f8905806-89e6-4a1a-b054-fc057d452918)

# Output corresponding to the datasets given to both model
![result](https://github.com/NANDHAKUMAR-PERIYANNAN/Heart_Failure_Prediction_Project/assets/93268682/87a658d7-f16a-4bf4-8adf-9b2b7cf5a399)

# Evaluation of model performance with 70:30(training:testing) from 918 datasets
![Evaluating the model_logistic regression](https://github.com/NANDHAKUMAR-PERIYANNAN/Heart_Failure_Prediction_Project/assets/93268682/bb444900-268c-4c34-9a3a-fd3dfc67e753)
![classification_report_logisticregression](https://github.com/NANDHAKUMAR-PERIYANNAN/Heart_Failure_Prediction_Project/assets/93268682/f7eff60f-bb04-43cd-94c6-272765fa2134)

_'Tools used'_:_Pandas and Numpy for dataframe,matrix||matplotlib and seaborn for visualization||Pickle for conversion of algorithm into ML model_

