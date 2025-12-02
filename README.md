# Glucose Prediction Model
A personalized AI system leveraging Dexcom Clarity time series data for glucose forecasting and meal impact prediction.

## Overview

This project aims to develop a personalized glucose prediction and meal recommendation system using of continuous glucose monitoring (CGM) data from Dexcom Clarity reports. The dataset contains glucose readings every 5 minutes along with detailed food logs and contextual information (e.g., time, meal content, and nutrition). 

By combining time series analysis and machine learning, this system seeks to understand how daily behaviors affect blood glucose trends and to provide recommendations for improving glycemic stability.

## Data Sources
 1. **Dexcom CGM Data:**
Continous Glucose Monitoring data, including timestamps, glucose values, estimated insulin, and estimated carb values.
2. **Apple Helath Data:**
Exported health metrics from Apple Health, such as heart rate, exercise time, and step count.

## Methodology
1. **Data Harmonization:**
Integration of Dexcom and Apple Health Data Based on timestamps.
2. **Feature Engineering:**
Extraction of historical glucose and current carbohydrate intake as features for the model.
3. **Model Architecture:**
A Long Short-Term Memory (LSTM) neural network is used to predict future glucose levels.
4. **Training and Evaluation:**
The model is trained on a split dataset and evaluated based on its ability to predict 2-hour post-meal glucose values.

## Setup and Installation
To run this notebook, you will need to:
1. **Mount Google Drive:**
The notebook uses files stored in Google Drive. Ensure you have mounted your Google Drive to `/content/drive`.
2. **Dataset Paths:**
Update the paths to your CSV files in the relevant cells if they differ from the provided paths.
 *
 `Clarity_Export_Parmar_Henna_2025-11_03_231446.csv`
*
`HealthAutoExport-2025-10-20-20-25-11-03.csv`
*
`Clarity_Export_Parmar_Henna_2025-11-22_205142.csv` (for validation)
4. **Dependencies:**





