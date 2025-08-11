🚗 Car Price Prediction using Machine Learning
📌 Overview
This project predicts the selling price of used cars based on various features like car name, year, fuel type, seller type, transmission, and owner history.
It uses Polynomial Regression and Linear Regression models to train on historical car sales data and make predictions.

The dataset is sourced from CarDekho and is publicly available.

Main Features:

name – Car model and variant

year – Year of manufacture

km_driven – Kilometers driven

fuel – Fuel type (Petrol, Diesel, CNG, etc.)

seller_type – Dealer or Individual

transmission – Manual or Automatic

owner – Ownership history

selling_price – Target variable (price to predict)

🛠️ Steps in the Project
1. Data Exploration & Cleaning
Display dataset info, shape, and descriptive statistics

Handle missing values and drop duplicates

Extract brand name from car name column (name_2)

2. Data Visualization
Count plots for brand, year, fuel type, seller type, transmission, owner

Pie charts for distribution analysis

Heatmap for feature correlations

Crosstab visualizations for brand vs transmission & owner

3. Data Preprocessing
Label Encoding for categorical variables

MinMaxScaler for feature scaling

4. Modeling
Polynomial Regression (degree=2)

Linear Regression (alternative approach in comments)

Train-Test split (70%-30%)

Evaluate model with:

R² Score

Mean Squared Error

5. Model Saving
Option to save trained Linear Regression model with pickle

📦 Libraries Used
python
Copy
Edit
numpy  
pandas  
matplotlib  
seaborn  
scikit-learn  
pickle

📈 Example Output
Model Performance:

R² Score: ~0.87 (varies with dataset shuffle)

Polynomial regression captures complex relationships between features and price.

Sample Prediction (Linear Regression model):

python
Copy
Edit
['Hyundai Verna 1.6 SX', 2016, 50000, 'Petrol', 'Individual', 'Manual', 'First Owner']
→ Predicted Price: ₹ 5.4 Lakh

📌 Future Improvements
Deploy as a web app using Flask or Streamlit

Use advanced models like Random Forest or XGBoost

Hyperparameter tuning for better accuracy


