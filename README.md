Crop Yield Prediction in India
Business Problem
India's agriculture sector experiences significant variability in crop yields due to factors such as climate change, soil quality, and resource availability. This project aims to build a Machine Learning model to predict crop production across different states and districts in India using features like state, district, crop type, and more. The predictions will help farmers and policymakers optimize crop selection, resource distribution, and risk management to enhance productivity and sustainability.

Objectives
Crop Selection Optimization: Predict crop yields to help farmers select the best crop for their region and season.
Resource Distribution: Advise policymakers on optimal resource allocation (e.g., water, fertilizers).
Risk Management: Forecast yield deficits to proactively manage risks.
Impact: Empower decision-makers with reliable predictions to improve productivity and resource utilization.
Key Features
State: The state where the crop is cultivated.
District: The district within the state where the crop is cultivated.
Crop: Type of crop being grown (e.g., rice, wheat).
Season: The cultivation season (e.g., Kharif, Rabi).
Crop Year: Year of cultivation.
Area: Land area used for cultivation (in hectares).
Production: Total production of the crop (in tonnes), which is the target variable.
Data Understanding
The dataset is sourced from crop_production.csv and contains 246,091 rows and 7 columns with information on crop production across different states and districts.

Data Preprocessing
Missing Values: 3,730 missing values in the Production column were filled with the median to avoid outliers.
Feature Engineering: A new feature, Yield_Production, was created based on the Production column. It labels the production as HIGH or LOW based on the 45th percentile threshold.
Data Summary
Rows: 246,091
Columns: 7 (State, District, Crop Year, Season, Crop, Area, Production)
Exploratory Data Analysis (EDA)
Performed visualizations to analyze the distribution of key features and their relationship with crop production. The target variable Yield_Production has a fairly balanced distribution:

HIGH: 135,350
LOW: 110,741
Modeling
Machine learning models such as Linear Regression and Logistic Regression were explored to predict the production levels of crops. The data was split into training and testing sets to build and evaluate the models.
