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

**2. Carbody, Enginelocation, aspiration, company, drivewheel, enginetype, fueltype, fuelsystem, carmodel:** These are all nominal features.

**3. InsuranceRisk, Doornumber, Cylindernumber, PriceCategory, HP-Category:** These are all Ordinal features.

## Selected Features for the Model

**1. Carwidth:**

**2. Cylindernumber:** Cylindernumber (5 & 4)

**3. PriceCategory:** PriceCategory (Luxuary, Premium, Standard)

**4. HP-Category:** HP-Category (Heavy-HP, Standard-HP)

**5. Company:** Company (BMW, PORSCHE)

**6. aspiration:** aspiration (turbo)

**7. carbody:** carbody (convertible)
