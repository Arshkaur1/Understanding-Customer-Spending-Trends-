# Understanding Customer Spending Trends for Smarter Business Decisions

## Project Overview
This project aims to analyze customer shopping behavior using a comprehensive dataset that includes demographic details, purchasing habits, seasonal trends, and promotional activities. The objective is to uncover key factors influencing individual transaction spending and identify traits that predict repeat purchase behavior and subscription loyalty.

## Dataset
The analysis utilizes the **Customer Shopping Trends Dataset** from Kaggle, containing 3,900 customer transactions.
* **Scope:** 19 variables capturing customer demographics, purchase patterns, and payment preferences.
* **Key Columns:** Age, Gender, Item Purchased, Purchase Amount (USD), Location, Size, Color, Season, Review Rating, Subscription Status, Shipping Type, and Previous Purchases.

## Analysis & Key Findings

### 1. Exploratory Data Analysis (EDA)
* **Category Dominance:** Clothing consistently leads in sales across all seasons, making it the most demanded category year-round.
* **Seasonal Spikes:** Accessories follow as the second-highest contributor, with noticeable spikes during Fall and Summer.
* **Subscription & Loyalty:** Customers with an active subscription show a higher average number of past purchases, indicating a strong link between subscription status and repeat buyer behavior.

### 2. Spending Behavior Insights
* **Linear Modeling:** A linear regression model identified that **Season** has the most consistent impact on spending, though the overall model's low $R^2$ (0.0078) suggests spending behavior is highly complex.
* **Non-Linear Patterns:** A follow-up Decision Tree model provided a clearer structure, identifying **Age** as the most influential variable, followed by **Review Rating**, **Shipping Type**, and **Payment Method**.

### 3. Subscription Prediction
A logistic regression model was developed to predict subscription status with strong results:
* **Performance:** Achieved **82.67% accuracy** and a **Kappa of 0.62**, indicating substantial predictive power.
* **Primary Predictor:** **Express Shipping** was significantly associated with a higher likelihood of subscription.
* **Monetary Incentives:** Interestingly, discounts and promo codes had no meaningful impact on subscription decisions, suggesting that convenience and urgency are stronger drivers than financial incentives.

### 4. Customer Segmentation (Clustering)
Using **K-Means Clustering** ($K=3$) and **Principal Component Analysis (PCA)**, the project identified three distinct customer personas:
* **Cluster 1 - High-Value Customers:** Individuals who make fewer purchases but spend significantly more on average.
* **Cluster 2 - New or Budget Shoppers:** Price-sensitive customers with the fewest purchases and lowest spend per transaction.
* **Cluster 3 - Loyal Mid-Spenders:** Frequent shoppers with moderate spending habits who are prime candidates for retention programs.

## Conclusion
The analysis suggests that businesses should prioritize **convenience and delivery options** over financial discounts to promote long-term engagement. Furthermore, inventory planning should be adjusted to align accessory stock with Fall and Summer peaks while maintaining high clothing inventory year-round.

---
**Project Contributors:** Arshdeep Kaur, Eisha Chaudhary, Maharsh Khamar, Shahzaib Rahat
