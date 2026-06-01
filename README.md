# Customer Shopping Behavior Analysis

## 📌 Project Overview

This project analyzes customer shopping behavior using transactional data from **3,900 customer purchases** across multiple product categories. The objective is to uncover insights into customer spending patterns, subscription behavior, product performance, and demographic trends to support strategic business decisions.

The project follows an end-to-end analytics workflow using:

* **Python** for data cleaning, preprocessing, and feature engineering
* **MySQL** for data storage and business analysis
* **Power BI** for interactive dashboard development and visualization

---

## 📊 Dataset Summary

| Metric         | Value                        |
| -------------- | ---------------------------- |
| Records        | 3,900                        |
| Features       | 18                           |
| Missing Values | 37 values in `review_rating` |

### Key Attributes

**Customer Information**

* Age
* Gender
* Location
* Subscription Status

**Purchase Information**

* Item Purchased
* Category
* Purchase Amount
* Season
* Size
* Color

**Shopping Behavior**

* Discount Applied
* Previous Purchases
* Frequency of Purchases
* Review Rating
* Shipping Type

---

## 🐍 Data Cleaning & Preprocessing

### Data Exploration

* Loaded data using Pandas
* Performed data inspection using:

  * `df.info()`
  * `df.describe()`
  * Null value checks

### Missing Value Treatment

* Identified 37 missing values in the `review_rating` column
* Filled missing values using the median rating within each category

### Data Standardization

* Renamed columns using snake_case convention
* Checked data consistency and duplicates

### Feature Engineering

Created additional features:

* `age_group`
* `purchase_frequency_days`

### Data Optimization

* Verified redundancy between `discount_applied` and `promo_code_used`
* Removed the redundant `promo_code_used` field

### MySQL Integration

* Connected Python to MySQL using **mysql-connector-python**
* Created database tables
* Loaded the cleaned dataset into MySQL
* Verified successful data insertion

---

## 🗄️ SQL Business Analysis (MySQL)

The following business questions were answered using SQL:

### Revenue Analysis

* Revenue by Gender
* Revenue by Age Group
* Revenue by Subscription Status

### Customer Behavior Analysis

* High-Spending Discount Users
* Repeat Buyers vs Subscription Status
* Customer Segmentation

### Product Analysis

* Top 5 Products by Rating
* Top 3 Products per Category
* Discount-Dependent Products

### Operational Analysis

* Shipping Type Comparison
* Purchase Frequency Trends

---

## 📈 Power BI Dashboard

### Dashboard Preview

### Dashboard KPIs

* Total Customers: **3.9K**
* Average Purchase Amount: **$60**
* Total Review Ratings: **14.63K**

### Interactive Filters

* Subscription Status
* Gender
* Product Category
* Shipping Type

### Visualizations

* Subscription Percentage Distribution
* Revenue by Category
* Sales by Category
* Revenue by Age Group
* Purchase Amount by Age Group

### Key Insights

* Clothing generated the highest sales revenue.
* Most customers are non-subscribers.
* Young adults contribute the highest revenue.
* Express and premium shipping users tend to spend more.
* Customer spending varies significantly across product categories.

---

## 💡 Business Recommendations

### Increase Subscription Adoption

Offer exclusive discounts, loyalty rewards, and early-access promotions.

### Strengthen Customer Retention

Develop loyalty programs targeting repeat buyers.

### Optimize Discount Strategy

Monitor discount effectiveness to balance profitability and sales growth.

### Promote Top Products

Feature highly-rated and top-selling products in marketing campaigns.

### Improve Customer Targeting

Focus marketing efforts on:

* Young Adults
* High-spending customers
* Frequent purchasers

---

## 🛠️ Tech Stack

| Technology             | Purpose                             |
| ---------------------- | ----------------------------------- |
| Python                 | Data Cleaning & Feature Engineering |
| Pandas                 | Data Manipulation                   |
| MySQL                  | Data Storage & Analysis             |
| mysql-connector-python | Database Connectivity               |
| SQL                    | Business Queries                    |
| Power BI               | Dashboard Development               |

---

## 📂 Project Structure

```text
customer-shopping-behavior-analysis/
│
├── data/
│   └── customer_shopping_behaviour.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── sql_queries/
│   └── analysis.sql
│
├── dashboard/
│   └── customer_purchase_dashboard.pbix
│
├── images/
│   └── customer_purchase_dashboard.png
│
├── README.md
└── requirements.txt
```

---

## 🎯 Project Outcome

This project demonstrates an end-to-end data analytics workflow from data preparation and database integration to business intelligence reporting. The insights generated can help businesses improve customer retention, optimize marketing campaigns, enhance subscription growth, and maximize revenue.

## 👤 Author

**Your Name**

Data Analyst | Python | SQL | MySQL | Power BI
