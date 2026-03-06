# Customer Segmentation using RFM Analysis

## Project Overview

Customer segmentation is a key technique in data analytics and marketing. It helps businesses understand customer behavior and design targeted marketing strategies.

In this project, **RFM Analysis** was used to segment customers based on their purchasing behavior using the **Online Retail Dataset**.

RFM stands for:

* **Recency (R):** How recently a customer made a purchase
* **Frequency (F):** How often a customer makes purchases
* **Monetary (M):** How much money a customer spends

By analyzing these three metrics, customers can be grouped into meaningful segments such as **Champions**, **Loyal Customers**, **At Risk**, and **Lost Customers**.
These segments help businesses apply different marketing strategies for each customer group.

---

## Dataset

The dataset used in this project is the **Online Retail Dataset**, which contains transactional data from a UK-based online retail store.

The dataset includes information such as:

* Invoice number
* Product description
* Quantity purchased
* Invoice date
* Unit price
* Customer ID
* Country

This dataset is commonly used for **customer behavior analysis and segmentation tasks**.

---

## Project Steps

### 1. Data Loading

The dataset was loaded using **Pandas** for further analysis.

### 2. Data Cleaning

Data cleaning was performed to ensure reliable analysis.

The following steps were applied:

* Removing missing `CustomerID` values
* Removing negative or zero quantities
* Creating a new column called **TotalPrice**

```
TotalPrice = Quantity * UnitPrice
```

### 3. Feature Engineering

New features were created to perform **RFM Analysis**.

#### Recency

Calculated as the number of days since the customer's last purchase.

#### Frequency

Calculated as the number of transactions made by each customer.

#### Monetary

Calculated as the total amount spent by each customer.

These three metrics form the **RFM table**.

---

## RFM Scoring

Each customer was assigned a score from **1 to 5** for each RFM metric.

* **Recency Score:** lower recency → higher score
* **Frequency Score:** more purchases → higher score
* **Monetary Score:** higher spending → higher score

These scores help standardize customers for segmentation.

---

## Customer Segmentation

Customers were grouped into segments based on their RFM scores.

The following segments were identified:

### Champions

Customers with high Recency, Frequency, and Monetary values.

**Characteristics**

* Very active customers
* High purchase frequency
* High spending

**Marketing Strategy**

* VIP loyalty programs
* Exclusive offers

---

### Loyal Customers

Customers who purchase frequently.

**Characteristics**

* Regular buyers
* Strong brand engagement

**Marketing Strategy**

* Reward programs
* Special discounts

---

### Big Spenders

Customers who spend large amounts but may not purchase frequently.

**Marketing Strategy**

* Premium offers
* Upselling opportunities

---

### New Customers

Customers who recently made their first purchases.

**Marketing Strategy**

* Welcome campaigns
* First-time purchase incentives

---

### At Risk Customers

Customers who have not purchased recently.

**Marketing Strategy**

* Re-engagement campaigns
* Personalized promotions

---

### Lost Customers

Customers with very low RFM scores who have not interacted with the business for a long time.

**Marketing Strategy**

* Strong discount campaigns
* Win-back strategies

---

## Data Visualization

To better understand the results, several visualizations were created.

### Customer Segment Distribution

A **Pie Chart** was used to show how customers are distributed across different segments.

### Segment Count

A **Bar Chart** was used to visualize the number of customers in each segment.

### RFM Heatmap

A **Heatmap** was created to show the relationship between Recency, Frequency, and Monetary scores across customer segments.

These visualizations help highlight patterns in customer behavior.

---

## Tools & Libraries

The following tools were used:

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* GoogleColab Notebook

---

## Key Insights

* A large number of customers fall into the **At Risk** category, indicating an opportunity for re-engagement campaigns.
* The presence of **Champions customers** shows strong loyalty and high-value customer relationships.
* Different segments require different marketing strategies to maximize retention and revenue.

---




