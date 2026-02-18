# Dashboard

## Overview

This folder contains interactive visualizations and KPI dashboards for the E-commerce Customer Churn Analysis. All visualizations are built from validated data and calculations to provide actionable business insights.

---

## Files

**Filename:** `G-6 DVA Capstone Dashboard.csv`  
**Source:** Cleaned Dataset + Pivot Table Analysis  
**Dashboard Type:** Executive KPI Dashboard  
**Format:** CSV/Excel with embedded charts and visualizations  
**Last Updated:** 2024

---

## Dashboard Components

### 1. Executive KPI Cards

**Primary Metrics:**
- **Total Customers:** 50,000
- **Churned Customers:** 14,450 (28.9%)
- **Active Customers:** 35,550 (71.1%)
- **Total Revenue:** $72,031,314.60
- **Revenue at Risk:** $20,597,365.76 (28.6%)
- **Average Order Value:** $123.12
- **Average Returns Rate:** 6.68%

### 2. Churn Analysis Visualizations

**Geographic Churn Distribution:**
- Country-wise churn rates and revenue impact
- Highest risk: USA (5,056 churned, $7.2M lost)
- Best retention: France (27.3% churn rate)

**Demographic Churn Patterns:**
- Gender distribution (minimal variance: 28-31%)
- Age group analysis (0-20 age group: 47.6% churn)
- Membership tenure distribution

**Behavioral Churn Indicators:**
- Cart abandonment vs churn correlation
- Days since last purchase impact
- Customer service calls frequency analysis

### 3. Revenue & Financial Dashboards

**Lifetime Value Analysis:**
- Active customer LTV: $51.4M ($1,446.81 avg)
- Churned customer LTV: $20.6M ($1,425.42 avg)
- Country × Gender segment breakdown
- Top performing segments identification

**Purchase Behavior:**
- Quarterly purchase trends (Q4 peak: 198,134 purchases)
- Average order value by churn status
- Total purchases comparison (Active: 13.84 vs Churned: 11.37)

### 4. Engagement & Retention Metrics

**Customer Engagement Score:**
- Social media engagement correlation with session duration
- Mobile app usage patterns (0-100 scale)
- Engagement tiers: Low (14.19%) to High (35.94%)

**Retention Risk Indicators:**
- Purchase recency analysis (0-287 days)
- Cart abandonment rate distribution (0-100%)
- Service call volume impact on churn

### 5. Predictive Churn Indicators

**High-Risk Segments:**
- Cart abandonment 75-100%: 64.2% churn rate
- Customer service calls 15+: 70.3% churn rate
- Days since purchase 186+: 63.6% churn rate
- Age group 0-20: 47.6% churn rate
- Service calls 12-14: 55.8% churn rate

**Early Warning Signals:**
- 31-61 days since purchase: 32.1% churn
- 50-75% cart abandonment: 26.2% churn
- 6-8 service calls: 40.6% churn

---

## Key Insights from Dashboard

### Critical Findings

1. **Revenue Impact:** $20.6M in lifetime value lost to churn (28.6% of total revenue)
2. **Geographic Concentration:** USA accounts for 35% of churned revenue ($7.2M)
3. **Behavioral Predictors:** Cart abandonment and service calls are strongest churn indicators
4. **Age Factor:** Youngest customers (0-20) churn at nearly 2x the average rate
5. **Purchase Recency:** Churn risk increases 2.5x after 186 days of inactivity

### Actionable Recommendations

**Immediate Actions:**
- Implement cart recovery campaigns for 50-75% abandonment segment
- Proactive outreach at 31-day purchase milestone
- Service quality improvement to reduce call volume
- Youth-focused retention programs

**Strategic Initiatives:**
- USA market retention strategy (highest revenue at risk)
- Engagement programs to increase session duration
- Mobile app optimization (current usage: 19.29%)
- Q4 seasonal campaign optimization

---

## Dashboard Metrics Summary

| Category | Metrics Count | Visualization Type |
|----------|---------------|-------------------|
| **KPI Cards** | 7 | Numeric indicators |
| **Geographic Analysis** | 8 countries | Bar charts, heat maps |
| **Churn Predictors** | 5 factors | Scatter plots, trend lines |
| **Revenue Breakdown** | 16 segments | Stacked bars, pie charts |
| **Engagement Scores** | 5 tiers | Line charts, gauges |
| **Time-based Analysis** | 10 ranges | Histograms, time series |

---

## Data Refresh Protocol

**Source Dependencies:**
1. Cleaned Dataset (50,000 records)
2. Pivot Table Calculations (11 tables)
3. KPI Calculations (5 metrics)

**Refresh Frequency:** On-demand or scheduled
**Validation:** All metrics cross-verified with source data

---

## Usage Guidelines

### For Executives
- Focus on KPI cards for high-level overview
- Review revenue impact and geographic distribution
- Prioritize high-risk segment interventions

### For Marketing Teams
- Use engagement metrics for campaign targeting
- Leverage demographic insights for personalization
- Monitor cart abandonment trends

### For Customer Success
- Track service call volume and satisfaction
- Identify at-risk customers via purchase recency
- Monitor retention rates by segment

### For Data Analysts
- Drill down into segment-level performance
- Validate predictive indicators
- Export data for advanced modeling

---

## Technical Specifications

**Data Volume:** 50,000 customer records  
**Calculation Engine:** Pivot tables + aggregations  
**Visualization Tools:** Excel charts, conditional formatting  
**Interactivity:** Filters, slicers, drill-down capabilities  
**Export Formats:** PDF, PNG, Excel, CSV

---

## Performance Benchmarks

| Metric | Current | Industry Benchmark | Status |
|--------|---------|-------------------|--------|
| Churn Rate | 28.9% | 20-25% | ⚠️ Above average |
| Cart Abandonment | 50.6% avg | 60-80% | ✅ Below average |
| Returns Rate | 6.68% | 8-10% | ✅ Below average |
| AOV | $123.12 | Varies | ℹ️ Context-dependent |
| Customer LTV | $1,440.62 | Varies | ℹ️ Context-dependent |

---

## Next Steps

1. **Predictive Modeling:** Build ML models using dashboard insights
2. **A/B Testing:** Design experiments for high-risk segments
3. **Automated Alerts:** Set up real-time churn risk notifications
4. **Executive Presentation:** Prepare stakeholder materials in `6. Presentation/`
5. **Documentation:** Archive methodology in `5. Documentation/`
