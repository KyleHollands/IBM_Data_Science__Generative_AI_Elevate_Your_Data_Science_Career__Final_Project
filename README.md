# IBM Data Science: Machine Learning with Python - Test Environment for Generative AI Labs  

## Project Overview  
This project provides a test environment for Generative AI classroom labs, focusing on analyzing and predicting car prices using machine learning techniques. The goal is to explore feature engineering, model selection, and evaluation methods to build accurate predictive models for vehicle prices based on various car attributes.  

## Data Understanding  
The dataset used in this project contains information about used cars, including attributes such as:  

- **Year**: Manufacturing year of the car  
- **Mileage**: Distance traveled (miles)  
- **Tax**: Annual tax cost (£)  
- **MPG**: Miles per gallon (fuel efficiency)  
- **Engine Size**: Engine capacity in liters  
- **Fuel Type**: Type of fuel used (e.g., petrol, diesel)  
- **Transmission**: Type of transmission (e.g., manual, automatic)  
- **Price**: Sale price of the car (£)  

The dataset was cleaned by handling missing values (replaced with column means), removing duplicate rows, and ensuring data integrity for analysis.  

## Modeling and Evaluation  
Several machine learning models were evaluated to predict car prices, including:  

- **Linear Regression**: Baseline model for price prediction based on MPG.  
- **Multiple Linear Regression**: Extended model incorporating multiple features like year, mileage, tax, MPG, and engine size.  
- **Polynomial Regression**: Captured non-linear relationships between features and price.  
- **Ridge Regression**: Regularized model to prevent overfitting.  
- **Polynomial Ridge Regression**: Combined polynomial features with Ridge regularization for improved accuracy.  

Hyperparameter tuning was performed using **GridSearchCV** to optimize Ridge regression's alpha parameter.  

### Key Findings:  
- **Feature Importance**: Year, mileage, and engine size were identified as significant predictors of car price.  
- **Best Performing Model**: Polynomial Ridge Regression achieved the highest R-squared value (~0.768) and the lowest mean squared error (5,240,266).  
- **Model Comparison**: Polynomial models outperformed linear models, indicating non-linear relationships between features and price.  

## Business Understanding  
The primary stakeholders for this project include car dealerships, buyers, and sellers in the used car market. Accurate price predictions can help:  

- **Dealerships**: Set competitive prices and optimize inventory management.  
- **Buyers**: Make informed decisions based on fair market value.  
- **Sellers**: Determine optimal listing prices for their vehicles.  

## Interactive Visualizations  
Interactive visualizations were developed to analyze car price distributions and relationships between features:  

- **Box Plot**: Visualized price outliers grouped by transmission type.  
- **Regression Plot**: Explored the relationship between MPG and car price, including correlation statistics.  

### Key Insights:  
- **Transmission Type**: Automatic cars generally had higher prices than manual cars.  
- **MPG vs. Price**: Fuel efficiency showed a weak negative correlation with car price, likely due to trade-offs with engine size and performance.  
- **Year and Engine Size**: Newer cars and larger engine sizes were associated with higher prices.  

## Conclusion  
The analysis revealed that car year, mileage, and engine size are critical factors in determining car prices. Polynomial Regression emerged as the best-performing model, capturing non-linear relationships and providing accurate predictions. These insights can help stakeholders in the used car market make data-driven decisions.  

## Next Steps  
Future work will focus on:  
- Incorporating additional features (e.g., brand, condition, location).  
- Exploring advanced models like Gradient Boosting and Neural Networks.  
- Building an interactive web application for real-time price predictions.  

By continuously improving the model and incorporating more features, we can enhance its predictive accuracy and provide even more valuable insights for stakeholders.  