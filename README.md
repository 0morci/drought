# Drought Detection using Time Series Models
## Overview
This project focuses on predicting droughts, an increasingly severe issue exacerbated by climate change. By using meteorological data from Spain's AEMET API, we have developed models to predict the Standardized Precipitation Index (SPI), a key drought indicator, at different time intervals (3, 6, and 12 months).

## Problem
Droughts are a natural, cyclical phenomenon affecting various regions with increased frequency and intensity due to climate change. Predicting droughts can help mitigate their impact on hydrological resources, agriculture, and economies. Our project aims to forecast droughts using time series models based on historical meteorological data, allowing for proactive resource management.

## Data
Meteorological data was gathered from the AEMET API, which provides variables such as temperature, precipitation, wind speed, and pressure. This data is used to calculate the SPI, an index that measures drought severity ranging from -3 (severe drought) to 3 (excessive moisture).

## Models Used
#### MLP (Multilayer Perceptron):
A neural network that models the relationship between the input (historical meteorological data) and the output (SPI predictions).
#### LSTM (Long Short-Term Memory):
A recurrent neural network capable of capturing long-term dependencies in time series data.
#### Recursive Autoregressive Forecasting: 
Utilizes the Skforecast library, with a RandomForestRegressor for time series predictions.

## Model Comparison
The MLP model showed the best performance, with the lowest Mean Squared Error (MSE) compared to LSTM and Skforecast models, making it the optimal choice for future predictions.

## Results
The SPI predictions for future drought events have been mapped using Power BI, visualizing the severity of drought across different regions in Spain. These maps highlight areas with higher or lower SPI values, offering insights into potential drought development in upcoming months.

## Visualization
![image](https://github.com/user-attachments/assets/2f836b40-dc3b-4fdd-a866-7c992227fe40)

## Future Work
Spatial Interpolation: Expanding drought predictions to areas without meteorological stations using spatial interpolation techniques.
Real-time Data: Incorporating live data from the AEMET API to continuously update the model with real-time predictions.
Model Improvements: Testing more complex neural network architectures or alternative algorithms, such as decision trees, to better understand the influence of various meteorological factors on drought severity.
