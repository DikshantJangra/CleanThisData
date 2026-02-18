# Calculation & Pivot Table

## Overview

This folder contains comprehensive statistical analysis, KPI calculations, and pivot table aggregations derived from the cleaned e-commerce customer churn dataset. All metrics are production-ready for dashboard visualization and executive reporting.

---

## Files

**Filename:** `G-6 DVA Capstone Analysis & Working.csv`  
**Source Data:** Cleaned Ecommerce Customer Churn Dataset (50,000 records)  
**Analysis Date:** 2024  
**Format:** CSV with multiple pivot tables and KPI calculations

---

## Key Performance Indicators (KPIs)

### Business Metrics Summary

| KPI | Value | Insight |
|-----|-------|---------|
| **Total Churned Customers** | 14,450 | 28.9% churn rate |
| **Average Order Value** | $123.12 | Overall customer spending |
| **Highest Churn Country** | USA | Geographic risk concentration |
| **Average Returns Rate** | 6.68% | Product satisfaction indicator |
| **Highest Performing Quarter** | Q4 | Seasonal performance peak |

### Financial Impact

| Metric | Active Customers | Churned Customers | Total |
|--------|------------------|-------------------|-------|
| **Customer Count** | 35,550 (71.1%) | 14,450 (28.9%) | 50,000 |
| **Lifetime Value** | $51,433,948.84 | $20,597,365.76 | $72,031,314.60 |
| **Avg Order Value** | $118.38 | $134.76 | $123.12 |
| **Avg Total Purchases** | 13.84 | 11.37 | 13.13 |

**Key Finding:** Churned customers had higher AOV ($134.76 vs $118.38) but fewer total purchases (11.37 vs 13.84), suggesting quality over frequency issues.

---

## Pivot Table Analysis

### 1. Churn Rate by Gender

| Gender | Active | Churned | Total | Churn Rate |
|--------|--------|---------|-------|------------|
| Female | 17,839 | 7,277 | 25,116 | 29.0% |
| Male | 17,067 | 6,880 | 23,947 | 28.7% |
| Other | 644 | 293 | 937 | 31.3% |
| **Total** | **35,550** | **14,450** | **50,000** | **28.9%** |

**Insight:** Gender shows minimal impact on churn (29.0% vs 28.7% vs 31.3%)

### 2. Churn Rate by Country

| Country | Active | Churned | Total | Churn Rate |
|---------|--------|---------|-------|------------|
| USA | 12,328 | 5,056 | 17,384 | 29.1% |
| UK | 5,365 | 2,169 | 7,534 | 28.8% |
| Canada | 4,255 | 1,768 | 6,023 | 29.4% |
| Germany | 3,505 | 1,420 | 4,925 | 28.8% |
| Australia | 2,847 | 1,214 | 4,061 | 29.9% |
| France | 2,918 | 1,095 | 4,013 | 27.3% |
| India | 2,493 | 1,019 | 3,512 | 29.0% |
| Japan | 1,839 | 709 | 2,548 | 27.8% |
| **Total** | **35,550** | **14,450** | **50,000** | **28.9%** |

**Insight:** USA represents largest customer base (34.8%) and highest absolute churn (5,056 customers). France and Japan show lowest churn rates (~27-28%).

### 3. Country-Wise Revenue Impact

| Country | Active Revenue | Churned Revenue | Total Revenue | Revenue at Risk |
|---------|----------------|-----------------|---------------|-----------------|
| USA | $17,735,199.58 | $7,226,902.82 | $24,962,102.40 | 29.0% |
| UK | $7,788,087.56 | $3,036,151.74 | $10,824,239.30 | 28.1% |
| Canada | $6,054,325.81 | $2,541,724.82 | $8,596,050.63 | 29.6% |
| Germany | $5,130,360.61 | $1,999,443.33 | $7,129,803.94 | 28.0% |
| Australia | $4,154,664.92 | $1,706,023.16 | $5,860,688.08 | 29.1% |
| France | $4,260,784.85 | $1,564,217.03 | $5,825,001.88 | 26.9% |
| India | $3,644,834.00 | $1,476,091.06 | $5,120,925.06 | 28.8% |
| Japan | $2,665,691.51 | $1,046,811.80 | $3,712,503.31 | 28.2% |
| **Total** | **$51,433,948.84** | **$20,597,365.76** | **$72,031,314.60** | **28.6%** |

**Critical Insight:** $20.6M in lifetime value lost to churn, with USA accounting for $7.2M (35% of total churn revenue).

### 4. Lifetime Value by Segment (Country × Gender)

**Top 5 Segments by Active Customer LTV:**

| Rank | Country | Gender | Active LTV | Avg LTV per Customer |
|------|---------|--------|------------|---------------------|
| 1 | USA | Female | $8,861,292.75 | $1,443.21 |
| 2 | USA | Male | $8,541,573.88 | $1,433.15 |
| 3 | UK | Female | $3,869,032.20 | $1,436.17 |
| 4 | UK | Male | $3,749,868.23 | $1,465.36 |
| 5 | Canada | Female | $3,020,590.97 | $1,438.38 |

**Insight:** Average LTV per active customer ($1,446.81) is slightly higher than churned customers ($1,425.42), indicating churn affects all value segments.

### 5. Churn by Membership Tenure

| Tenure (Years) | Active % | Churned % | Overall % |
|----------------|----------|-----------|-----------|
| 0 - 2 | 37.53% | 36.90% | 37.35% |
| 2 - 4 | 36.22% | 37.12% | 36.48% |
| 4 - 6 | 16.74% | 16.71% | 16.73% |
| 6 - 8 | 6.32% | 6.17% | 6.28% |
| 8 - 10 | 3.19% | 3.09% | 3.16% |

**Insight:** Churn distribution mirrors overall tenure distribution—no significant tenure-based churn pattern detected.

### 6. Days Since Last Purchase Analysis

| Days Range | Active | Churned | Total | Churn Rate |
|------------|--------|---------|-------|------------|
| 0 - 30 | 24,724 | 8,384 | 33,108 | 25.3% |
| 31 - 61 | 7,493 | 3,537 | 11,030 | 32.1% |
| 62 - 92 | 2,272 | 1,461 | 3,733 | 39.1% |
| 93 - 123 | 730 | 616 | 1,346 | 45.8% |
| 124 - 154 | 219 | 283 | 502 | 56.4% |
| 155 - 185 | 76 | 106 | 182 | 58.2% |
| 186+ | 36 | 63 | 99 | 63.6% |

**Critical Finding:** Churn rate increases dramatically with purchase recency—from 25.3% (0-30 days) to 63.6% (186+ days). Strong predictor of churn risk.

### 7. Cart Abandonment vs Churn

| Abandonment Rate | Active | Churned | Total | Churn Rate |
|------------------|--------|---------|-------|------------|
| 0 - 25% | 1,381 | 233 | 1,614 | 14.4% |
| 25 - 50% | 11,514 | 2,778 | 14,292 | 19.4% |
| 50 - 75% | 20,303 | 7,212 | 27,515 | 26.2% |
| 75 - 100% | 2,352 | 4,227 | 6,579 | 64.2% |

**Critical Finding:** Customers with 75-100% cart abandonment have 64.2% churn rate vs 14.4% for low abandoners. Strong churn predictor.

### 8. Customer Service Calls vs Churn

| Call Range | Active | Churned | Total | Churn Rate |
|------------|--------|---------|-------|------------|
| 0 - 2 | 4,799 | 656 | 5,455 | 12.0% |
| 3 - 5 | 16,584 | 3,181 | 19,765 | 16.1% |
| 6 - 8 | 10,369 | 7,080 | 17,449 | 40.6% |
| 9 - 11 | 3,290 | 2,856 | 6,146 | 46.5% |
| 12 - 14 | 475 | 599 | 1,074 | 55.8% |
| 15+ | 33 | 78 | 111 | 70.3% |

**Critical Finding:** Churn rate escalates from 12% (0-2 calls) to 70.3% (15+ calls). High service call volume indicates dissatisfaction and churn risk.

### 9. Total Purchases by Signup Quarter

| Quarter | Total Purchases | % of Total |
|---------|-----------------|------------|
| Q4 | 198,134 | 30.2% |
| Q3 | 153,967 | 23.5% |
| Q1 | 152,319 | 23.2% |
| Q2 | 152,020 | 23.2% |
| **Total** | **656,440** | **100%** |

**Insight:** Q4 shows 30% higher purchase volume than other quarters—likely holiday season impact.

### 10. Churn Rate by Age Group

| Age Group | Active | Churned | Total | Churn Rate |
|-----------|--------|---------|-------|------------|
| 0 - 20 | 1,657 | 1,505 | 3,162 | 47.6% |
| 20 - 40 | 18,645 | 7,638 | 26,283 | 29.1% |
| 40 - 60 | 14,083 | 4,880 | 18,963 | 25.7% |
| 60 - 80 | 1,149 | 423 | 1,572 | 26.9% |
| 100+ | 16 | 4 | 20 | 20.0% |

**Critical Finding:** Youngest customers (0-20) have 47.6% churn rate—nearly double the overall average. Age is a significant churn factor.

### 11. Engagement Score vs App Usage

| Social Media Score | Avg Session Duration (min) | Avg Mobile App Usage (%) |
|--------------------|---------------------------|-------------------------|
| 0 - 20 | 21.18 | 14.19 |
| 20 - 40 | 27.19 | 18.99 |
| 40 - 60 | 33.73 | 24.20 |
| 60 - 80 | 40.99 | 29.75 |
| 80 - 100 | 49.17 | 35.94 |
| **Overall** | **27.60** | **19.29** |

**Insight:** Strong positive correlation between social media engagement, session duration, and mobile app usage. High engagement customers spend 2.3x more time on platform.

---

## Statistical Summary

### Churn Predictors (Ranked by Impact)

| Rank | Factor | Impact Level | Evidence |
|------|--------|--------------|----------|
| 1 | Cart Abandonment Rate (75-100%) | **Critical** | 64.2% churn rate |
| 2 | Customer Service Calls (15+) | **Critical** | 70.3% churn rate |
| 3 | Days Since Last Purchase (186+) | **High** | 63.6% churn rate |
| 4 | Age Group (0-20) | **High** | 47.6% churn rate |
| 5 | Customer Service Calls (12-14) | **High** | 55.8% churn rate |

### Retention Opportunities

1. **Early Intervention:** Target customers at 31-61 days since last purchase (32.1% churn)
2. **Cart Recovery:** Implement aggressive cart abandonment campaigns for 50-75% abandoners
3. **Service Quality:** Reduce need for 6+ service calls through proactive support
4. **Youth Engagement:** Develop retention programs for under-20 demographic
5. **Geographic Focus:** Prioritize USA retention (largest revenue at risk: $7.2M)

---

## Data Quality

- ✅ **Zero Missing Values:** All calculations based on complete cleaned dataset
- ✅ **50,000 Records:** Full dataset coverage
- ✅ **26 Dimensions:** Comprehensive multi-dimensional analysis
- ✅ **Validated Aggregations:** All pivot tables cross-verified

---

## Next Steps

1. **Dashboard Development:** Visualize KPIs in `4. Dashboard/`
2. **Predictive Modeling:** Build churn prediction models using identified risk factors
3. **Segmentation Strategy:** Create targeted retention campaigns by segment
4. **A/B Testing:** Design experiments to reduce cart abandonment and service calls
5. **Executive Reporting:** Prepare presentation materials in `6. Presentation/`

---

**Status:** ✅ Analysis Complete  
**Total Pivot Tables:** 11  
**KPIs Calculated:** 5  
**Revenue Analyzed:** $72,031,314.60
