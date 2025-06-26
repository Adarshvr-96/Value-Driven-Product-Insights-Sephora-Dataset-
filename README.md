#  Exploratory Data Analysis (EDA) – Sephora Product Dataset

This analysis explores Sephora's product listings dataset to uncover patterns related to customer satisfaction, product pricing, and value performance.

---

## 📌 Objective

To clean, analyze, and derive insights from Sephora product data using Python (Pandas, Seaborn, Matplotlib). The project highlights product performance, customer trends, and value-driven buying behavior.

---

## Dataset Overview

- *brand*: Name of the product brand  
- *category*: Product category type  
- *name*: Product title or short description  
- *price*: Selling price (USD)  
- *value_price*: Original value or market price (USD)  
- *rating*: Customer rating (1 to 5)  
- *number_of_reviews*: Review count per product  
- *love*: Like count per product  
- *best_value_score*: Engineered column (value_price / price) to show how much value the product gives

---

##  Data Cleaning Steps

- Removed duplicate records (by brand + name + category)
- Dropped irrelevant columns like how_to_use, ingredients, options, etc.
- Converted price-related fields to numeric
- Handled missing values in rating, value_price, and reviews

---

##  Feature Engineering

- *Best Value Score* = value_price / price  
    → Helps identify how much value customer gets per dollar  
- *Composite Score* = Custom score combining rating, reviews, and likes  
    → Used to rank products by both quality and popularity  
- *Full Name* = brand + " - " + name  
    → Easier identification in plots and dashboards

---

##  Visuals & Insights

### 1. Best Value Score vs. Rating (Scatterplot)
- Customers are willing to pay more for high-quality products
- High ratings cluster in low value-score zones

### 2. Top 10 Products by Composite Score
- Sephora Collection dominates top spots
- Value + engagement = performance

### 3. Top 10 Brands by Average Rating
- Shows which brands deliver consistent quality

### 4. Product Rating Distribution
- Most products rated between 4.0 to 5.0

### 5. Top Categories by Avg Best Value Score
- Gift Sets and Curls & Coils offer great bang for buck

---

##  Key Metrics (KPIs)

| KPI                  | Value       |
|----------------------|-------------|
| Total Products       | 9,179       |
| Avg Rating           | ~4.1        |
| Avg Price            | ~$15.06     |
| Avg Best Value Score | ~1.2        |
| Most Reviewed Product| Sephora Collection Set |

---

##  Business Relevance

- *Pricing Strategy*: Value score helps identify underpriced winners  
- *Marketing Targets*: Brands with high composite score are good for campaigns  
- *Product Decisions*: Categories with low value or rating can be improved  

---

## 📁 Project Files
    Visuals and Python Code
    https://github.com/Adarshvr-96/Value-Driven-Product-Insights-Sephora-Dataset-/blob/main/sephoraEDA.ipynb 
