# Customer Segmentation using RFM Analysis

## Problem Statement

A UK-based online retailer selling unique all-occasion gifts lacks a structured understanding of customer value and purchasing behaviour. The objective of this project is to identify high-value customers, understand purchasing patterns, and develop actionable business recommendations using RFM (Recency, Frequency, Monetary) analysis.

## Repository Contents

* `rfm_analysis.ipynb` – Complete analysis notebook
* `README.md` – Project overview, methodology, and key findings

## Dataset

The analysis uses the Online Retail dataset containing transactional records from a UK-based online gift retailer.

Dataset characteristics:

* 541,909 transactions
* 4,372 customers after cleaning
* Transaction history from December 2010 to December 2011

## Project Objectives

* Clean and prepare transactional data for analysis
* Explore customer purchasing behaviour
* Calculate Recency, Frequency, and Monetary (RFM) metrics
* Segment customers based on RFM characteristics
* Identify high-value and at-risk customer groups
* Develop data-driven business recommendations

## Methodology

### 1. Data Cleaning

* Removed records with missing Customer IDs
* Removed cancelled transactions
* Removed returns and negative quantities
* Removed internal adjustment transactions
* Investigated and removed wholesale customer outliers

### 2. Exploratory Data Analysis

Performed exploratory analysis to understand:

* Transaction patterns
* Customer purchase behaviour
* Revenue distribution
* Data quality issues

### 3. RFM Analysis

Calculated:

* **Recency** – Days since last purchase
* **Frequency** – Number of purchases
* **Monetary** – Total customer spend

Customers were then assigned RFM scores ranging from 1 to 5.

### 4. Customer Segmentation

Traditional RFM segments were combined with dedicated one-time customer segments.

One-time customers represented approximately **35% of all customers**, making them too significant to be grouped into a generic category.

The following segments were created:

* Champions
* Loyal Customers
* Potential Loyalists
* Big Ticket Buyers
* At Risk
* Hibernating
* Promising
* Need Nurturing
* New Customers
* Recent One-Time Customers
* Lapsed One-Time Customers

## Key Findings

* Approximately **35% of customers** made only a single purchase.
* Champions represented the most valuable customer segment and generated the highest revenue.
* Potential Loyalists accounted for **11.3% of customers** and were identified as the highest-priority growth opportunity.
* At Risk customers previously demonstrated strong purchasing behaviour but showed declining engagement.
* Dedicated one-time customer segments reduced the proportion of unclassified customers from approximately **11.5% to 1.3%**.

## Business Recommendations

### 1. Target Potential Loyalists

Potential Loyalists should be the primary target for marketing campaigns due to their recent engagement, repeat purchase behaviour, and significant customer base.

### 2. Retain Champions

Champions generate the highest revenue and should be retained through loyalty programs, personalised promotions, and exclusive offers.

### 3. Re-engage At Risk Customers

At Risk customers have historically purchased frequently and spent significantly but have not returned recently. Targeted win-back campaigns can help recover valuable customers.

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Conclusion

RFM analysis successfully identified distinct customer segments and highlighted opportunities for customer retention, revenue growth, and targeted marketing. The resulting segmentation framework provides actionable insights that can support data-driven decision making and improve customer lifetime value.

