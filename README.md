# Product Sales Analysis and  Forecasting





This project analyzes historical sales data to identify trends and build a machine learning model for sales forecasting.

## Business Problem We Are Solving


The project aims to analyze historical sales data to identify trends and patterns. The primary business problem addressed is the need to accurately forecast future sales based on various factors such as time of year, location, and product. This allows businesses to optimize inventory, plan marketing strategies, and improve resource allocation. Additionally, understanding product relationships and optimal purchase times helps in promotional planning and maximizing revenue.

## Aim

- Perform EDA to understand sales trends (months, cities, products).
- Identify frequently co-purchased products.
- Build and optimize ML models (Random Forest, Gradient Boosting, Neural Network) to predict sales amounts.
- Evaluate model performance (R², MSE) and select the best one for forecasting.

## Approach

- **Data Loading and Cleaning:** Load data, handle missing values, and correct data types.
- **Feature Engineering:** Create 'month', 'hour', 'minute', and combined 'city' features.
- **Exploratory Data Analysis (EDA):** Visualize sales trends over time and locations, analyze products.
- **Data Preprocessing for ML:** One-hot encode categorical features.
- **Model Selection and Training:** Train Random Forest, Gradient Boosting, and Neural Network regressors.
- **Model Evaluation:** Assess performance using R² and MSE.
- **Model Optimization:** Use GridSearchCV for hyperparameter tuning.
- **Comparison of Models:** Compare initial and optimized model performance.

## Data Analysis and EDA

- Data loaded from a GitHub CSV.
- Missing values handled and data types converted.
- Features like 'month', 'sales', 'city', 'Hour', and 'Minute' created.
- Visualizations show:
    - Sales peak in certain months (e.g., December).
    - Top-performing cities for sales.
    - Peak hours for placing orders (e.g., around 11 am and 7 pm).

## Months Vs Total Sales 

![sales-2](https://user-images.githubusercontent.com/72175654/215282847-b0541ee1-feb5-419b-abd1-0486ff06feb8.png)

## Product vs Quantity ordered
![sales-1](https://user-images.githubusercontent.com/72175654/214647801-66922c23-6c45-4869-92cc-83074e38b0fe.png)

## Sales vs City
![Image](https://github.com/user-attachments/assets/8c7d3b4a-e85e-46b3-bb04-844ea7a56af3)

- Analysis identifies frequently sold together products (e.g., iPhone and Lightning Charging Cable).
- Visualization shows a general inverse relationship between product price and quantity ordered.

## Dashbord
![sales-3](https://github.com/Bhawani-Rabisankar-Sahoo/Sales_Analysis/assets/72175654/48ccefce-9b5c-4ebc-9f56-d343a54e3da4)

## Machine Learning

- The task is framed as a regression problem to predict 'sales'.
- Features used: 'month', 'Hour', 'Minute', one-hot encoded 'city', and 'Product'.
- Data split into training and testing sets.
- Initial models trained: Random Forest, Gradient Boosting, and Neural Network.
- GridSearchCV used to optimize hyperparameters for each model.

  ![Image](https://github.com/user-attachments/assets/67a5c4aa-127f-46f6-bb7c-1446d1709764)

## Result

- EDA successfully revealed sales trends and patterns.
- Identification of frequently co-purchased items provides insights for bundling.
- Initial models showed reasonable performance.
- Optimization using GridSearchCV significantly improved model performance.
- **Optimized Model Performance Comparison (on Test Set):**

| Model                       | R² Score | MSE        |
|-----------------------------|----------|------------|
| Optimized Random Forest     | 0.8440   | 1384.7062 |
| Optimized Gradient Boosting | 0.8807   | 1058.5110 |
| Optimized Neural Network    | 0.9502   | 442.3473 |

![Image](https://github.com/user-attachments/assets/4825c289-51cb-4852-b409-7a036821079f)
![Image](https://github.com/user-attachments/assets/0914f4b5-33c3-4a52-87c9-e745c570e814)


- The Optimized Neural Network and Gradient Boosting models achieved the highest R² scores and lowest MSE, indicating superior performance in predicting sales.

## Impact on Business

- **Optimized Inventory:** Accurate sales forecasts reduce storage costs and stockouts.
- **Targeted Marketing:** Identifying peak periods and top cities enables effective campaign planning.
- **Improved Product Bundling:** Insights from co-purchased items increase sales and average order value.
- **Enhanced Customer Service:** Understanding peak order hours optimizes staffing.
- **Data-Driven Decisions:** Provides a framework for informed decisions in sales planning and resource allocation.


