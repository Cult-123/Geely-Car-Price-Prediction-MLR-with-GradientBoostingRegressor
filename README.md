# Used-Car-Price-Prediction-MLR-Evaluation-Result
Python Data Science Project, Used Car Price Prediction using MLR algo with 98.27% accuracy, RMSE: 1148, MAE: 828, Mallow's_CP: 0.004, D_Watson: 2.17, No Multicollinearity

## About the Car Price Prediction

Price is Target variable & Features are PriceCategory, Company, Aspiratiion, Carbody, Drivewheel, Wheelbase, Carlength, Carwidth, Curbweight, Enginetype, Cylindernumber, Enginesize, Fuelsystem, Boreratio, Horsepower, CityMileage, HighwayMileage.

## Project Overview

In this Project I will try to unleash useful insights using this CAR Price datasets and will perform feature selection to build multiple linear regression model by combining the power of best statistical rules & principles to maximise accuracy at its best. The best thing is my model is not having Multicollinearity problem.

This Project is divided into 13 major steps which are as follows:

1. [Check out the Data](#data-desc)
2. [Importing Libraries & setting up environment](#imp-lib)
3. [Loading dataset](#data-load)
4. [Data Cleaning & Preprocessing](#data-prep)
5. [Shapiro for Normality test of All Numeric Columns](#data-norm)
6. [Spearman Correlation Test for Measures of Association between non-normal Datas](#data-Spearman)
7. [Outlier Treatment/Check](#data-out)
8. [Skewness Check](#cross-skew)
9. [Exploratory Data Analysis ( EDA )](#data-eda)
10. [Measures of Association between Continuous and Categorical Variables](#model-cate)<br>
11. [New Feature Creation](#model-feature)<br>
12. [Removal/Selection of Categorical Features](#feature-select)
13. [Saving The Cleaned CAR DataFrame](#data-Clean)
14. [Assigning Label & Features](#Labe-Feature)
15. [Features Encoding Technique](#Features-Encoding)

## About Data

This dataset consists of 11 features and a target variable. It has 6 nominal variables and 5 numeric variables. The detailed description of all the features are as follows:

**1. Age:** Patients Age in years (Numeric)<br>
**2. Sex:** Gender of patient (Male - 1, Female - 0) (Nominal)<br>
**3. Chest Pain Type:** Type of chest pain experienced by patient categorized into 1 typical, 2 typical angina, 3 non-anginal pain, 4 asymptomatic (Nominal)<br>
**4. resting bp s:** Level of blood pressure at resting mode in mm/HG (Numerical)<br>
**5. cholestrol:** Serum cholestrol in mg/dl (Numeric)<br>
**6. fasting blood sugar:** Blood sugar levels on fasting > 120 mg/dl represents as 1 in case of true and 0 as false (Nominal)<br>
**7. resting ecg:** Result of electrocardiogram while at rest are represented in 3 distinct values 0 : Normal 1: Abnormality in ST-T wave 2: Left ventricular hypertrophy (Nominal)<br>
**8. max heart rate:** Maximum heart rate achieved (Numeric)<br>
**9. exercise angina:** Angina induced by exercise 0 depicting NO 1 depicting Yes (Nominal)<br>
**10. oldpeak:** Exercise induced ST-depression in comparison with the state of rest (Numeric)<br>
**11. ST slope:** ST segment measured in terms of slope during peak exercise 0: Normal 1: Upsloping 2: Flat 3: Downsloping (Nominal)<br>
