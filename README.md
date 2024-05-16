# Customer Churn Analysis Using SyriaTel Dataset

![SyriaTel](https://github.com/vkeya/Phase3_Project/blob/master/Phase3_images/SyriaTel_Logo.jpg))



## Overview

This project aims to analyze customer churn behavior using the SyriaTel dataset from the telecommunications industry. 
The analysis involves understanding customer attributes, identifying patterns, and predicting churn using various machine learning models.

## Business and Data Understanding

### Business Understanding
Customer churn is a critical issue in the telecommunications industry, directly impacting revenue and growth. 
By understanding the factors that contribute to churn, SyriaTel company can devise strategies to retain customers and enhance their services.

### Data Understanding
The SyriaTel dataset contains detailed information about customer usage patterns, plans, and service interactions. 
Key attributes include account length, international plan, voice mail plan, total call minutes across different times of the day, customer service calls, and whether the customer churned or not.

#### Dataset Choice
The SyriaTel dataset is chosen for its comprehensive coverage of customer behavior and service usage. It includes attributes such as:
- `Account length`: Duration of the customer's account in days.
- `International plan`: Indicator if the customer has an international calling plan.
- `Voice mail plan`: Indicator if the customer has a voice mail plan.
- `Number vmail messages`: Number of voice mail messages.
- `Total day minutes`, `Total eve minutes`, `Total night minutes`, `Total intl minutes`: Total minutes of calls during day, evening, night, and international.
- `Total day calls`, `Total eve calls`, `Total night calls`, `Total intl calls`: Number of calls during day, evening, night, and international.
- `Total day charge`, `Total eve charge`, `Total night charge`, `Total intl charge`: Charges for calls during day, evening, night, and international.
- `Customer service calls`: Number of customer service calls.
- `Churn`: Indicator if the customer churned (1) or not (0).

#### Stakeholder Audience
The primary stakeholders for this analysis are the customer retention team, marketing strategists, and senior management within the telecommunications company. 
They are interested in identifying the key factors driving customer churn and developing strategies to reduce churn rates.

## Modeling
The project employs various machine learning models to predict customer churn. These models include:
- Logistic Regression
- Decision Trees
- Random Forests
  
Various machine learning models are used and tested to predict customer churn.
The process involves:
1. **Data Preprocessing**: Handling missing values, encoding categorical variables, and normalizing numerical features.
2. **Model Training**: Using algorithms such as Logistic Regression, Decision Trees and Random Forests.
3. **Hyperparameter Tuning**: Optimizing model parameters to improve performance.
4. **Feature Selection**: Identifying the most important features contributing to churn.

## Evaluation
The models are evaluated based on:
- **Accuracy**: Proportion of correctly predicted churn and non-churn cases.
- **Precision**: Proportion of true positive churn predictions out of all positive predictions.
- **Recall**: Proportion of true positive churn predictions out of all actual churn cases.
- **F1 Score**: Harmonic mean of precision and recall.

## Conclusion
The analysis reveals key insights into customer behavior and churn patterns. 
High usage during the day, frequent international calls, and multiple customer service interactions are significant predictors of churn. 
These insights can guide the development of customer retention strategies, such as targeted offers for high-risk customers and improved customer service.

## Limitations
Phone Number Column: The 'phone number' column is likely irrelevant for predictive modeling and should be removed or transformed.
Geographic Information: The 'state' column may introduce regional biases and might need to be encoded properly or analyzed for its impact on churn.
Account Length: While this could be a significant feature, without context (e.g., is a longer account length generally better or worse?), it might be hard to interpret its impact directly.

## Recommendations
Address High Charges: Analyze the relationship between high total charges and churn. 
Consider offering discounts or loyalty programs to high-usage customers to enhance their satisfaction and reduce churn risk.

Improve Customer Service: Since frequent customer service calls are a strong churn predictor, focus on improving the quality of customer service. 
Implement training programs for service representatives and ensure quick resolution of customer issues.

Monitor High Usage: Keep an eye on customers with high total day minutes and total minutes. 
Provide them with personalized offers or services to increase their satisfaction.

International Plan Customers: Pay special attention to customers with international plans. 
Ensure their specific needs are met, possibly by providing better international call rates or packages.
