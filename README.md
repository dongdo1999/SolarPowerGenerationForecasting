# 2023-2-PSAT-team-deeplearning
[notion page](https://www.notion.so/d8e330e9fa9f4461b48caeb27d2f5f8f?v=498c78de406e491296467a215f8275a2)

Topic Analysis by the P-SAT Deeplearning Data Analysis Team in the Statistical Analysis Society for the 2st Semester of 2023

## 💻 Project introduction

<Forecasting Solar Power Generation Using Predicted Weather & Generation Data>☀️

Competition Overview:
Hosted by POSTECH and H energy, this competition is part of the 5th OIBC CHALLENGE for university and graduate students.

Utilized Data:
- Predicted power generation
- Actual power generation of the target solar plant
- 13 weather features including cloud cover, temperature, and humidity
- Incentives (model evaluation scores) of predicted generation

Data Source:
Provided by the organizers.

Project Duration:
2023.10.22 ~ 2023.11.17


## 🔥 Team members and Roles
- Jung-Hwan Lee (Team Leader): Solar cell domain research, feature engineering (time/season transformation), LGBM, LSTM, MLP+LGBM ensemble, RNN+LGBM ensemble, SCINet.
- Dong-Hwan Kim: Solar cell domain research, feature engineering (vector similarity), LGBM, LSTM, time series clustering, regression+LGBM ensemble, structural time series model.
- Ga-Min Kwon: Ensemble methods, XGBoost, correlation analysis, X-variable clustering (error rate/season), pattern analysis (error rate/generation by time/season). 
- Chae-Won Park: Ensemble methods, LGBM, correlation analysis, seasonal linear regression, X-variable clustering (error rate/season), feature selection (season).
- Jun-Young Park: Ensemble methods, correlation analysis, linear regression by time/season, similarity prediction, X-variable clustering (error rate/season).
- 

## 🔍 Analysis Workflow

1. **Domain Research**
   - Investigating solar cell characteristics and relevant domain knowledge.

2. **Exploratory Data Analysis (EDA)**
   - Predicted power generation for different models.
   - Variance and mean of predictions by time of day.
   - Error rates by season.
   - Correlation analysis.
   - Etc.

3. **Feature Engineering,Selection and Modeling**
   - Applying various techniques to enhance performance.

4. **Visualization and Analysis of Prediction Results / Score Calculation**
   - Visualizing and analyzing prediction outcomes.
   - Calculating evaluation scores.

## 📈 Compeition introduction
<img src="https://github.com/dongdo1999/SolarPowerGenerationForecasting/assets/47492780/fa58d2a9-51e7-43fc-b663-29920b5df04e" width="50%" height="auto"/><img src="https://github.com/dongdo1999/SolarPowerGenerationForecasting/assets/47492780/7d99b035-b0b8-4f64-ab98-8fcfd6b8329b" width="50%
" height="auto"/>

## 🚨 Unusal patterns are observed
![image](https://github.com/dongdo1999/SolarPowerGenerationForecasting/assets/47492780/feb439f0-df64-47f0-bdc8-01ed0d95b6b0)


Power generation usually follows a curve with a peak at midday; however, on certain days, this pattern is not observed


💡 Efforts to Resolve
- To isolate days exhibiting such unique patterns, various techniques were employed, including time-series clustering, error rate-based clustering, seasonal and hourly clustering, and variable selection methods. Subsequent modeling was performed for each cluster.
- It was assumed that days with unique patterns must have occurred in the past. Derived variables were created using vector similarity.

## Clustering
![image](https://github.com/dongdo1999/SolarPowerGenerationForecasting/assets/47492780/a5a0fa69-59b8-43bf-bf33-4bcb439b0543)
![image](https://github.com/dongdo1999/SolarPowerGenerationForecasting/assets/47492780/8df6984c-dafa-4c67-9eb8-3d3f3253ac79)



## 📃 Modeling

<img src= "https://github.com/dongdo1999/SolarPowerGenerationForecasting/assets/47492780/524e87ba-4b87-4c3a-9005-76a79d171ba4" width="33%" height="auto"/>
<img src = "https://github.com/dongdo1999/SolarPowerGenerationForecasting/assets/47492780/46549804-2342-4b41-8639-28094922e6c1" width="33%" height="auto"/>
<img src="https://github.com/dongdo1999/SolarPowerGenerationForecasting/assets/47492780/93db9b4d-4c2b-4dd6-acae-40e95d13cd18" width="33%" height="auto"/>

