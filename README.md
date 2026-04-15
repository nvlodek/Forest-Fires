# Forest Fire Burned Area Prediction

## Overview
This project predicts the burned area of forest fires in Montesinho Natural Park (Portugal) using machine learning models. It explores how environmental and weather-related features can be used to model wildfire severity.

## Problem
Wildfires are increasing in frequency due to climate change, causing significant environmental and economic damage. Accurately predicting burned area can help improve preparedness and response strategies.

## Dataset
- Source: UCI Machine Learning Repository (Forest Fires dataset)  
- Includes weather and environmental features such as temperature, humidity, wind, and components of the Fire Weather Index (FWI) system  

## Data Preprocessing
- Performed one-hot encoding for categorical features (month, day)  
- Applied Min-Max scaling to normalize numerical features  
- Verified dataset contained no missing values  
- Split data into 80% training and 20% testing  

## Models Implemented
- Random Forest Regression  
- Gradient Boosting Regression  
- AdaBoost Regression  

## Evaluation Metrics
- Mean Absolute Error (MAE)  
- Mean Squared Error (MSE)  
- Root Mean Squared Error (RMSE)  
- R-squared (R²)  

## Results
- All models achieved low error (MAE and RMSE), indicating accurate predictions on average  
- AdaBoost performed best overall, achieving the highest R² and lowest error metrics  
- All models struggled with low R² values, suggesting difficulty capturing variance in the target variable  

## Key Insights
- Ensemble methods (Random Forest, Gradient Boosting, AdaBoost) are effective for regression tasks  
- Low R² values indicate the dataset is complex and may require additional feature engineering  
- Boosting methods improved performance by learning from previous model errors  

## Tools & Technologies
- Python  
- scikit-learn  
- NumPy  
- matplotlib  

## Key Takeaways
- Model evaluation requires multiple metrics, not just accuracy  
- Feature engineering is critical for improving regression performance  
- Real-world datasets often contain noise and complex relationships that limit model performance  

## How to Run
1. Clone the repository  
2. Install required libraries (`scikit-learn`, `numpy`, etc.)  
3. Run the main script or notebook  
