# Prediction of GHG and energy consumption from Seattle commercial buildings

Dataset: https://data.seattle.gov/dataset/2016-Building-Energy-Benchmarking/2bpz-gwpy

Context/Scenario: You work for the City of Seattle. To achieve its goal of a carbon-neutral city by 2050, your team is looking closely at emissions from non-housing buildings. Careful but chronophage and expensive surveys were carried out by your officers in 2015 and 2016

Problem: Predict energy use and GHGs emissions from commercial building and assess the importance of the ENERGY STAR Score for predicting emissions.

Methods:
1. Clean the dataset (outlier identification, NA ratio)
2. EDA
3. Extract pertinent features
4. Feature engineering
5. Do univariate and multivariate analysis
6. Split datas in train and test sets
7. Pipeline (Standardisation, Lasso pre-treatment)
8. Grid Search CV
9. Benchmark models with RMSE, R², execution time
10. Feature importance

Results:
1. Best model to predict GHGs : Ridge kernel in 0.1 sec and R²=0.93
2. Best model to predict energy use : XGBoost in 2.54 sec and R²=0.80
3. Energy STAR score is not an important feature in regard of the feature importance
4. It will save the time of the Seattle city agents

Libraries: Pandas, Numpy, Matplotlib, Scikit-learn
