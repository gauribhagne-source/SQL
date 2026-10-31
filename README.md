# 🎬 STREAMNEXA
## Subscription Management & Customer Retention Analytics System

### 📌 1. Project Scenario

StreamNexa is a subscription-based digital entertainment company providing online streaming services to customers across different cities in India. The company offers multiple subscription plans, including Basic, Standard, Premium and Family plans.

The company faces challenges in retaining customers, as some subscribers cancel their subscriptions, fail to renew their plans or become inactive over time.

The organization wants to develop a Subscription Management & Customer Retention Analytics System to store, manage and analyse customer, subscription, payment and usage data using a structured SQL database.

The system will help the company understand customer behaviour, monitor subscription performance, analyse payment activities and identify factors responsible for customer cancellations.

### 🗄️ 2. Database Tables

#### 👥 1. Customers

The company stores personal and registration information for every customer, including:

- Customer ID
- Customer Name
- Gender
- Age
- Email
- Phone
- City
- Registration Date
- Customer Status

A customer can purchase one or more subscription plans over time and can have multiple subscription records.

#### 📦 2. Subscription Plans

The company offers different subscription plans to customers.

For example:
- Basic
- Standard
- Premium
- Family

For each plan, the system stores:

- Plan ID
- Plan Name
- Plan Type
- Plan Price
- Subscription Duration
- Plan Description
- Plan Status

A subscription plan can be associated with multiple customers and subscription records.

#### 🔄 3. Subscriptions

Customers subscribe to different plans depending on their requirements.

For each subscription, the system stores:

- Subscription ID
- Customer ID
- Plan ID
- Start Date
- End Date
- Subscription Status
- Auto-Renewal Status
- Cancellation Date

Subscription statuses include:
- Active
- Cancelled
- Expired
- Paused

A customer can have multiple subscriptions over time, and each subscription is associated with a particular plan.

#### 💳 4. Payments

Customers make payments to purchase or renew their subscriptions.

For every payment, the system stores:

- Payment ID
- Subscription ID
- Payment Date
- Payment Amount
- Payment Method
- Payment Status
- Transaction Reference

Payment statuses include:
- Successful
- Failed
- Pending
- Refunded

A subscription can have multiple payment records, allowing analysis of payment history and failed transactions.

#### 📱 5. Usage Activity

The company records customer activity to understand how frequently customers use its services.

For each activity record, the system stores:

- Activity ID
- Customer ID
- Activity Date
- Login Count
- Usage Duration
- Last Active Date
- Device Type

This information helps analyse customer engagement and identify customers with declining usage activity.

#### ❌ 6. Churn Records

The company maintains information about customers who discontinue their subscriptions.

For each churn record, the system stores:

- Churn ID
- Subscription ID
- Customer ID
- Cancellation Date
- Cancellation Reason
- Feedback
- Refund Status

Common cancellation reasons include:
- High Subscription Price
- Lack of Usage
- Better Alternatives
- Poor Service Experience
- Financial Reasons

Churn records help the company understand why customers leave and identify possible improvements in customer retention.

### 📊 3. SQL Business Analysis Question Bank

The following questions will help analyse subscription performance, customer behaviour, churn patterns and revenue.

#### 👥 Customer Analysis

1. What is the total number of registered customers?
2. How many customers are Active vs Inactive?
3. How are customers distributed across different cities?
4. How many customers registered each year?
5. Which customers have never purchased a subscription?

#### 📦 Subscription Plan Analysis

1. How many subscription plans are available?
2. How many subscriptions are associated with each plan?
3. Which subscription plan has the highest number of customers?
4. What is the average subscription price by plan type?
5. Which plans generate the highest subscription revenue?

#### 🔄 Subscription Analysis

1. How many subscriptions are Active, Cancelled, Expired and Paused?
2. How many subscriptions were started each month?
3. Which subscription plans have the highest cancellation rates?
4. What is the average subscription duration?
5. Which customers have renewed their subscriptions multiple times?
6. Which customers have multiple subscription records?

#### 💳 Payment Analysis

1. What is the total number and total amount of payments?
2. How many payments are Successful, Failed, Pending and Refunded?
3. What is the total successful payment amount?
4. Which payment methods are used most frequently?
5. Which customers have multiple failed payments?
6. What percentage of payments are successful?

#### 📱 Customer Usage Analysis

1. Which customers have the highest usage duration?
2. Which customers have the lowest login activity?
3. What is the average usage duration of customers?
4. Which device types are used most frequently?
5. Identify customers whose usage activity has declined.

#### ❌ Churn Analysis

1. What is the total number of churned customers?
2. What is the overall customer churn rate?
3. What are the most common cancellation reasons?
4. Which subscription plans have the highest churn rate?
5. What is the average time customers remain subscribed before cancelling?
6. Which months have the highest number of cancellations?

#### 🔗 Customer Retention Analysis

1. Which customers have renewed their subscriptions?
2. What percentage of customers renewed their subscriptions?
3. Which subscription plans have the highest renewal rates?
4. How many customers remained subscribed for more than one year?
5. Identify customers who previously cancelled but later subscribed again.

#### 🧩 Customer Segmentation & Classification

1. Categorize customers into Young, Adult, Middle-Aged and Senior based on age.
2. Categorize customers based on subscription duration as Short-Term, Medium-Term and Long-Term.
3. Classify customers based on usage activity as Low, Medium and High.
4. Categorize customers based on their subscription value as Low, Medium and High.
5. Classify customers based on their subscription relationship as Active, Churned, Expired or Never Subscribed.

#### 🔎 Customer Insights

1. Rank subscription plans based on total revenue using RANK().
2. Find the top 3 customers by subscription spending in each city using window functions.
3. Find customers whose total subscription spending is above the overall average using a subquery.
4. Find customers who have more than one subscription using GROUP BY and HAVING.
5. Identify customers who have never made a successful payment using joins.
6. Create a consolidated customer subscription view showing customer, plan, payment and churn information.
7. Find the monthly churn trend using date functions and aggregation.

#### 📈 Revenue & Business Performance

1. What is the total revenue generated from successful payments?
2. Which subscription plans generate the highest revenue?
3. What is the average revenue per customer?
4. Compare revenue generated from monthly and yearly plans.
5. What is the relationship between subscription cancellations and revenue trends?

### 🎓 Project Conclusion

The Subscription Churn & Customer Retention Analytics System provides a comprehensive view of customer subscriptions, payment activities, usage behaviour and cancellation patterns.

The analysis helps the company understand customer behaviour, identify subscription plans with higher churn rates, monitor payment performance and evaluate customer retention.

Customer usage and churn analysis can help identify customers who may be at risk of discontinuing their subscriptions. Revenue analysis helps the organization understand the financial impact of cancellations and subscription renewals.

Overall, this SQL project demonstrates how subscription data can be organized, analysed and transformed into meaningful business insights to support data-driven decision-making and improve customer retention.
