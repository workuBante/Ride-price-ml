Ride Price Machine Learning Project


This project focuses on building a machine learning model to predict ride prices based on trip-related features such as distance, duration, traffic conditions, and weather. The objective is to develop a regression model that can estimate the expected price of a ride before it is completed.

The project demonstrates the complete machine learning workflow including data preprocessing, exploratory data analysis, feature engineering, model training, evaluation, and interpretation of results.

The final model aims to provide accurate and reliable price predictions that could be used in ride-hailing or transportation systems.

Repository Structure

ride-price-ml||
  README.md/
  ride_price1.csv/
  ride_price.ipynb


data/ contains the dataset used for training and evaluation.

notebook/ contains the Jupyter Notebook with all preprocessing, training, and evaluation steps.

README.md explains the project and how to use it.

Dataset Description

The dataset (ride_price1.csv) contains ride-level information used to predict the ride price.

Each row represents a single ride and includes the following attributes:

trip_id: Unique identifier for each ride

city: City where the ride took place

distance_km: Distance of the ride in kilometers

trip_duration_min: Duration of the ride in minutes

time_of_day: Time category (morning, afternoon, evening, night)

traffic_level: Traffic condition during the ride (low, medium, high)

weather_condition: Weather during the ride (clear, rainy, etc.)

demand_level: Demand intensity at the time of the ride

ride_price: Target variable — the total price of the ride

The goal of the project is to predict the ride_price using the other features.

Features Used and Justification

The following features were used to train the model:

Distance (distance_km)
Distance directly affects fuel consumption and trip cost. Longer distances typically result in higher prices.

Trip Duration (trip_duration_min)
Duration reflects time spent on the trip, which impacts driver cost and pricing.

Time of Day
Prices may vary depending on peak and off-peak hours.

Traffic Level
Heavy traffic increases trip duration and operational costs.

Weather Condition
Adverse weather conditions can increase demand and affect pricing.

Demand Level
Higher demand may lead to surge pricing and increased ride costs.

The target variable ride_price was excluded from the input features during training to avoid data leakage.

These features were selected because they logically influence ride pricing and provide meaningful predictive information for the model.

How to Run the Notebook

Clone the repository to your local machine.

Ensure Python and Jupyter Notebook are installed.

Navigate to the notebook/ directory.

Open ride_price.ipynb using Jupyter Notebook.

Run all cells sequentially from top to bottom.

The notebook includes:

Data loading

Data preprocessing

Feature encoding and scaling

Model training

Model evaluation

Key Findings

Distance and trip duration were strong predictors of ride price.

Traffic level and demand level also significantly influenced pricing.

Proper preprocessing (handling categorical variables and scaling) improved model performance.

Avoiding data leakage (excluding ride_price from input features) was critical for obtaining reliable evaluation results.

The trained model can generalize to unseen data when preprocessing steps are applied consistently.


Overall, the project demonstrates how structured data preprocessing and careful model training can produce accurate ride price predictions.



