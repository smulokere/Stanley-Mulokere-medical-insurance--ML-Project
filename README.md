Medical Insurance Charges Prediction Using Machine Learning

 PROJECT SUMMARY

This project applies supervised machine learning to predict medical insurance charges based on personal attributes such as age, BMI, smoking status, and number of children. The notebook walks step-by-step through loading the dataset, exploratory data analysis, feature encoding, and building multiple predictive models.This study first identified potential confounding factors through description and correlation analysis, and then used a stepwise regression model to control variables such as age, BMI, sex, children, and region from simple to complex to verify whether smoking is the independent and strongest influencing factor of medical expenditures. Model diagnosis ensures the reliability of OLS, and then the conclusion shows that smoking always remains the most stable and significant influence, with strong explanatory power and policy significance.



PROJECT Objectives

-Analyze factors influencing medical insurance cost

-Preprocess and encode categorical features

-Train regression models to predict charges

-Evaluate model performance using standard metrics

-Interpret findings and identify key cost drivers


Dataset Description and Feature	Description

-Age of the insured individual

-sex	Male/Female

-bmi	Body mass index

-children	Number of dependents covered

-smoker	Smoker or non-smoker

-region	Geographical area

-charges (target)	Medical insurance cost

SOURCE

-Kaggle:https://www.kaggle.com/datasets/mirichoi0218/insurance

Missing Values: None detected
Target Behavior: Right-skewed distribution — high outliers linked to smokers & high BMI



🧪TOOLS AND LIBRARIES USED 

-Data inspection & summary statistics

-Exploratory visual analysis (distributions, correlations)

-Categorical encoding & scaling

-Train/Test split

-Baseline model: Linear Regression

-Model evaluation with MAE, MSE, RMSE, R²

-Random forest

BUSINESS INSIGHTS
Recommendation

-Insurance Companies Should Clearly Distinguish Pricing Strategies for Smokers and Non-Smokers
Insurance companies can setting up a smoker risk premium and offer health plan discounts.

-Focus on High-BMI Groups and Establish an Obesity-Related Risk Management Mechanism
Regression shows that BMI is a robust and significant risk factor, suggesting insurance companies to improve health management programs for clients with higher BMI, provide nutrition consultation and set up health improvement incentives.

-The Elderly Group Should Be Given Extra Attention and Expected Cost Management
Because the aging suffor from higher risks of chronic dieases, welfare should include chronic disease management projects for middle-aged and elderly customers and increase coverage of physical examinations and early screening.

-Further Research is Recommended, Such As Smoker×BMI and Smoker × Age

Limitation
-The Data Are Cross-Sectional and Temporal Causality Cannot Be Identified
This study is only based on a time section and cannot observe changes in medical expenses over time. Therefore, researchers need to determine cumulative effects of long-term smoking.

-The Data Comes from Kaggle and Has Limited Representativeness
The data are still not necessarily cover all socioeconomic backgrounds and not necessarily representative of the overall U.S. population structure. Therefore, the external validity of the conclusions needs to be interpreted with caution.

-Key Socioeconomic Variables Are Not Included
Medical costs may be affected by SES (socioeconomic status) such as: income, education and occupation. The absence of these variables may limit the explanatory power of some models.



📈 Results Summary 


Metric	Score
MAE	=from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
import numpy as np
-MAE= 4181.194
-RMSE	= 5796.285
-R²	= 0.784
-Smoking, BMI, and age appear to be the strongest predictors of insurance cost.

LINK TO NOTEBOOK :https://colab.research.google.com/drive/12vfxRZJvxQJfqf48cCGl0SRVoWdv4UB8?usp=sharing


▶ How to Run
Option 1 — Google Colab
from google.colab import files
uploaded = files.upload()

REFERENCE


Finkelstein, E. A., Trogdon, J. G., Cohen, J. W., & Dietz, W. (2009). Annual medical spending attributable to obesity. Health Affairs.

Health system tracker.(2023). How have costs associated with obesity changed over time? Retieved from: https://www.healthsystemtracker.org/chart-collection/how-have-costs-associated-with-obesity-changed-over-time/


Kaggle. (2018). Medical Cost Personal Dataset. Retrieved from: https://www.kaggle.com/datasets/mirichoi0218/insurance


U.S. Department of Health and Human Services. (2014). The health consequences of smoking—Surgeon General’s report. 
https://www.hhs.gov/surgeongeneral/reports-and-publications/tobacco/consequences-smoking-factsheet/index.html









