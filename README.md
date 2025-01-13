
# Airbnb Analytics: Predicting Rental Prices

## Project Overview
This project leverages data analytics and machine learning techniques to predict the rental prices of Airbnb listings based on various factors like location, room type, number of bedrooms, and more. By utilizing models such as Linear Regression and Random Forest, we aim to provide insights for Airbnb hosts to set competitive and optimal prices.

## Table of Contents
- [Introduction](#introduction)
- [Data](#data)
- [Methodology](#methodology)
- [Results](#results)
- [Conclusion and Recommendations](#conclusion-and-recommendations)
- [Getting Started](#getting-started)
- [Technologies Used](#technologies-used)
- [References](#references)

## Introduction
Airbnb has transformed the travel and accommodation industry by offering unique, flexible, and personalized stays. This project addresses the question: *How can Airbnb hosts leverage data to accurately predict rental prices and optimize revenue?*

By understanding the factors that influence rental pricing, hosts can set competitive prices, optimize revenue, and improve decision-making in a competitive marketplace.

## Data
The dataset contains 279,712 observations and 31 variables, including:
- Room type
- Number of bedrooms
- Minimum and maximum nights
- Location
- Accommodation capacity

### Data Processing
1. Handling missing values using imputation techniques.
2. Removing outliers using the interquartile method.
3. Log transformation of price data to address skewness.

## Methodology
The following models were implemented:
1. **Baseline Model**: Provides initial metrics for comparison.
2. **Linear Regression**: Evaluates relationships between predictors and rental prices.
3. **Stepwise Regression**: Identifies significant predictors to improve model performance.
4. **Random Forest**: Ensures robust and flexible predictions.

## Results
- **Baseline Model**: RMSE = 1.222, MAPE = 19.88%
- **Linear Regression**: RMSE = 1.616, MAPE = 18.12%
- **Stepwise Regression**: RMSE = 0.622, MAPE = 8.78%
- **Random Forest**: RMSE = 0.607, MAPE = 8.69%

The Random Forest model outperformed all others, offering the most accurate and robust predictions.

## Conclusion and Recommendations
### Key Findings:
- Room type has the highest influence on pricing (36.10%).
- Accommodation capacity significantly impacts pricing (18.10%).
- Additional bedrooms can increase revenue potential.

### Recommendations for Hosts:
1. Highlight room features that align with hotel standards.
2. Maximize accommodation capacity with adequate amenities.
3. Optimize bedroom count to improve pricing.
4. Reassess minimum night requirements to attract more bookings.

## Getting Started
### Prerequisites:
- Python 3.x
- Libraries: pandas, numpy, sklearn, matplotlib

### Installation:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/airbnb-prediction.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Run the Project:
1. Preprocess the data and build models by running:
   ```bash
   python analysis.py
   ```
2. Visualize results:
   ```bash
   python visualize.py
   ```

## Technologies Used
- Python
- Jupyter Notebook
- Random Forest Algorithm
- Linear Regression

## References
1. [Samwel Meigeka (2022)](https://doi.org/10.22158/ibes.v4n1p26)
2. [Veronica Leoni & William Nilsson (2021)](https://doi.org/10.1016/j.ijhm.2021.102914)
3. [OpenDataSoft (2023)](https://data.opendatasoft.com/explore/dataset/airbnb-listings%40public/table)
