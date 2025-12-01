🚗📈 Car Price Prediction – Machine Learning Model
📌 Overview

This project predicts car prices using a combination of data cleaning, feature engineering, statistical analysis, and machine learning. After performing extensive EDA, building visual insights, and preparing clean data, a stacked model (Random Forest + Linear Regression feeding into Gradient Boosting) was developed to generate accurate price predictions.

📂 Dataset

Loaded from: Ai_data_set_third_year_project.csv

Contains features such as year, mileage, mpg, engine size, manufacturer, fuel type, and more.

Cleaned through encoding, outlier removal (IQR method), type fixing, trimming whitespace, and filtering unrealistic rows.

🛠 Tools & Libraries

Python

Pandas, NumPy – data cleaning & preprocessing

Seaborn, Matplotlib – data visualisation

Scikit-learn – ML models (Random Forest, Linear Regression, Gradient Boosting), scaling, metrics

Statsmodels – mosaic and categorical plots

Google Colab – execution environment

🔍 Steps & Workflow
1️⃣ Data Cleaning & Preparation

Removed missing values and duplicates

Encoded categorical columns

Removed outliers using the IQR method

Fixed data types and trimmed strings

Filtered unrealistic values (e.g., years outside 2010–2020)

2️⃣ Exploratory Data Analysis (EDA)

Univariate plots: histograms, boxplots

Bivariate plots: scatterplots, price relationships

Correlation heatmap

Pairplots for numerical features

Visual analysis of:

mileage vs price

engine size vs price

manufacturer effect

transmission type

fuel type patterns

3️⃣ Feature Engineering

Standardization using StandardScaler

Label encoding for categorical variables

Removal of weak features (e.g., tax column)

4️⃣ Machine Learning Model

A stacked regression model:

Random Forest → predicts price

Linear Regression → predicts price

Combined predictions → passed into

Gradient Boosting Meta-Model → final prediction

5️⃣ Evaluation

Metrics calculated:

MAE

MSE

RMSE

R² Score

Visualizations include:

Predicted vs Actual (test set)

Training set performance

Residual plots

Residual distributions

📊 Results

✔️ Clean and analysis-ready dataset

✔️ Rich visual insights into what impacts car prices

✔️ Stacked model improving prediction accuracy

✔️ Strong alignment between predicted and actual values

✔️ Error and residual analysis confirming model stability

▶️ How to Run the Project

Install dependencies:

pip install pandas numpy matplotlib seaborn scikit-learn statsmodels


Open the notebook or script (price_prediction.py).

Update the file path to your dataset if needed.

Run the script top-to-bottom in Google Colab or any Python environment.

View visual outputs and model evaluation at the bottom.
