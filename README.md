# Customer Churn Analysis Using SyriaTel Dataset

![SyriaTel](https://github.com/vkeya/Phase3_Project/blob/master/Phase3_images/SyriaTel_Logo.jpg)



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

### Dataset Choice

The SyriaTel dataset is chosen for its comprehensive coverage of customer behavior and service usage. It includes attributes such as:

Account length: The duration (in days) that the customer has had an account with the company.

International plan: Binary indicator of whether the customer has an international calling plan (1 = Yes, 0 = No).

Voice mail plan: Binary indicator of whether the customer has a voice mail plan (1 = Yes, 0 = No).

Number vmail messages: Number of voice mail messages the customer has.

Total day minutes: Total number of minutes the customer has used during the day.

Total day calls: Total number of calls the customer has made during the day.

Total day charge: Total charge for the customer's day usage.

Total eve minutes: Total number of minutes the customer has used during the evening.

Total eve calls: Total number of calls the customer has made during the evening.

Total eve charge: Total charge for the customer's evening usage.

Total intl calls: Total number of international calls made by the customer.

Total intl charge: Total charge for the customer's international usage.

Customer service calls: Number of calls the customer has made to customer service.

Churn: Binary indicator of whether the customer has churned (1 = Yes, 0 = No).

Total_calls: Total number of calls made by the customer.

Total_minutes: Total number of minutes the customer has used.

Total_charge: Total charge for the customer's usage.

Day_calls_per_minute: Ratio of day calls to day minutes.

Eve_calls_per_minute: Ratio of evening calls to evening minutes.

Night_calls_per_minute: Ratio of night calls to night minutes.

### Stakeholder Audience

The primary stakeholders for this analysis are the customer retention team, marketing strategists, and senior management within the telecommunications company. 

They are interested in identifying the key factors driving customer churn and developing strategies to reduce churn rates.

## Methodology

The analysis of this dataset was conducted using a series of methodical steps to extract meaningful insights and develop a predictive model to identify potential churners. 

Below is a breakdown of the methodology employed:

### Data Preprocessing:

Data Cleaning: Identifying and handling missing values, outliers, and any inconsistencies in the data.

Data Transformation: Converting categorical variables into numerical formats using techniques such as one-hot encoding.

### Exploratory Data Analysis (EDA):

Descriptive Statistics: Calculating summary statistics for each column to understand the central tendency and dispersion of the data.

![Statistics](https://github.com/vkeya/Phase3_Project/blob/master/Phase3_images/Descriptive%20statistics.png)

Visualization: Using various plots (histograms, box plots, scatter plots) to visually inspect the distribution of variables and relationships between them.

#### Univariate Analysis

![Univariate](https://github.com/vkeya/Phase3_Project/blob/master/Phase3_images/Univariate_Analysis.png)

#### Bivariate Analysis

![Bivariate](https://github.com/vkeya/Phase3_Project/blob/master/Phase3_images/Bivariate_Analysis.png)

#### Multivariate Analysis

![Multivariate](https://github.com/vkeya/Phase3_Project/blob/master/Phase3_images/Multivariate_Analysis.png)

### Feature Engineering:

New Features: Creating new features such as Total_calls, Total_minutes, and Total_charge to provide additional insights.

Ratios and Proportions: Calculating ratios such as Day_calls_per_minute, Eve_calls_per_minute, and Night_calls_per_minute to capture customer behavior more effectively.

## Modeling

Model Selection: We Evaluated different machine learning models (i.e., logistic regression, decision trees, random forests) to predict churn.

Model Training: Splitting the dataset into training and testing sets to train the selected model.

Model Evaluation: Assessing the performance of the model using metrics such as accuracy, precision, recall, and F1-score.

## Evaluation

The models are evaluated based on:

- **Accuracy**: Proportion of correctly predicted churn and non-churn cases.
- 
- **Precision**: Proportion of true positive churn predictions out of all positive predictions.
- 
- **Recall**: Proportion of true positive churn predictions out of all actual churn cases.
- 
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
