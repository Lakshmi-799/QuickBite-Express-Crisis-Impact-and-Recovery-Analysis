# QuickBite-Express-Crisis-Impact-and-Recovery-Analysis
In June 2025, QuickBite Express lost 70% of its customer base in less than 90 days.
This repository contains my complete Power BI analysis of what went wrong — and how data can guide the recovery.

**A comprehensive data-driven analysis of a food delivery startup's crisis 
and evidence-based recovery strategy.**

---
## 📋 Table of Contents

1. Project Overview
2. Problem Statement
3. Dataset Description
4. Methodology
5. Key Findings
6. Recommendations
7. Technical Implementation
8. Deliverables
9. Sources & References
10. How to Explore
## 🎯 Project Overview

**Project Type:** Business Case Analysis | Data Analytics | Strategic Consulting  
**Domain:** Food Delivery & Consumer Analytics  
**Time Period Analyzed:** January - September 2025  
**Focus:** Crisis Analysis & Recovery Strategy Development  
**Tools Used:** Power BI, DAX, Excel
**Audience:** Data Analysts, Business Strategists, Recruiters
### Executive Summary

In June 2025, QuickBite Express - a Bengaluru-based food delivery startup 
(founded 2020) - faced a critical crisis triggered by:
- Viral food safety incident involving partner restaurants
- Week-long delivery infrastructure outage during monsoon season
- Aggressive competitor campaigns capitalizing on operational failures
  **Crisis Impact:**
- 73,000 customers churned (70% of active base)
- ₹27 million revenue lost in 4 months
- Customer ratings collapsed from 4.5 → 2.3 stars
- 20% restaurant partner exodus

**Key Discovery:**
Despite the severity, **30% of churned customers (22,000) were recoverable** 
because they left due to operational failure, not dissatisfaction.

**Strategic Output:**
A data-driven ₹70-80M recovery roadmap with 4 strategic pillars, expected 
to achieve 80-90% recovery within 6-9 months with 3-4x ROI on reactivation.

---
## 💼 Problem Statement

### Business Challenge

QuickBite Express requires a comprehensive analysis of its June-September 2025 
crisis to:

1. **Understand Crisis Severity:** Quantify impact across all business metrics
2. **Identify Root Causes:** Determine what triggered the cascade of failures
3. **Customer Impact Analysis:** Segment churned customers by recovery probability
4. **Competitive Context:** Benchmark against industry peers during crisis
5. **Recovery Strategy:** Design a data-backed turnaround plan with timelines & ROI
6. **Operational Insights:** Identify systemic vulnerabilities to prevent recurrence

### Analysis Questions Addressed
**Primary Analysis (10 questions):**
1. Monthly order decline comparison (pre-crisis vs crisis)
2. Top 5 cities by order decline percentage
3. Top 10 high-volume restaurants with largest decline
4. Cancellation rate trend analysis and geographic impact
5. Delivery SLA performance degradation
6. Monthly customer rating fluctuations
7. Negative keyword sentiment analysis
8. Revenue impact quantification
9. Loyalty impact on 5+ order customers with 4.5+ ratings
10. High-value customer (top 5%) decline patterns
---
### Data Sources

| Data Type | Source | Time Period | Records | Key Metrics |
|-----------|--------|-------------|---------|------------|
| **Orders** | QuickBite transactional DB | Jan-Sep 2025 | 149K orders | order_id, customer_id, order_date, order_total, phase |
| **Customers** | CRM system | Jan-Sep 2025 | 105K customers | customer_id, acquisition_date, total_spend, LTV |
| **Reviews & Ratings** | Review system | Jan-Sep 2025 | 48K reviews | rating, sentiment, review_text, date |
| **Restaurant Data** | Partner DB | Jan-Sep 2025 | 20K restaurants | restaurant_id, cuisine_type, order_count, status |
| **Operational Metrics** | Delivery/Operations DB | Jan-Sep 2025 | Daily logs | delivery_time, sla_compliance, cancellations, delays |


