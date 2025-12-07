Medical Insurance Charges Prediction Using Machine Learning
 Overview

This project applies supervised machine learning to predict medical insurance charges based on personal attributes such as age, BMI, smoking status, and number of children. The notebook walks step-by-step through loading the dataset, exploratory data analysis, feature encoding, and building multiple predictive models.

Objectives

Analyze factors influencing medical insurance cost

Preprocess and encode categorical features

Train regression models to predict charges

Evaluate model performance using standard metrics

Interpret findings and identify key cost drivers

Dataset Description
Feature	Description
age	Age of the insured individual
sex	Male/Female
bmi	Body mass index
children	Number of dependents covered
smoker	Smoker or non-smoker
region	Geographical area
charges (target)	Medical insurance cost

Missing Values: None detected
Target Behavior: Right-skewed distribution — high outliers linked to smokers & high BMI



🧪 Techniques & Models Used

Data inspection & summary statistics

Exploratory visual analysis (distributions, correlations)

Categorical encoding & scaling

Train/Test split

Baseline model: Linear Regression

Model evaluation with MAE, MSE, RMSE, R²

📈 Results Summary 
Metric	Score
MAE	=from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
import numpy as np
MAE= 4181.194
RMSE	= 5796.285
R²	= 0.784
Smoking, BMI, and age appear to be the strongest predictors of insurance cost.

LINK TO NOTEBOOK :https://colab.research.google.com/drive/13Uh1A5Msb1kf66_FVU4b5r4H2JpDIng5?usp=sharing


▶ How to Run
Option 1 — Google Colab
from google.colab import files
uploaded = files.upload()


