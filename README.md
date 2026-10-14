# 🛍️ RetailPulse: Retail Analytics & Consumer Insights
### End-to-End Data Analytics Project using Python, PostgreSQL, SQL & Power BI

## 📌 Project Overview

This project analyzes customer shopping behavior using transactional data from **3,900 purchases** across multiple product categories.

The objective is to transform raw customer shopping data into actionable business intelligence by analyzing:

- Customer demographics
- Purchasing patterns
- Product preferences
- Customer loyalty
- Subscription behavior
- Discount usage
- Shipping preferences
- Review ratings
- Revenue contribution across customer segments

The project follows an end-to-end data analytics workflow, starting with data preparation in Python, followed by business analysis using PostgreSQL and SQL, and finally visualization through an interactive Power BI dashboard.

---

## 🎯 Business Problem

A leading retail company wants to better understand its customers' shopping behavior in order to improve sales, customer satisfaction, and long-term loyalty.

The central business question is:

> **How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?**

---

## 📊 Dataset

The dataset contains **3,900 customer purchase records** and **18 columns**.

### Dataset Features

| Category | Features |
|---|---|
| Customer Demographics | Age, Gender, Location, Subscription Status |
| Purchase Details | Item Purchased, Category, Purchase Amount, Season, Size, Color |
| Shopping Behavior | Discount Applied, Previous Purchases, Frequency of Purchases |
| Customer Feedback | Review Rating |
| Fulfillment | Shipping Type |

There were **37 missing values in the Review Rating column**, which were handled during data preparation.

---

## Project Architecture

```text
Raw Customer Data
       ↓
Python — Data Cleaning & EDA
       ↓
Feature Engineering
       ↓
PostgreSQL Database
       ↓
SQL Business Analysis
       ↓
Power BI Dashboard
       ↓
Business Insights & Recommendations
```

---

# 🔄 Project Workflow

## 1. Data Preparation & Exploratory Data Analysis — Python

The first stage involved importing, exploring, cleaning, and transforming the raw dataset.

### Data Cleaning

- Checked for missing values
- Handled missing review ratings
- Standardized column names
- Checked data consistency
- Removed redundant information

The missing `Review Rating` values were imputed using the **median rating of each product category**.

### Feature Engineering

Additional analytical features were created:

- `age_group` — customer ages grouped into meaningful categories
- `purchase_frequency_days` — purchase frequency converted into a numerical day-based measure

`discount_applied` and `promo_code_used` were checked for redundancy, after which `promo_code_used` was dropped.

---

# 🗄️ 2. PostgreSQL & SQL Business Analysis

The cleaned dataset was loaded into **PostgreSQL** for structured business analysis.

### Business Questions

1. Revenue by Gender
2. High-Spending Discount Users
3. Top 5 Products by Rating
4. Shipping Type Comparison
5. Subscribers vs. Non-Subscribers
6. Discount-Dependent Products
7. Customer Segmentation
8. Top 3 Products per Category
9. Repeat Buyers & Subscriptions
10. Revenue by Age Group

---

# 📈 3. Power BI Dashboard

The cleaned and analyzed data was visualized using an interactive **Power BI Customer Behavior Dashboard**.


### Dashboard KPIs

The dashboard currently highlights:

- **3.9K** — Number of Customers/Purchases represented in the dashboard
- **$59.76** — Average Purchase Amount
- **3.75** — Average Review Rating
- **27%** — Customers with an active subscription
- **73%** — Customers without a subscription

### Dashboard Visualizations

The dashboard provides interactive analysis of:

- Customer subscription status
- Gender
- Product category
- Shipping type
- Revenue by category
- Sales by category
- Revenue by age group
- Sales by age group

### Interactive Filters

Users can filter the dashboard by:

- Subscription Status
- Gender
- Category
- Shipping Type

This allows stakeholders to explore customer behavior from different demographic and purchasing perspectives.

---

# 💡 Business Recommendations

### 1. Boost Subscriptions

Promote exclusive benefits and incentives for subscribers to encourage customers to adopt subscription plans.

### 2. Develop Customer Loyalty Programs

Reward repeat customers and create strategies that encourage customers to move from the **New → Returning → Loyal** stages.

### 3. Review Discount Strategy

Analyze discount-dependent products carefully to balance increased sales with margin considerations.

### 4. Strengthen Product Positioning

Use highly rated and frequently purchased products in marketing campaigns and product recommendations.

### 5. Targeted Marketing

Use demographic and behavioral insights to develop targeted campaigns for high-revenue customer groups.

---

# 🛠️ Tech Stack

### Programming & Data Analysis
- Python
- Pandas
- NumPy
- Jupyter Notebook

### Database & SQL
- PostgreSQL
- SQL

### Visualization
- Microsoft Power BI
- DAX

### Version Control
- Git
- GitHub

---


# 🚀 How to Run the Project

## Step 1 — Clone the Repository

```bash
git clone  https://github.com/SafaMansoor/Customer-behavior-analysis.git
cd customer-shopping-behavior-analysis
```

## Step 2 — Install Python Dependencies

```bash
pip install pandas numpy jupyter sqlalchemy psycopg2-binary
```

## Step 3 — Run the Python Notebook

Open:

```text
notebooks/Customer_Shopping_Behavior_Analysis.ipynb
```

The notebook contains:

- Data import
- Data exploration
- Data cleaning
- Feature engineering
- PostgreSQL connection
- Data loading

## Step 4 — Run SQL Analysis

Open:

```text
sql/customer_behavior_sql_queries.sql
```

Run the queries against the PostgreSQL database.

## Step 5 — Open Power BI

Open:

```text
powerbi/customer_behavior_dashboard.pbix
```

Connect Power BI to PostgreSQL and refresh the dataset if required.

---

# 🎓 Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Python & Pandas
- PostgreSQL
- SQL Business Analysis
- Customer Segmentation
- Revenue Analysis
- Product Analysis
- Discount Analysis
- Subscription Analysis
- Power BI Dashboard Development
- Data Visualization
- Business Storytelling

---

# 🔮 Future Improvements

Potential extensions include:

- Customer Lifetime Value (CLV) analysis
- RFM customer segmentation
- Customer churn prediction
- Purchase propensity modeling
- Recommendation systems
- Sales forecasting
- Customer clustering using machine learning
- Marketing campaign response prediction



