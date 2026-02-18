# Documentation

## Final Project Report

**📄 Complete Documentation:** [View Full Report on Google Docs](https://docs.google.com/document/d/1jkbtK3LNOrbsEqr9IhsTYEBhu1T8lW5lKxFoBwbdJRI/edit?pli=1&tab=t.0)

---

## Report Highlights

### Project Overview
- **Title:** Customer Churn Analysis & Retention Strategy Using E-Commerce Behavioral Data
- **Sector:** E-Commerce / Retail Analytics
- **Team:** Group 6
- **Dataset:** 50,000 customer records × 26 attributes
- **Churn Rate:** 28.9% (14,450 churned customers)

---

### Key Findings

#### Critical Churn Drivers
1. **Inactivity Risk:** High days since last purchase strongly correlates with churn
2. **Low Engagement:** Reduced login frequency and shorter sessions predict churn
3. **Cart Abandonment:** Higher abandonment rates (50.6% avg) among churned customers
4. **Service Issues:** High customer service calls indicate dissatisfaction
5. **Email Disengagement:** Lower email open rates reduce marketing effectiveness
6. **Purchase Behavior:** Customers with higher total purchases and LTV churn less

#### Financial Impact
- **Revenue at Risk:** $20.6M in lifetime value from churned customers
- **Retention Opportunity:** 3-5% churn reduction = 1,500-2,500 customers retained
- **Cost Efficiency:** Retention costs 5-10x less than acquisition

---

### Data Cleaning Summary

**Issues Resolved:**
- ✅ 53,286+ missing values imputed (4.26% of dataset)
- ✅ 23 data type conversions (text → numeric)
- ✅ Outliers handled (Age: 200 → realistic values)
- ✅ Range validation (percentages capped at 0-100)
- ✅ Negative values corrected (Total_Purchases)
- ✅ Binary conversion (Churned: 0/1 → Yes/No)

**Cleaning Techniques:**
- Median/mean imputation for numerical columns
- Average-based filling for percentage columns
- Rounding and formatting standardization
- Data type validation and conversion

---

### KPI Framework

#### Customer Engagement Metrics
- Login Frequency
- Session Duration Average
- Pages Per Session
- Email Open Rate
- Mobile App Usage

#### Purchase Behavior Metrics
- Total Purchases
- Average Order Value (AOV)
- Days Since Last Purchase
- Lifetime Value (LTV)

#### Risk Indicators
- Cart Abandonment Rate
- Customer Service Calls
- Returns Rate
- Discount Usage Rate

---

### Strategic Recommendations

#### 1. Re-Engagement Campaigns
**Target:** Customers inactive >30-60 days  
**Action:** Automated email/push notifications with personalized offers  
**Impact:** Recover customers before permanent churn  
**Feasibility:** High

#### 2. Cart Abandonment Recovery
**Target:** 50-75% abandonment segment  
**Action:** Reminder notifications, limited-time incentives, checkout optimization  
**Impact:** Convert lost carts into sales, 10-15% churn reduction  
**Feasibility:** Medium-High

#### 3. Service Quality Enhancement
**Target:** Customers with 6+ service calls (40.6% churn rate)  
**Action:** First-call resolution, proactive support, escalation tracking  
**Impact:** Reduce dissatisfaction-driven churn  
**Feasibility:** Medium

#### 4. Loyalty Program for High-LTV Customers
**Target:** Top-tier customers with high lifetime value  
**Action:** VIP membership, exclusive discounts, early product access  
**Impact:** Protect revenue and strengthen retention  
**Feasibility:** High

#### 5. Email Personalization Strategy
**Target:** Low email engagement customers  
**Action:** Behavioral triggers, product recommendations, personalized offers  
**Impact:** Improve engagement and repeat purchases  
**Feasibility:** High

---

### Analysis Methodology

#### Exploratory Data Analysis (EDA)
- **Trend Analysis:** Signup quarter vs churn patterns
- **Comparison Analysis:** Churned vs non-churned behavior
- **Distribution Analysis:** Age, LTV, engagement metrics
- **Correlation Analysis:** Churn drivers identification
- **Segmentation:** Country × Gender × Churn status (48 segments)

#### Statistical Insights
- Customers with high inactivity show 2.5x higher churn risk
- Youth segment (0-20 age) has 47.6% churn rate (nearly double average)
- USA market accounts for 35% of churned revenue ($7.2M)
- High cart abandonment (75-100%) correlates with 64.2% churn rate
- Customers with 15+ service calls have 70.3% churn rate

---

### Dashboard Components

#### Executive View
- Total customers: 50,000
- Churn rate: 28.9%
- Revenue at risk: $20.6M
- Geographic heat maps
- KPI cards and trend charts

#### Operational View
- Days since last purchase histogram
- Cart abandonment vs churn scatter plot
- Customer service calls distribution
- Engagement score correlations
- Segment-based churn tracking

#### Interactive Filters
- Country, City, Gender
- Signup Quarter
- Customer risk segments

---

### Project Limitations

- ❌ Cross-sectional data (no time-series tracking)
- ❌ Missing product category information
- ❌ No delivery experience or payment failure data
- ❌ Limited marketing engagement data (email only)
- ❌ Some unrealistic outliers in raw data
- ❌ Correlational insights (not causal)

---

### Future Scope

#### Predictive Analytics
- Build ML-based churn prediction model (Logistic Regression, Random Forest, XGBoost)
- Real-time churn alert system for high-risk customers
- Automated risk scoring dashboard

#### Advanced Analysis
- Cohort analysis by signup month and lifecycle stage
- A/B testing for retention campaigns
- Customer satisfaction and delivery experience integration
- Product category-level churn analysis

#### Business Integration
- Automated intervention triggers
- CRM system integration
- Real-time monitoring dashboards
- Continuous model retraining pipeline

---

### Team Contributions

| Team Member | Role | Responsibilities |
|-------------|------|------------------|
| **Tattva Rajput** | Report Lead | Dataset sourcing, cleaning checks, report writing |
| **Aryan Kumar** | Team Lead | KPI development, analysis, dashboard creation |
| **Dikshant Jangra** | PPT Lead | Dashboard checks, presentation, dataset sourcing |
| **Swagato Bauri** | Data Cleaning Lead | Data cleaning, analysis and KPI checks |
| **Yuvraj Chandravansi** | Documentation Lead | Logs, documentation, data cleaning, report checks |
| **Adityaraj Pal** | Data Sourcing | Dataset acquisition and validation |

---

### Technical Stack

**Tools Used:**
- Google Sheets (data cleaning, pivot tables, dashboard)
- ARRAYFORMULA functions for batch processing
- Pivot tables for aggregation and KPI calculation
- Conditional formatting and data validation
- Charts and visualizations

**Formulas Applied:**
- Median/mean imputation: `ARRAYFORMULA(IF(LEN(TRIM(...))=0, MEDIAN(...), ...))`
- Range capping: `IF(value>100, 100, IF(value<0, 0, value))`
- Data type conversion: `VALUE()`, `ROUND()`
- Binary transformation: `IF(value=1, "Yes", "No")`

---

## Document Structure

### Report Sections
1. **Executive Summary** - Key findings and recommendations
2. **Sector & Business Context** - E-commerce industry overview
3. **Problem Statement & Objectives** - Project scope and goals
4. **Data Description** - Dataset structure and data dictionary
5. **Data Cleaning & Preparation** - Cleaning methodology and transformations
6. **KPI & Metric Framework** - Business metrics and indicators
7. **Exploratory Data Analysis** - Trends, comparisons, distributions
8. **Advanced Analysis** - Root cause and correlation analysis
9. **Dashboard Design** - Visualization and interactivity
10. **Insights Summary** - 8-12 key findings
11. **Recommendations** - Actionable strategies with impact estimation
12. **Impact Estimation** - Financial and business value
13. **Limitations** - Data and methodology constraints
14. **Future Scope** - Next steps and enhancements
15. **Conclusion** - Project summary and outcomes
16. **Appendix** - Data dictionary, formulas, charts
17. **Contribution Matrix** - Team member roles

---

## Quick Reference

**📊 Dataset:** 50,000 customers × 26 attributes  
**🔴 Churn Rate:** 28.9% (14,450 customers)  
**💰 Revenue at Risk:** $20.6M lifetime value  
**📈 Key Metric:** Days Since Last Purchase (strongest churn predictor)  
**🎯 Target:** Reduce churn to 23% (industry benchmark)  
**💡 Top Recommendation:** Re-engagement campaigns for inactive customers  
**⚡ Quick Win:** Cart abandonment recovery (10-15% churn reduction potential)

---

**For complete analysis, methodology, formulas, and detailed insights:**  
👉 [**Access Full Report**](https://docs.google.com/document/d/1jkbtK3LNOrbsEqr9IhsTYEBhu1T8lW5lKxFoBwbdJRI/edit?pli=1&tab=t.0)
