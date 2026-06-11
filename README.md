# Used Car Price Prediction
Machine Learning project for predicting used car selling prices using Linear Regression and Lasso Regression with data preprocessing, categorical encoding, model evaluation, and price prediction analysis.
# 🚗 Used Car Price Prediction Using Machine Learning

A Machine Learning project that predicts the selling price of used cars using Regression algorithms. The project applies data preprocessing, categorical feature encoding, Linear Regression, and Lasso Regression to estimate vehicle prices based on various car attributes.

---

## 📌 Project Overview

Used car pricing is influenced by multiple factors such as vehicle age, fuel type, transmission, ownership history, and mileage.

This project builds predictive models to estimate car selling prices and compares the performance of:

- Linear Regression
- Lasso Regression

The project also evaluates model performance using R² Score and visualizes actual vs predicted prices.

---

## 🎯 Objectives

- Analyze used car market data.
- Perform categorical feature encoding.
- Build regression models for price prediction.
- Compare Linear Regression and Lasso Regression performance.
- Visualize actual and predicted prices.
- Predict selling prices of used vehicles.

---

## 📂 Dataset

Dataset File:

```text
CAR DETAILS.csv
```

### Features

| Feature | Description |
|----------|-------------|
| name | Car Name |
| year | Manufacturing Year |
| selling_price | Selling Price (Target Variable) |
| km_driven | Total Kilometers Driven |
| fuel | Fuel Type |
| seller_type | Seller Category |
| transmission | Transmission Type |
| owner | Ownership History |

---

## 🛠️ Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## ⚙️ Machine Learning Workflow

### 1. Data Collection

Load vehicle dataset using Pandas.

### 2. Exploratory Data Analysis (EDA)

- Dataset shape
- Data types
- Missing value detection
- Category distributions

Analyzed categorical features:

- Fuel Type
- Seller Type
- Transmission Type

---

### 3. Data Preprocessing

Categorical values are converted into numerical format.

#### Fuel Encoding

| Fuel Type | Value |
|------------|--------|
| Petrol | 0 |
| Diesel | 1 |
| CNG | 2 |
| LPG | 3 |
| Electric | 4 |

#### Seller Type Encoding

| Seller Type | Value |
|-------------|--------|
| Dealer | 0 |
| Individual | 1 |
| Trustmark Dealer | 2 |

#### Transmission Encoding

| Transmission | Value |
|--------------|--------|
| Manual | 0 |
| Automatic | 1 |

#### Owner Encoding

| Owner Type | Value |
|------------|--------|
| First Owner | 0 |
| Second Owner | 1 |
| Third Owner | 2 |
| Fourth & Above Owner | 3 |
| Test Drive Car | 4 |

---

### 4. Train-Test Split

Features and target variable are separated.

```python
X = car_dataset.drop(columns=['name', 'selling_price'])
Y = car_dataset['selling_price']
```

Dataset split:

```python
test_size = 0.1
random_state = 2
```

Training Data: 90%

Testing Data: 10%

---

## 📈 Model 1: Linear Regression

### Training

```python
LinearRegression()
```

### Evaluation

Model performance is measured using:

```python
R² Score
```

The model predicts car selling prices and compares them with actual values.

---

## 📈 Model 2: Lasso Regression

### Training

```python
Lasso()
```

### Evaluation

Model performance is evaluated using:

```python
R² Score
```

Lasso Regression helps reduce overfitting by applying regularization.

---

## 📊 Visualization

Scatter plots are generated for:

### Training Data

- Actual Prices
- Predicted Prices

### Testing Data

- Actual Prices
- Predicted Prices

These visualizations help evaluate model prediction quality.

---

## 📁 Project Structure

```text
used-car-price-prediction/
│
├── CAR DETAILS.csv
├── car_price_prediction.py
├── requirements.txt
├── README.md
```

---

## ▶️ Installation

### Clone Repository

```bash
git clone https://github.com/vatsal-dhuvad/used-car-price-prediction.git
```

### Navigate to Project Folder

```bash
cd used-car-price-prediction
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Project

```bash
python car_price_prediction.py
```

---

## 📊 Evaluation Metrics

The project evaluates model performance using:

### R² Score

Measures how well the model explains variance in selling prices.

```python
from sklearn import metrics
metrics.r2_score()
```

Higher values indicate better prediction performance.

---

## 📈 Sample Outputs

### Linear Regression

```text
R squared Error : 0.85
```

### Lasso Regression

```text
R squared Error : 0.84
```

*(Results may vary depending on dataset and train-test split.)*

---

## 🚀 Future Enhancements

- Random Forest Regressor
- XGBoost Regressor
- Hyperparameter Tuning
- Feature Importance Analysis
- Streamlit Web Application
- Car Price Prediction API
- Model Deployment on Cloud

---

## 💼 Real-World Applications

- Automotive Market Analysis
- Vehicle Valuation Systems
- Online Car Marketplace Platforms
- Dealership Pricing Strategy
- Resale Value Prediction

---

## 📚 Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Categorical Encoding
- Regression Analysis
- Linear Regression
- Lasso Regression
- Model Evaluation
- Data Visualization
- Predictive Analytics

---

## 👨‍💻 Author

**Vatsal Dhuvad**

GitHub: https://github.com/vatsal-dhuvad

---

## ⭐ If you found this project useful, consider giving it a star on GitHub.
