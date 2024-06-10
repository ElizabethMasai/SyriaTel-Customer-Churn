## SYRIATEL CUSTOMER CHURN
Author:Elizabeth Masai

TM:Asha Deen

## Overview 

In the world of telecommunications, keeping customers is just as important as acquiring new ones. For SyriaTel, a telecommunications company based in Syria,the cost of acquiring a new customer is six times higher than retaining an existing one . Therefore, understanding why customers leave, or "churn," is crucial for the company's financial well being. This project therefore aims at helping SyriaTel tackle this challenge by building a classifier to predict whether a customer will soon stop doing business with the telecommunication company.

## Problem statement

SyriaTel, a telecommunications company, is facing the challenge of customer churn, where customers decide to end their subscription. This churn rate is currently at approximately 15%. The company wants to understand if there are any predictable patterns or factors that contribute to customer churn. By identifying these patterns, SyriaTel aims to develop strategies to reduce churn and retain more customers, ultimately improving their financial performance and well being.

## Objectives

1.Identify Predictive Patterns: Analyze the provided dataset from SyriaTel to identify patterns and factors that are associated with customer churn. This involves exploring various features such as call minutes, charges, customer service calls, and plan details to understand their impact on churn.

2.Build a Churn Prediction Model: Develop a binary classification model using machine learning techniques to predict whether a customer is likely to churn or not. The model should be trained on historical customer data and evaluated using appropriate metrics such as accuracy, precision, recall, and F1-score.

3.Provide Actionable Insights: Generate actionable insights and recommendations based on the analysis and model results. These insights should help SyriaTel make informed decisions and develop targeted strategies to reduce churn, such as improving customer service, offering personalized promotions, or enhancing plan features.

## Data Understanding

The dataset is sourced from kaggle and it plays an important role in  coming up with predictive models that will aid in mitigating financial losses and customer retention.

## Data Preparation

This involves checking for outliers,duplicates and null values which if not worked on will lead to misleading end results.

## Exploratory Data Analysis

 This step involves better understanding of the data, identifying patterns, and testing various assumptions. Data visualization plays a key role in streamlining this process making it easier to analyze and communicate the findings.
It entails looking at the Univariate analysis,Bivariate analysis and Multivariate analysis

## Univariate analysis 
It involves examining the distribution of single variables.
 
![Churn distribution](https://github.com/ElizabethMasai/SyriaTel-Customer-Churn-Project/assets/150329461/df53a8c6-689d-48cd-8af8-e0e49097f536)

It also examins numerical and categorical variables and how they relate with the target variable "churn".


![Numeric variables](https://github.com/ElizabethMasai/SyriaTel-Customer-Churn-Project/assets/150329461/14ec4b41-5f01-433f-8239-d3658ca4a421)

## Bivariate Analysis

- This entails analysing the relatioship between two variables to understand the relatiosnhip between them.

State vs. Churn: inspects to see if the churn rates vary significantly across different states. This can reveal geographic patterns in customer behavior.

-Voice Mail Plan vs. Churn: determines if having a voice mail plan affects the likelihood of a customer churning. This can indicate if certain services are retaining customers better or not

-International Plan vs. Churn: Checks to find out if customers with an international plan are more or less likely to churn. This can help in understanding if offering international plans is beneficial in reducing churn.
![Voice mail distribution](https://github.com/ElizabethMasai/SyriaTel-Customer-Churn-Project/assets/150329461/5bbaff29-4538-453c-b566-bc426d008718)




![International distribution](https://github.com/ElizabethMasai/SyriaTel-Customer-Churn-Project/assets/150329461/a3aad26e-16f1-484a-89e2-2939f8f27f33)


## Multivariate Analysis

 It helps us identify complex patterns and correlations between various features such as total day minutes, total day calls, total day charge, voice mail plan, international plan, and churn. This in return helps us in understanding and providing valuable insights for decision-making and strategy development while trying to solve the churn problem.The correlation matrix of the relationship in shown in the figure below.
 
![Correlation heatmap](https://github.com/ElizabethMasai/SyriaTel-Customer-Churn-Project/assets/150329461/0cb2ae82-afeb-4bc4-a47b-8611df93a6a1)

## Modeling

This step entails selecting and training a machine learning algorithm, validating its performance, and refining it to ensure accuracy and generalizability. The modeling process aims at accurately predicting customer churn by identifying at risk customers,optimizing market efforts and also improving customer retention.

Algorithms such as Logistic Regression, Random Forest, and Decision Trees combined with preprocessing techniques like SMOTE and scaling, will provide a clear framework for achieving these goals.

## Model Evaluation

ROC and AUC are used to assess the models.Recall sores measures the proportion of actual positive instances that were correctly identified by the model. A higher recall score indicates that the model has a strong ability to identify positive instances correctly.

##  Conclusions and Recommendations 
XGBoost is the best algorithm to use due to its highest recall and F1-Score, making it effective at identifying churn while minimizing false positives. If computational resources are limited or model interpretability is important, Random Forest is also a reliable choice.


## Recommendations



![download](https://github.com/ElizabethMasai/SyriaTel-Customer-Churn-Project/assets/150329461/4e2d13b5-3962-48fd-8e9e-8d61fa0d7523)


![download](https://github.com/ElizabethMasai/SyriaTel-Customer-Churn-Project/assets/150329461/3fc7b58c-9a86-4c11-beca-719f63d605c8)



Looking at the Feature importance visual above, the following recommendations will arise:

Since customer service calls have the highest importance, it's necessary to focus on improving customer service,this can be done by implementing better training for customer service representatives, reducing wait times, and resolving issues more efficiently will eventually reduce churn.

Total Day Minutes and Total Day Charge -Customers with higher usage might be more prone to churn if they feel they are not getting value for money. Syriatel should therefore consider offering better day-time packages or discounts to heavy users to make them feel valued and reduce their churn rates.

International Plan- The presence of an international plan is a strong predictor of churn. Evaluate the current international plan's competitiveness in terms of price and features. Introduce more attractive international calling plans or special offers to make these plans more appealing to the customers who might be on the verge of terminating their contracts.

 


