### [Flight Price Prediction](https://github.com/SUPREME-CODER/Flight-Price-Prediction/blob/main/Flight%20Price%20Prediction.ipynb)


#### Problem Statement
The study aims to analyze the flight booking dataset sourced from the **Ease My Trip** website and perform various statistical hypothesis tests to extract meaningful insights.

The dataset will be trained using the 'Linear Regression' algorithm to predict a continuous target variable.

**Ease My Trip** is a popular online platform for booking flight tickets, frequently used by passengers to purchase their tickets.

A detailed analysis of this dataset will help uncover valuable insights that can significantly benefit potential passengers.


[Data Source](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction)
The dataset comprises 300,261 records with 11 features, detailing flight booking options from Easemytrip for travel between India’s top six metro cities.

#### Features
The cleaned dataset includes the following features:

1. **Airline:** Categorical, contains the names of 6 airlines.
2. **Flight:** Categorical, stores flight codes.
3. **Source City:** Categorical, indicates the departure city (6 unique cities).
4. **Departure Time:** Categorical, derived by grouping departure times into 6 time bins.
5. **Stops:** Categorical, represents the number of stops (3 distinct values).
6. **Arrival Time:** Categorical, derived by grouping arrival times into 6 time bins.
7. **Destination City:** Categorical, indicates the arrival city (6 unique cities).
8. **Class:** Categorical, specifies seat class (Business or Economy).
9. **Duration:** Continuous, shows travel time between cities in hours.
10. **Days Left:** Derived, calculated as the difference between the trip date and booking date.
11. **Price:** Continuous, the target variable representing ticket cost.


#### Dependencies
**Tech Stack** - Pandas, Scikit-learn, Matplotlib, RandomForestRegressor, BaggingRegressor and Supervised Learning.

#### Project Workflow

* **Overview** - Developed a predictive model to estimate flight prices based on factors such as class, itinerary, and route.<br>
* **Utility Functions** - Designed some utility functions for assisstance in data visualization analysis of the given features, feature engineering and data cleaning.
* **Data Anslysis and Transformation** -
    * Performed data transformation to combine the business and economic class flights dataset into one and data scaling.
    * Discovered insights for precise price prediction by analysing flight booking data from various airlines and performing A/B tests to profile business and economy class flights.
* **Data Visualization** - Presented the flight distribution for various arrival and destination plots, airline brands number of stops in the journey and the class of the flight.
* **Feature Engineering** - Conducted feature engineering by encoding the arrival and departure times for the ease of analysis.
* **Data Preprocessing** - Performed Target Encoding for the categorical variables. Calculated Mutual Information between dependent and resultant variables and found out the arrival and departure timings, class and airline brand play a huge role in the price prediction.
* **Model Building using GridSearchCV** - Implemented and optimized  RandomForestRegressor, BaggingRegressor models through hyperparameter tuning and implementing metrics like RMSE and Adjusted R^2 to enhance robustness and accuracy.
* **Best Model** - **RandomForestRegressor** performed better as it performed well on all metrics of **Adj R^2, RMSE and MAPE**.


#### Usage
Install the Jupyter Notebook and access the data mentioned in the link in Data Source and execute the cells one by one.


#### Results
The model was able to process the flight details and predict the price with an **$Adjusted$ $R^2$ metric being 98.5 %**.


#### Final Notes
This is a great project to learn:-
* Feature Engineering.
* Data Analysis.
* Data Transformation and Encoding.
* A/B Tests for customer segmentation.
* Grid Search CV for hyper parameter tuning.