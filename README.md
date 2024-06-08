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
<img src="https://github.com/dongdo1999/SolarPowerGenerationForecasting/assets/47492780/6e91cc45-6165-40b8-bd35-630eee3640b9",style="width: 50%; height: auto;")
![image](https://github.com/dongdo1999/SolarPowerGenerationForecasting/assets/47492780/f88793b8-7006-42ad-91fe-552d97f45819,style="width: 50%; height: auto;")

## 🚨 특수한 발전량 패턴 존재
![image](https://github.com/donghwan0318/Solar-Power-Generation-Forecasting-Using-Weather-and-Generation-Data/assets/136334371/52dfcb34-d0aa-4dc4-9ec5-5242f0898e4f)

일반적으로 정오에 발전량이 최대치를 보이는 커브 형태를 띠지만, 특정한 날에는 그렇지 않을 때가 있음 

💡 해결을 위한 노력들
- 단순 그러한 특수한 패턴을 띄는 날들을 클러스터링,변수선택법 등을 통해 분리하고자 하였음(시계열 클러스터링, 오차율기반 클러스터링, 계절별, 시간별, 변수선택법), 이후 클러스터별 개별 모델링 진행
- 특수한 패턴을 띄는 날들이 과거에 하루는 존재할 것이다 판단하고, 백터 유사도를 이용하여 파생변수를 생성

## 클러스터링
![image](https://github.com/donghwan0318/Solar-Power-Generation-Forecasting-Using-Weather-and-Generation-Data/assets/136334371/7b6276b6-9ab5-4870-8887-1f52989ce87e)
![image](https://github.com/donghwan0318/Solar-Power-Generation-Forecasting-Using-Weather-and-Generation-Data/assets/136334371/22b6b698-1d23-44a5-81aa-cf1717972486)



## 📃 모델링
![image](https://github.com/donghwan0318/Solar-Power-Generation-Forecasting-Using-Weather-and-Generation-Data/assets/136334371/876ba0d6-23e0-405e-a68b-a52a7b07cd3a)
![image](https://github.com/donghwan0318/Solar-Power-Generation-Forecasting-Using-Weather-and-Generation-Data/assets/136334371/9a53886e-e74a-4617-8d93-78962fd65639)
![image](https://github.com/donghwan0318/Solar-Power-Generation-Forecasting-Using-Weather-and-Generation-Data/assets/136334371/3480801a-ef37-4977-8661-0fa8c4b0eb5c)






