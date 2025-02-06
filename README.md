# Shaping the Future: Forecasting Used Car Prices

**Jupyter Notebook with code, experimentation, further insights, and deployment strategies: [here](https://github.com/JunGaoca/usedCarPricePrediction/blob/main/used-car-price-prediction.ipynb).**

## Business Goal
Accurate price assessment is essential in the used-car trading business. This analysis aims to identify key factors affecting used car prices and develop predictive models for price forecasting. These insights will help dealers optimize inventory and pricing strategies to maximize profitability. 

## Data
The original Kaggle dataset of 3 million used cars was reduced to 426,880 entries to enhance processing speed and efficiency. The dataset is [here](https://github.com/JunGaoca/usedCarPricePrediction/blob/main/data/vehicles.csv).

This dataset with 18 features includes:
-   Numeric Features – price, odometer, year
-   Categorical Features – region, manufacturer, model, condition, cylinders, fuel, title_status, transmission, VIN, drive, size, type, paint_color, state

## Modeling and Performance
In this project, we applied various regression techniques to predict used car prices. The models explored include `Linear Regression`, `Ridge Regression`, and `Elastic Net Regression`. Each model was trained and tested using a train/test split, followed by cross-validation and hyperparameter tuning with GridSearchCV to improve performance.

Among these, the Ridge Regression model has been better compared to all other models we tested. The MSE (52296153.93) was about 60% less than the baseline error values.

## Conclusions
The model revealed a significant correlation between specific features and used car prices. Notably, year, type, and title status positively impact resale value, while higher odometer readings are linked to lower prices. These insights can help dealers optimize inventory and pricing strategies more effectively.

### Interesting Findings
| **Feature**     | **Recommendation**    | **Impact**                    | **Interpretation**    
|-----------------|-----------------------|-------------------------------|-----------------------
| Odometer        | Highlight and promote low-mileage cars in the inventory.   | Strong negative    | Lower mileage increases its price
| Year            | Expand the inventory with newer model cars    | Significant positive    | Newer car models tend to have higher prices
| Type            | Expand the inventory by adding more trucks    | Strong positive    | Trucks tend to have higher resale value
| Title status    | Stock more cars with a clean title            | Strong positive    | Vehicles with a clean title are valued more highly

### Actionable Insights

##  Next steps and recommendations
