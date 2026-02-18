# E-commerce Customer Churn Analysis Project

## Overview
Complete end-to-end data analysis project analyzing 50,000 e-commerce customer records to identify churn patterns, predict at-risk customers, and provide actionable retention strategies. The project encompasses data cleaning, statistical analysis, KPI development, interactive dashboards, and executive reporting.

---

## Project Structure
```
CleanThisData/
├── 1. Raw Dataset/               # Original dataset (50,000 records, 25 columns)
├── 2. Cleaned Dataset/           # 100% validated data (26 columns with unique ID)
├── 3. Calculation & Pivot table/ # 11 pivot tables, 5 KPIs, statistical analysis
├── 4. Dashboard/                 # 25+ visualizations, executive KPI cards
├── 5. Documentation/             # Technical documentation and methodology
└── 6. Presentation/              # Executive presentation (PDF deliverable)
```

---

## Dataset

### E-commerce Customer Churn Dataset
**Source:** [Kaggle - E-commerce Customer Behavior Dataset](https://www.kaggle.com/datasets/dhairyajeetsingh/ecommerce-customer-behavior-dataset/data)

**Specifications:**
- **Records:** 50,000 customers
- **Attributes:** 25 columns (26 after cleaning with unique identifier)
- **Format:** CSV
- **Size:** 5.8 MB
- **Date Acquired:** 2024

**Key Features:**
- **Demographics:** Age, Gender, Country, City
- **Membership:** Membership_Years, Signup_Quarter
- **Engagement:** Login_Frequency, Session_Duration_Avg, Pages_Per_Session, Mobile_App_Usage
- **Shopping Behavior:** Cart_Abandonment_Rate, Wishlist_Items, Total_Purchases, Average_Order_Value, Days_Since_Last_Purchase
- **Promotions:** Discount_Usage_Rate, Returns_Rate
- **Communication:** Email_Open_Rate, Customer_Service_Calls, Product_Reviews_Written, Social_Media_Engagement_Score
- **Financial:** Lifetime_Value, Credit_Balance, Payment_Method_Diversity
- **Target Variable:** Churned (Binary: 0 = Active, 1 = Churned)

---

## Project Results

### Key Findings

**Churn Metrics:**
- **Total Churned Customers:** 14,450 (28.9% churn rate)
- **Active Customers:** 35,550 (71.1% retention rate)
- **Revenue at Risk:** $20,597,365.76 (28.6% of total revenue)
- **Total Revenue Analyzed:** $72,031,314.60

**Critical Churn Predictors:**
1. **Cart Abandonment (75-100%):** 64.2% churn rate
2. **Customer Service Calls (15+):** 70.3% churn rate
3. **Days Since Last Purchase (186+):** 63.6% churn rate
4. **Age Group (0-20 years):** 47.6% churn rate
5. **Customer Service Calls (12-14):** 55.8% churn rate

**Geographic Insights:**
- **Highest Risk Country:** USA (5,056 churned customers, $7.2M lost revenue)
- **Best Retention:** France (27.3% churn rate)
- **Countries Analyzed:** 8 (USA, UK, Canada, Germany, Australia, France, India, Japan)

**Financial Impact:**
- **Average Order Value:** $123.12 overall ($118.38 active vs $134.76 churned)
- **Average Purchases:** 13.13 overall (13.84 active vs 11.37 churned)
- **Customer Lifetime Value:** $1,440.62 average ($1,446.81 active vs $1,425.42 churned)

**Engagement Patterns:**
- **Average Session Duration:** 27.60 minutes
- **Mobile App Usage:** 19.29% average
- **Seasonal Peak:** Q4 (30.2% of total purchases - 198,134 purchases)
- **Average Returns Rate:** 6.68%

---

## Data Quality Assessment

### Cleaning Results
| Issue Type | Status | Resolution |
|------------|--------|------------|
| **Missing Values** | ✅ Resolved | 53,286 missing values (4.26%) imputed across 15 columns using mean/median/conditional average |
| **Data Type Errors** | ✅ Resolved | 23 columns converted from text to numeric with precision rounding |
| **Out-of-Range Values** | ✅ Resolved | Percentage fields capped at [0-100], negative values corrected |
| **Outliers** | ✅ Resolved | Unrealistic ages, dirty decimals, and anomalies corrected |
| **Duplicate Records** | ✅ Validated | No duplicates found |
| **Unique Identifiers** | ✅ Added | Rec_No. column added (1-50,000) |

**Data Quality Score:** 100% Complete, Validated, and Production-Ready

---

## Analysis Deliverables

### Completed Outputs

**1. Cleaned Dataset**
- 50,000 records, 26 columns
- 0% missing values
- All data types validated
- Formula-based cleaning using Google Sheets ARRAYFORMULA

**2. Statistical Analysis**
- 11 comprehensive pivot tables
- 5 primary KPIs calculated
- Multi-dimensional analysis (country, gender, age, tenure, behavior)
- Churn predictor ranking by impact

**3. Interactive Dashboard**
- 7 executive KPI cards
- 25+ visualizations (charts, heat maps, trend lines)
- Geographic churn distribution
- Behavioral churn indicators
- Revenue and financial breakdowns
- Engagement and retention metrics

**4. Executive Presentation**
- 10-15 slide PDF presentation
- Key findings and business impact
- Strategic recommendations (15+ actionable items)
- Implementation roadmap
- Success metrics and ROI projections

### Technical Stack
- **Data Processing:** Google Sheets, CSV
- **Analysis:** Pivot tables, Statistical aggregations, ARRAYFORMULA functions
- **Visualization:** Charts, KPI cards, Conditional formatting
- **Reporting:** PDF presentation, Technical documentation

---

## Strategic Recommendations

### Immediate Actions (0-30 days)
1. **Cart Recovery Campaigns:** Target 50-75% abandonment segment (26.2% churn risk)
2. **Purchase Recency Outreach:** Proactive engagement at 31-day milestone (32.1% churn risk)
3. **Service Quality Task Force:** Reduce need for 6+ service calls (40.6% churn risk)
4. **Youth Engagement Pilot:** Specialized retention programs for 0-20 age group (47.6% churn)

### Short-term Initiatives (1-3 months)
1. **Predictive Churn Scoring:** Deploy ML model using identified risk factors
2. **USA Market Strategy:** Priority retention program ($7.2M revenue at risk)
3. **Mobile App Optimization:** Increase usage from 19.29% baseline
4. **Engagement Tier Programs:** Leverage social media engagement correlation

### Long-term Strategy (3-6 months)
1. **Automated Churn Alerts:** Real-time risk notifications
2. **Comprehensive Retention Playbook:** Scalable intervention framework
3. **Continuous Monitoring:** Dashboard refresh and KPI tracking
4. **A/B Testing Framework:** Validate retention program effectiveness

### Expected Outcomes
- **Churn Reduction:** From 28.9% to 23% (industry benchmark)
- **Revenue Retention:** $10M+ of at-risk lifetime value
- **Cart Abandonment:** 15% reduction
- **Service Call Volume:** 25% reduction in high-volume calls
- **Youth Retention:** 20% improvement in 0-20 age segment

---

## Project Files

### 1. Raw Dataset
- `Ecommerce Customer Churn Dataset.csv` (50,000 records, 25 columns, 5.8 MB)
- `Ecommerce Customer Behavior Dataset.png` (Dataset preview image)
- `README.md` (Detailed dataset documentation)

### 2. Cleaned Dataset
- `G-6 DVA Capstone Cleaned Dataset.csv` (50,000 records, 26 columns, 100% complete)
- `README.md` (Cleaning methodology and validation results)

### 3. Calculation & Pivot Table
- `G-6 DVA Capstone Analysis & Working.csv` (11 pivot tables, 5 KPIs)
- `README.md` (Statistical analysis and insights)

### 4. Dashboard
- `G-6 DVA Capstone Dashboard.csv` (25+ visualizations, KPI cards)
- `README.md` (Dashboard components and usage guidelines)

### 5. Documentation
- `README.md` (Project documentation)

### 6. Presentation
- `DVA_Project_Presentation.pdf` (Executive presentation)
- `README.md` (Presentation structure and key messages)

---

## Project Status
- **Status:** ✅ Complete
- **Last Updated:** February 18, 2026
- **Version:** 1.0
- **Data Quality:** 100% Complete and Validated
- **Business Impact:** $20.6M revenue retention opportunity identified

---

## Quick Start

1. **Review Raw Data:** Start with `1. Raw Dataset/README.md` for dataset overview
2. **Understand Cleaning:** Check `2. Cleaned Dataset/README.md` for data quality details
3. **Explore Analysis:** Review `3. Calculation & Pivot table/README.md` for key insights
4. **View Dashboard:** Access `4. Dashboard/README.md` for visualizations
5. **Executive Summary:** Open `6. Presentation/DVA_Project_Presentation.pdf` for stakeholder presentation

---

*E-commerce Customer Churn Analysis - Data-Driven Retention Strategy*
