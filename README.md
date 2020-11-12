# Used-Car-Price-Prediction-MLR-Evaluation-Result
Python Data Science Project, Used Car Price Prediction using MLR algo with 98.27% accuracy, RMSE: 1148, MAE: 828, Mallow's_CP: 0.004, D_Watson: 2.17, No Multicollinearity, Homoscedastic Residual/Error Distribution

## About the Car Price Prediction

Price is Target variable & 27 Features are PriceCategory, Company, Aspiratiion, Carbody, Drivewheel, Wheelbase, Carlength, Carwidth, Curbweight, Enginetype, Cylindernumber, Enginesize, Fuelsystem, Boreratio, Horsepower, CityMileage, HighwayMileage, HP-Category, Enginelocation, Stroke, Fueltype, Peakrpm, Doornumber, Compressionratio, Carmodel, Carheight, InsuranceRisk

## Project Overview

In this Project I have unleashed the useful Data Science insights using this CAR Price datasets and performed the feature selection precisely to build multiple linear regression model by combining the power of best statistical rules & principles to maximise accuracy at its best. The best thing is my model is not having Multicollinearity & Heteroscedasticity problem problem.

## This Project is divided into 26 major steps which are as follows:

1. [Check out the Data](#data-check)
2. [Importing Libraries & setting up environment](#imp-lib)
3. [Loading dataset](#data-load)
4. [Data Cleaning & Preprocessing](#prep-clean)
5. [Shapiro for Normality test of All Numeric Columns](#shapiro-norm)
6. [Spearman Correlation Test for Measures of Association between non-normal Datas](#spear-corr)
7. [Outlier Treatment/Check](#out-check)
8. [Skewness Check](#skew-check)
9. [Exploratory Data Analysis ( EDA )](#data-expo)
10. [Measures of Association between Continuous and Categorical Variables](#cat-measure)
11. [New Feature Creation](#new-feature)
12. [Removal/Selection of Categorical Features](#feature-select)
13. [Saving The Cleaned CAR DataFrame](#save-clean)
14. [Assigning Label & Features](#Labe-Feature)
15. [Features Encoding Technique](#Features-Encoding)
16. [Scaling of Numeric Features](#scale-feature)
17. [Train & Test Split](#data-split)
17. [Features P-Value & VIF Check](#p-vif)
18. [Final Implimentation of the MLR Model](#final-model)
19. [Model Evaluation](#mod-eval)
20. [Actual vs Predicted Price of Used CAR](#actual-predicted)
21. [Residual Distribution of Predicted Used CAR Price](#re-dit)
22. [Amount of Error in Used CAR Price Prediction](#amt-er)
23. [Durbin Watson Auto-Correlation Test](#dur-wat)
24. [Regression Evaluation Metrics](#mod-eval)
25. [Plotting the Regression Line](#reg-plot)
26. [Heteroscedasticity Tests](#het-test)
27. [Auto-Correlation plot](#auto-plot)

## About Data

This dataset consists of 27 features and a target variable. It has 9 nominal variables, 13 numeric variables, 5 ordinal variables. The detailed description of all the features are as follows:

**1. wheelbase, carlength, carwidth, carheight, curbweight, enginesize, boreratio, stroke, compressionratio, horsepower, CityMileage, HighwayMileage, Peakrpm:** These are all numeric features.
**2. Carbody, Enginelocation, aspiration, company, drivewheel, enginetype, fueltype, fuelsystem, carmodel :** These are all nominal features.
**3. Chest Pain Type:** Type of chest pain experienced by patient categorized into 1 typical, 2 typical angina, 3 non-anginal pain, 4 asymptomatic (Nominal)<br>
**4. resting bp s:** Level of blood pressure at resting mode in mm/HG (Numerical)<br>
**5. cholestrol:** Serum cholestrol in mg/dl (Numeric)<br>
**6. fasting blood sugar:** Blood sugar levels on fasting > 120 mg/dl represents as 1 in case of true and 0 as false (Nominal)<br>
**7. resting ecg:** Result of electrocardiogram while at rest are represented in 3 distinct values 0 : Normal 1: Abnormality in ST-T wave 2: Left ventricular hypertrophy (Nominal)<br>
**8. max heart rate:** Maximum heart rate achieved (Numeric)<br>
**9. exercise angina:** Angina induced by exercise 0 depicting NO 1 depicting Yes (Nominal)<br>
**10. oldpeak:** Exercise induced ST-depression in comparison with the state of rest (Numeric)<br>
**11. ST slope:** ST segment measured in terms of slope during peak exercise 0: Normal 1: Upsloping 2: Flat 3: Downsloping (Nominal)<br>
