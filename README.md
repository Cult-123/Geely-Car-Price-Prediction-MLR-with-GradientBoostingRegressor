# Geely-Car-Price-Prediction-MLR-Evaluation-With-GradientBoostingRegressor-Result
Python Data Science Project, Geely Car Price Prediction using MLR algo with GradientBoostingRegressor:

![](Images/Car1.JPG)

- 99% accuracy (MLR)
- RMSE: 658 (MLR)
- MAE: 532 (MLR)
- D_Watson: 2.004
- Kurtosis/Peakedness=[M4/M2^2]=3.609 (MLR)
- Skewness=Mean-Mode=Positive=0.351 (MLR)
- Regression Model Overall F-test for Regression Line Slope = MSR/MSE = 150.3 (MLR)
- Mallow's_CP: 0.0060 (MLR)
- Probability (P-Value) of F-test for Regression Line Slope 3.26e-88 (MLR)
- Jack Bera (goodness-of-fit) for Regression Model Residuals Normal Distribution & the Value is 5.910 & the P-Value of it is 0.0521 (MLR)

![](Images/Car3.JPG)
![](Images/Car4.JPG)
![](Images/Car5.JPG)
![](Images/Car6.JPG)
![](Images/Car7.JPG)
![](Images/Car8.JPG)
![](Images/Car9.JPG)
![](Images/Car11.JPG)

- 98% accuracy (GradientBoostingRegressor with 10 Features)
- RMSE: 864 (GradientBoostingRegressor with 10 Features)
- MAE: 688 (GradientBoostingRegressor with 10 Features)
- D_Watson: 1.93
- Kurtosis/Peakedness=[M4/M2^2]=3.280 (GradientBoostingRegressor)
- Skewness=Mean-Mode=Positive=0.304 (GradientBoostingRegressor)
- Gradient Boosting Regression Model Overall F-test for model Line Slope = MSR/MSE = 280.2 (GradientBoostingRegressor)
- Mallow's_CP: 0.0040 (GradientBoostingRegressor with 10 Features)
- Probability (P-Value) of F-test for Regression Line Slope 6.15e-105 (GradientBoostingRegressor)
- Jack Bera (goodness-of-fit) for Regression Model Residuals Normal Distribution & the Value is 3.060 & the P-Value of it is 0.216 (GradientBoostingRegressor)
- No Multicollinearity
- Homoscedastic 'Residual/Error Distribution' in All Models
- No Autocorrelation in All Models 'Residual/Error Distribution'

## Problem Statement
A Chinese automobile company Geely Auto aspires to enter the US market by setting up their manufacturing unit there and producing cars locally to give competition to their US and European counterparts.

They have contracted an automobile consulting company to understand the factors on which the pricing of cars depends. Specifically, they want to understand the factors affecting the pricing of cars in the American market, since those may be very different from the Chinese market. The company wants to know:

- Which variables are significant in predicting the price of a car

- How well those variables describe the price of a car

Based on various market surveys, the consulting firm has gathered a large dataset of different types of cars across the Americal market.

## About the Car Price Prediction
Price is Target variable & 27 Features are PriceCategory, Company, Aspiratiion, Carbody, Drivewheel, Wheelbase, Carlength, Carwidth, Curbweight, Enginetype, Cylindernumber, Enginesize, Fuelsystem, Boreratio, Horsepower, CityMileage, HighwayMileage, HP-Category, Enginelocation, Stroke, Fueltype, Peakrpm, Doornumber, Compressionratio, Carmodel, Carheight, InsuranceRisk

## Business Goal
You are required to model the price of cars with the available independent variables. It will be used by the management to understand how exactly the prices vary with the independent variables. They can accordingly manipulate the design of the cars, the business strategy etc. to meet certain price levels. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## Project Overview
In this Project I have unleashed the useful Data Science insights using this CAR Price dataset and performed the feature selection precisely to build multiple linear regression model along with GradientBoostingRegressor by combining the power of best statistical rules & principles to maximise accuracy at its best. The best thing is my model is not having Multicollinearity & Heteroscedasticity problem.

## This Project is divided into 29 major steps which are as follows:
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
18. [Features P-Value & VIF Check](#p-vif)
19. [Final Implimentation of the MLR Model](#final-model)
20. [Model Evaluation](#mod-eval)
21. [Actual vs Predicted Price of Used CAR](#actual-predicted)
22. [Residual Distribution of Predicted Used CAR Price](#re-dit)
23. [Amount of Error in Used CAR Price Prediction](#amt-er)
24. [Durbin Watson Auto-Correlation Test](#dur-wat)
25. [Regression Evaluation Metrics](#mod-eval)
26. [Plotting the Regression Line](#reg-plot)
27. [Heteroscedasticity Tests](#het-test)
28. [Auto-Correlation plot](#auto-plot)
29. [Gradient Boosting For Regression](#grad-boost)
30. [GradientBoostingRegressor Deviance Check](#grad-boost)

## About Data
This dataset consists of 27 features and a target variable. It has 9 nominal variables, 13 numeric variables, 5 ordinal variables. The detailed description of all the features are as follows:

**1. wheelbase, carlength, carwidth, carheight, curbweight, enginesize, boreratio, stroke, compressionratio, horsepower, CityMileage, HighwayMileage, Peakrpm:** These are all numeric features.

**2. Carbody, Enginelocation, aspiration, company, drivewheel, enginetype, fueltype, fuelsystem, carmodel:** These are all nominal features.

**3. InsuranceRisk, Doornumber, Cylindernumber, PriceCategory, HP-Category:** These are all Ordinal features.

## Selected Features for the Final Model
**1. Carwidth:**

**2. Cylindernumber:** Cylindernumber (5 & 4)

**3. PriceCategory:** PriceCategory (Luxuary, Premium & Standard)

**4. HP-Category:** HP-Category (Heavy-HP & Standard-HP)

**5. Company:** Company (BMW & PORSCHE)

**6. aspiration:** aspiration (turbo)

**7. carbody:** carbody (convertible)
