# Energy Consumption Forecasting Project
 Energy Consumption Forecasting using LSTM Recurrent Neural Network Model

## 1. Problem Definition:
- The goal of the Energy Consumption Forecasting Project is to develop an accurate and reliable model that can predict future energy consumption for a given region or facility. This project addresses the need for efficient energy management and resource planning by providing insights into future energy demand patterns.

## 2. Data Collection:
- Data has been downloaded from UCI Machine Learning Repository in the form of csv file.

## 3. Feature Description:
- DateTime - Each ten minutes
- Temperature - Weather Temperature of Tetouan city
- Humidity - Weather Humidity of Tetouan city
- Wind Speed - Wind speed of Tetouan city
- general diffuse flows - general diffuse flows
- diffuse flows - diffuse flows
- Zone 1 Power Consumption - power consumption of zone 1 of Tetouan city
- Zone 2 Power Consumption - power consumption of zone 2 of Tetouan city
- Zone 3 Power Consumption - power consumption of zone 3 of Tetouan city

## 4. Data Exploration and Analysis:
Insights:
- The distribution of the temperature data follows a Bimodal distribution.
- The temperature of the city often lies between 15 to 25 degree celsius.
- Distribution of Humidity data is skewed towards left. Most of the data points lies in the right side end of the distribution.
- The Humidity level of the city is mostly between 80 to 95.
- The wind speed of the city either between 0-1 mph or 4.5-5.5 mph mostly.
- The distributionof Zone 1 power consumption follows a bimodal distrbution.
- The power consumption of zone 1 often be at 25000MW or 35000MW.
- The distributionof Zone 2 power consumption follows a near normal distrbution.
- The power consumption of zone 2 often between 20000MW to 30000MW.
- The distribution of Zone 3 power consumption is skewed towards right and there are some outlier point in the left end of the distribution.
- The power consumption of zone 3 is around 15000MW mostly.
- The power consumption of all three zones are peaking between Jul to Sep months. The temperature of the city is also peaking at this time in the city. July to Sep is the summer season in Tetouan city. People would use Air Conditioners during this time which might have causes a raise in consumption of Electricity.
- The average power consumption is in the peak during thursday and reaches its lowest point between sunday and monday.
- The average power consumption is maximum between 8 to 9 pm at night. The lowest consumption occurred in the morning time.

## Summary:
- loaded the data as a pandas dataframe.
- Analyzed the outline of the data, datatypes and summary of the data.
- Performed exploratory data analysis to understand the distribution of the data and relationship of each feature with target variable.
- Checked the number of missing values and duplicates in the data.
- Built two models (Prophet and LSTM Recurrent Neural Network) to forecast power consumption data.
- Evaluated the performance of the models with different metrics (MAPE and Accuracy).
- Based on the evaluation, concluding that the LSTM recurrent neural network model performed well in forecasting the power consumption data with mean absolute percentage error of 4% and accuracy score of 90%.