# Customer Segmentation & Lifetime Value Analysis

## 📌 Project Overview

Understanding customer behavior is essential for developing effective and targeted marketing strategies. This project analyzes customer demographics, purchasing behavior, customer segmentation, and customer value to identify high-value customers and opportunities for improving customer retention and revenue.

The analysis applies **RFM (Recency, Frequency, Monetary)** segmentation to classify customers based on their purchasing behavior and **Customer Lifetime Value (CLV)** to estimate the economic value of customers.

The project combines **Python for data preprocessing and analysis** with **Power BI for interactive business intelligence and dashboard visualization**.


## 🎯 Business Objectives

This project aims to:

* Understand customer characteristics based on demographic and purchasing data.
* Explore customer purchasing patterns through Exploratory Data Analysis (EDA).
* Segment customers based on purchasing behavior using RFM analysis.
* Measure customer value using Customer Lifetime Value (CLV).
* Identify high-value and at-risk customer segments.
* Generate data-driven marketing recommendations to improve customer retention and profitability.


## 📊 Dataset

The dataset contains customer demographic information, income, purchasing behavior, product spending, purchasing channels, and responses to marketing campaigns.

After preprocessing, the dataset contains:

* **2,092 customers**
* Demographic variables
* Product purchasing information
* Purchase channel information
* Marketing campaign responses
* RFM metrics
* CLV metrics
* Customer segments

### Key Variables

| Variable         | Description                             |
| ---------------- | --------------------------------------- |
| `Age`            | Customer age                            |
| `Income`         | Customer income                         |
| `Education`      | Education level                         |
| `Marital_Status` | Marital status                          |
| `TotalSpend`     | Total customer spending                 |
| `TotalPurchases` | Total number of purchases               |
| `Recency`        | Days since the customer's last purchase |
| `Frequency`      | Purchase frequency                      |
| `Monetary`       | Total purchase value                    |
| `CLV`            | Customer Lifetime Value                 |
| `Segment`        | RFM customer segment                    |
| `CLV_Segment`    | Customer value category                 |



## 🛠️ Data Preprocessing

Before performing the analysis, several preprocessing steps were conducted to improve data quality and prepare the dataset for analysis.

### Data Preparation Steps

* Handle missing values in `Income`.
* Convert customer date fields into appropriate date formats.
* Create `Age` from `Year_Birth`.
* Create `TotalChildren` from `Kidhome` and `Teenhome`.
* Calculate `TotalSpend` from product categories.
* Calculate `TotalPurchases` from purchasing channels.
* Calculate `Recency`, `Frequency`, and `Monetary` for RFM analysis.
* Calculate Customer Lifetime Value (CLV).
* Create RFM and CLV customer segments.

These steps resulted in a final dataset ready for analysis and visualization.


# 🔎 Exploratory Data Analysis

## Income Distribution

Customer income is concentrated mainly between approximately **20,000 and 85,000**, with two dominant distribution areas around 35,000–40,000 and 65,000–70,000.

A small number of customers have substantially higher income levels, including observations above 150,000.

## Customer Education

The **Graduation** group represents the largest customer population, followed by **PostGraduation**, while **UnderGraduation** has the smallest customer population.

## Marital Status

Customers categorized as **Together** represent the majority of the dataset, with approximately 1,350 customers compared with around 750 customers categorized as Alone.

## Product Spending

**Wine products** generate the highest total spending, followed by **Meat Products**. Other categories, including Gold, Fish, Sweets, and Fruits, contribute considerably less spending.

## Purchase Channels

The **Store Purchase** channel is the most frequently used purchasing channel, followed by **Web Purchase** and **Catalog Purchase**.

* Store Purchase: ~12,000
* Web Purchase: ~8,200
* Catalog Purchase: ~5,500

This indicates that physical stores remain an important purchasing channel for customers.


# 📈 RFM Analysis

## What is RFM?

RFM is a customer segmentation method based on three behavioral dimensions:

* **Recency** — how recently a customer made a purchase.
* **Frequency** — how frequently a customer makes purchases.
* **Monetary** — how much a customer spends.

Higher RFM scores indicate stronger customer value from a purchasing behavior perspective.

## RFM Segments

The analysis identified four major customer segments:

| Segment            | Customers |
| ------------------ | --------: |
| Loyal Customer     |   **654** |
| Potential Loyalist |   **621** |
| At Risk            |   **504** |
| Champion           |   **313** |

### Segment Interpretation

**🏆 Champion**

Customers with high purchase frequency, high purchase value, and strong recent activity.

**💙 Loyal Customer**

Customers who purchase regularly and have established a strong relationship with the company.

**🌱 Potential Loyalist**

Customers with the potential to become loyal customers through appropriate marketing strategies.

**⚠️ At Risk**

Customers who are becoming less active and may be at risk of churn.


# 💰 Customer Lifetime Value Analysis

## What is CLV?

**Customer Lifetime Value (CLV)** measures the economic value generated by a customer throughout their relationship with the company.

In this analysis, CLV is calculated using a combination of **Frequency and Monetary**, meaning customers who purchase frequently and spend more tend to have higher CLV.

## CLV Segmentation

Customers are divided into four value categories:

* **Low Value**
* **Medium Value**
* **High Value**
* **VIP**

The segmentation uses a **quantile-based approach**, resulting in relatively balanced customer groups.


# 📊 Power BI Dashboard

The project includes two main dashboard perspectives:

### 1. Customer Overview

The dashboard provides an overview of:

* Total Customers
* Total Revenue
* Average Income
* Average CLV
* Customer Education
* Marital Status
* Total Spending
* Purchase Channels
* RFM Segments
* CLV Segments

The dashboard reports:

* **Total Customers:** 2.092K
* **Total Revenue:** ~1M
* **Average Income:** 51.95K
* **Average CLV:** 11.09K

### 2. RFM & CLV Analysis

The second dashboard focuses on:

* RFM Segment Distribution
* CLV Segment Distribution
* RFM Relationship
* Income vs CLV
* Average CLV by RFM Segment
* Revenue by CLV Segment

Key metrics include:

* **Average RFM Score:** 9.03
* **Average CLV:** 11.09K
* **Highest CLV:** 71K
* **Champion Customers:** 313


# 💡 Key Findings

### 1. Loyal Customer is the largest RFM segment

Loyal Customers account for **654 customers**, followed by **621 Potential Loyalists**.

This indicates that the business already has a substantial base of customers with strong potential for retention and further value development.

### 2. Champion customers generate the highest customer value

The Champion segment contains **313 customers** and has the highest average CLV at approximately **28K**.

This confirms that customers with stronger RFM profiles also tend to generate greater economic value.

### 3. VIP customers contribute the largest revenue

The **VIP CLV segment generates approximately 772K in revenue**, making it the largest revenue-contributing CLV segment.

This indicates that high-value customers represent an important source of business revenue.

### 4. Income and customer value show a positive relationship

The Income vs CLV analysis indicates a positive relationship between customer income and CLV, suggesting that customers with higher income levels tend to generate greater customer value.

### 5. Store remains the dominant purchase channel

Store Purchase is the most frequently used purchasing channel, while Web Purchase also shows strong activity.

This creates an opportunity to strengthen digital purchasing without neglecting the existing physical-store customer base.



# 🎯 Business Recommendations

## 1. Retain Champion Customers

Prioritize Champion customers through:

* Exclusive loyalty programs
* Special rewards
* Early access to promotions
* Personalized communication

The objective is to maintain their loyalty and protect their high contribution to revenue.

## 2. Convert Loyal Customers into Champions

Loyal Customers represent the largest RFM segment and therefore provide a significant opportunity for value growth.

Potential strategies include:

* Cross-selling
* Upselling
* Repeat-purchase rewards
* Personalized offers

## 3. Reactivate At-Risk Customers

The At Risk segment contains customers who are becoming less active.

A **win-back campaign** can be used through:

* Discount vouchers
* Special offers
* Personalized reminders
* Email campaigns

## 4. Prioritize VIP & High Value Customers

Since VIP and High Value customers contribute substantially to revenue, marketing investment can be prioritized toward these segments to maximize potential return on investment.

## 5. Develop Potential Loyalists

Potential Loyalists can be targeted with personalized product recommendations, relevant promotions, and loyalty programs designed to encourage more frequent purchases.



# 🧰 Tools & Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Google Colab**
* **Power BI**



# 🔄 Project Workflow

Customer Dataset
       ↓
Data Understanding
       ↓
Data Preprocessing
       ↓
Feature Engineering
       ↓
Exploratory Data Analysis
       ↓
RFM Analysis
       ↓
Customer Segmentation
       ↓
CLV Calculation
       ↓
CLV Segmentation
       ↓
Power BI Dashboard
       ↓
Business Insights
       ↓
Marketing Recommendations


# 📌 Conclusion

This project demonstrates how customer transaction and demographic data can be transformed into actionable marketing insights through **RFM segmentation and Customer Lifetime Value analysis**.

The analysis identifies **Champion, Loyal Customer, Potential Loyalist, and At Risk** segments while also classifying customers into **Low Value, Medium Value, High Value, and VIP** categories.

The findings highlight the importance of retaining high-value customers, developing loyal and potential-loyal customers, reactivating at-risk customers, and optimizing marketing investment based on customer value.

By combining behavioral segmentation with CLV analysis, businesses can move from broad marketing strategies toward more targeted and data-driven customer management.
