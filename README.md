# Flight Fare Prediction using Machine Learning

## Project Overview

This project focuses on predicting flight ticket prices using Machine Learning techniques.  
The model analyzes various factors such as airline, source city, destination city, total stops, duration, and journey timing to estimate the flight fare.

The project includes:
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Model Building
- Hyperparameter Tuning
- Model Evaluation and Comparison

---

## Problem Statement

Flight ticket prices change dynamically based on several factors.  
The objective of this project is to build a regression model capable of predicting flight fares accurately using historical flight data.

---

## Dataset Information

The dataset contains information about:
- Airline
- Date of Journey
- Source
- Destination
- Route
- Departure Time
- Arrival Time
- Duration
- Total Stops
- Additional Information
- Price (Target Variable)

Dataset Size:
- Rows: ~10,000+
- Columns: 11

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

---

## Project Workflow

### 1. Data Cleaning
- Handled missing values
- Removed duplicate records

### 2. Exploratory Data Analysis (EDA)
Performed:
- Univariate Analysis
- Bivariate Analysis
- Correlation Analysis

Key visualizations:
- Price Distribution
- Airline vs Price
- Stops vs Price
- Source/Destination vs Price
- Correlation Heatmap

### 3. Feature Engineering
Extracted:
- Journey Day
- Journey Month
- Departure Hour & Minute
- Arrival Hour & Minute
- Duration Hours & Minutes

Converted categorical stop information into numerical format.

### 4. Encoding
Applied One Hot Encoding on categorical variables.

### 5. Model Building
Trained multiple regression models:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor

### 6. Hyperparameter Tuning
Used:
- GridSearchCV
- RandomizedSearchCV

to optimize model performance.

### 7. Model Evaluation
Evaluation metrics used:
- MAE
- MSE
- R² Score

---

## Model Performance

| Model | R² Score |
|-------|----------|
| Linear Regression | Lower Performance |
| Decision Tree | Moderate Performance |
| Random Forest | Good Performance |
| XGBoost | Best Performance |

Final Model R² Score:
```python
0.83
```

---

## Key Insights

- Airline and total stops significantly affect ticket prices.
- Non-stop flights are generally more expensive.
- Duration and journey timing strongly influence airfare.
- Ensemble models performed better than linear models due to complex non-linear relationships.

---

## Challenges Faced

- Handling categorical features
- Feature engineering from date/time columns
- Hyperparameter tuning
- Managing outliers without losing real-world patterns

---

## Future Improvements

Possible improvements include:
- Adding real-time flight pricing data
- Incorporating holiday and seasonal information
- Deploying the model using Flask or Streamlit
- Using advanced ensemble or stacking techniques

---

## Conclusion

This project helped me understand the complete Machine Learning workflow starting from raw data preprocessing to model evaluation and optimization.  
It also provided practical experience in feature engineering, regression modeling, and performance tuning.
