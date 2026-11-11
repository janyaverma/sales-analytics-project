
## 1. Purpose

This document records the 14 analytical questions supplied by the hypothetical client. They define the expected analytical scope of the Power BI deliverable and provide a reference for data preparation, modeling, measure development, validation, and dashboard acceptance.

The requirements are grouped by business domain for navigation.

## 2. Detailed Analytical Requirements

### 2.1 Executive Sales Overview

#### BR-01 — Core Sales and Customer KPIs

**Client requirement:** Create visuals showing:

1. Total customers.
2. Total orders.
3. Total sales.
4. Average order value (**total sales / total orders**).
5. Count of customers who have not purchased in the last **12 months**.

### 2.2 Product and Category Performance

#### BR-02 — Product Category Contribution to Sales

**Client requirement:** Calculate each product category's percentage contribution to overall sales. Apply the following category color rules:

- **Green:** contribution **> 5%**.
- **Cream:** contribution **3%–5%**.
- **Yellow:** contribution **< 3%**.

Display percentage values using a **blue gradient**.

#### BR-04 — Product Photos and Quantity Sold

**Client requirement:** Analyze the relationship between the number of product photos available on the website and the quantity of products sold. **Each order row counts as one unit of quantity.** Determine whether products with more photos tend to sell in greater quantities.

#### BR-05 — Market Basket Analysis

**Client requirement:** Identify products frequently purchased together in the **same order**, to inform cross-selling, bundling, and targeted marketing strategies.

#### BR-06 — Recently Launched Product Performance

**Client requirement:** Evaluate each category using products introduced within the **last six months relative to the latest date in the dataset**. Include **total sales** and **total orders** for these products.

#### BR-07 — Monthly Product Sales Seasonality

**Client requirement:** Identify products whose sales exhibit recurring **monthly** seasonal patterns, supporting inventory planning, promotions, and marketing.

#### BR-08 — Product Price Changes and Sales

**Client requirement:** Calculate the **average change in product prices over the last year** for each category and analyze its relationship with sales, to inform pricing strategy.

#### BR-13 — Category Revenue: First 90 Days vs. Most Recent 90 Days

**Client requirement:** For each product category, compare total revenue during its **first 90 days on the platform** with revenue during the **most recent 90 days** to assess product-line maturity.

### 2.3 Customer Retention and Payments

#### BR-03 — Annual Customer Churn

**Client requirement:** Identify customers who purchased in a given year but **did not place any orders in the following year**. Report churned customers year by year to track retention trends.

#### BR-10 — Sales Distribution by Payment Type

**Client requirement:** Group customer payments by **payment type** and analyze the distribution of sales across payment methods to understand preferences and inform financial or promotional strategies.

### 2.4 Promotion and Profitability

#### BR-09 — Buy One, Get One Free (BOGO) Simulation

**Client requirement:** Simulate the effect on **profit margin** of a hypothetical BOGO promotion applied **last year** to the **top 10 products by quantity sold**. Assume:

- The promotion **doubles the quantity sold** for these products.
- **Every second item** is sold at **zero price**.

### 2.5 Fulfillment and Customer Experience

#### BR-11 — Delivery Timeliness and Review Scores

**Client requirement:** Compare **average review scores** for orders delivered **on time** versus **late**.

#### BR-12 — Order Fulfillment Stage Durations

**Client requirement:** Calculate the **average elapsed time, in hours, for each stage** of the order fulfillment process.

### 2.6 Seller and Local-Market Performance

#### BR-14 — Highly Rated Sellers with Low Local Sales Share

**Client requirement:** Identify sellers meeting **both** conditions:

1. **Average review score > 4.5**.
2. **Less than 10% of their total sales** come from customers in the **same state as the seller**.

These sellers may represent missed local marketing opportunities.








