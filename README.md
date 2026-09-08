# car-price-prediction
Car Price Prediction is a machine-learning-based project developed using Python. The system predicts the price of a new or used car based on important features such as brand, manufacturing year, kilometers driven, fuel type, engine size, number of previous owners, and transmission type.
# Car Price Prediction

## 1. Introduction

Car Price Prediction is a Machine Learning project that predicts the price of a car based on its features. The project is designed for educational purposes and demonstrates how regression techniques can be applied to real-world prediction problems.

## 2. Objective

The main objectives of this project are:

* To analyze car-related data.
* To identify factors that influence car prices.
* To clean and preprocess the dataset.
* To train a Machine Learning regression model.
* To predict car prices.
* To compare actual and predicted prices.
* To visualize the relationship between car features and price.

## 3. Technologies Used

* **Python**
* **Pandas** – Data processing and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Scikit-learn** – Machine Learning

## 4. Dataset

The dataset contains information about different cars.

### Features

* `car_id` – Unique identification number
* `brand` – Car brand
* `year` – Manufacturing year
* `kilometers_driven` – Distance travelled by the car
* `fuel_type` – Type of fuel used
* `engine_size_l` – Engine size in litres
* `number_of_owners` – Number of previous owners
* `transmission` – Manual or Automatic
* `price` – Price of the car

### Target Variable

**Price** is the target variable that the model predicts.

## 5. Data Preprocessing

Before training the model, the dataset is preprocessed.

The following steps are performed:

1. Load the dataset using Pandas.
2. Check the dataset for missing values.
3. Fill missing numerical values using the median.
4. Fill missing categorical values using the most frequent value.
5. Standardize numerical features using `StandardScaler`.
6. Convert categorical features into numerical form using `OneHotEncoder`.
7. Split the dataset into training and testing data.

## 6. Machine Learning Algorithm

### Linear Regression

The project uses **Linear Regression** to predict car prices.

Linear Regression finds the relationship between the input features and the car price. The trained model uses these relationships to estimate the price of an unseen car.

The dataset is divided into:

* **80% Training Data**
* **20% Testing Data**

## 7. Model Evaluation

The model is evaluated using the following metrics:

### Mean Absolute Error (MAE)

Measures the average difference between actual and predicted prices.

### Root Mean Squared Error (RMSE)

Measures prediction error while giving more importance to larger errors.

### R² Score

Shows how well the model explains the variation in car prices. A value closer to 1 indicates better performance.

## 8. Prediction

The trained model can predict the price of a new car using details such as:

* Brand
* Year
* Kilometers driven
* Fuel type
* Engine size
* Number of owners
* Transmission

For example, the program predicts the price of a Toyota manufactured in 2022 with 35,000 kilometres driven, a 1.8-litre engine, one owner, petrol fuel, and automatic transmission.

## 9. Visualizations

The project generates two graphs:

### Kilometers Driven vs Car Price

Shows the relationship between the distance travelled and the price of cars.

### Actual vs Predicted Prices

Compares the actual prices with the prices predicted by the Machine Learning model.

## 10. Project Workflow

**Dataset → Data Cleaning → Data Preprocessing → Train/Test Split → Linear Regression → Model Training → Prediction → Evaluation → Visualization**

## 11. How to Run the Project

Install Python and open the project folder in a terminal.

Install the required libraries:

```bash
pip install -r requirements.txt
```

Run the program:

```bash
python car_price_prediction.py
```

## 12. Output

The program displays:

* First five rows of the dataset
* Dataset size
* Missing-value information
* MAE
* RMSE
* R² Score
* Actual vs predicted prices
* Predicted price for a new car
* Important factors affecting car price

It also generates:

* `kilometers_vs_price.png`
* `actual_vs_predicted.png`

## 13. Conclusion

The Car Price Prediction project demonstrates how Machine Learning can be used to estimate vehicle prices from historical car information. By applying data preprocessing and Linear Regression, the system can learn relationships between car characteristics and their prices and provide predictions for new vehicles.

The project provides practical experience in **data preprocessing, regression, model evaluation, prediction, and data visualization** using Python.

## 14. Note

The included dataset is **synthetic** and is intended for educational and classroom Machine Learning practice. It does not represent real vehicle sales records.
