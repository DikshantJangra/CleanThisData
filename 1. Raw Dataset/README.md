# Raw Dataset

## Purpose

This folder contains the original, unprocessed datasets used for analysis. These files remain unchanged throughout the project to maintain data integrity and enable reproducibility.

---

## Datasets

### 1. E-commerce Customer Churn Dataset (Primary)

**Filename:** `Ecommerce Customer Churn Dataset.csv`  
**Source:** [Kaggle - E-commerce Customer Behavior Dataset](https://www.kaggle.com/datasets/dhairyajeetsingh/ecommerce-customer-behavior-dataset/data)  
**Records:** 50,000 customers  
**Attributes:** 25 columns  
**Format:** CSV (Comma-Separated Values)  
**Size:** ~4.5 MB  
**Date Acquired:** 2024

#### Business Context

This dataset captures comprehensive customer behavior patterns for an e-commerce platform, designed to support churn prediction and customer retention strategies. Understanding customer churn is critical for e-commerce businesses as acquiring new customers costs 5-25x more than retaining existing ones.

#### Dataset Structure

| Category | Attributes | Description |
|----------|------------|-------------|
| **Demographics** | Age, Gender, Country, City | Customer profile information |
| **Membership** | Membership_Years, Signup_Quarter | Account tenure and registration period |
| **Engagement** | Login_Frequency, Session_Duration_Avg, Pages_Per_Session, Mobile_App_Usage | Platform interaction metrics |
| **Shopping Behavior** | Cart_Abandonment_Rate, Wishlist_Items, Total_Purchases, Average_Order_Value, Days_Since_Last_Purchase | Purchase patterns and intent signals |
| **Promotions** | Discount_Usage_Rate, Returns_Rate | Price sensitivity and product satisfaction |
| **Communication** | Email_Open_Rate, Customer_Service_Calls, Product_Reviews_Written, Social_Media_Engagement_Score | Customer communication preferences |
| **Financial** | Lifetime_Value, Credit_Balance, Payment_Method_Diversity | Monetary value and payment behavior |
| **Target Variable** | Churned | Binary indicator (0 = Active, 1 = Churned) |

#### Data Characteristics

**Numerical Features (20):**
- Continuous: Age, Session_Duration_Avg, Average_Order_Value, Lifetime_Value, etc.
- Discrete: Login_Frequency, Total_Purchases, Customer_Service_Calls, etc.
- Percentages: Cart_Abandonment_Rate, Discount_Usage_Rate, Email_Open_Rate, etc.

**Categorical Features (5):**
- Binary: Gender (Male/Female), Churned (0/1)
- Nominal: Country, City, Signup_Quarter

#### Known Data Quality Issues

Based on preliminary inspection, the following issues require attention during cleaning:

1. **Missing Values:** Present across multiple columns (Age, Pages_Per_Session, Returns_Rate, etc.)
2. **Data Type Inconsistencies:** Some numerical fields may contain non-numeric values
3. **Outliers:** Potential extreme values in financial and behavioral metrics
4. **Duplicate Records:** Requires validation for unique customer identification
5. **Range Validation:** Percentage fields should be bounded [0-100], rates should be non-negative

#### Use Cases

- **Churn Prediction:** Build machine learning models to identify at-risk customers
- **Customer Segmentation:** Cluster analysis for targeted marketing campaigns
- **Lifetime Value Modeling:** Predict future customer value for resource allocation
- **Behavioral Analysis:** Understand engagement patterns and conversion drivers
- **A/B Testing:** Baseline metrics for experimental design

---

### 2. Boeing Historical Data (Secondary)

**Filename:** Pending  
**Source:** [Kaggle - Boeing Historical Airplane Orders & Deliveries](https://www.kaggle.com/datasets/nurielreuven/boeing-historical-airplane-orders-deliveries)  
**Status:** Not yet ingested  
**Expected Format:** CSV/Excel  

#### Planned Analysis

- Historical trend analysis of aircraft orders and deliveries
- Supply chain performance metrics
- Market demand forecasting
- Cross-dataset comparative analysis (if applicable)

---

## Data Pipeline

```
Raw Dataset → Cleaned Dataset → Calculations & Pivot Tables → Dashboard → Presentation
```

---

## Next Steps

1. **Data Profiling:** Generate statistical summary of all variables
2. **Quality Assessment:** Identify missing values, outliers, and anomalies
3. **Data Cleaning:** Apply transformations and save to Cleaned Dataset folder
4. **KPI Calculation:** Build metrics in Calculation & Pivot Table folder


