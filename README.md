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
**Key Metric**: 62.67% Drop Rate in overall business performance.
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
---
## 📊 Key Findings (From the Data)

### Crisis Impact Summary

| Metric | Pre-Crisis | Crisis | Change | % Change |
|--------|-----------|--------|--------|----------|
| Monthly Orders | 24,000 | 9,000 | -15,000 | -62.5% |
| Monthly Revenue | ₹7.6M avg | ₹2.75M avg | -₹4.85M | -63.8% |
| Total Revenue (period) | ₹38M | ₹11M | -₹27M | -71% |
| Active Customers | 100,000 | 27,000 | -73,000 | -73% |
| Avg Rating | 4.55 stars | 2.30 stars | -2.25 | -49% |
| SLA Compliance | 44% | 12% | -32% | -73% |
| Avg Delivery Time | 40 min | 60 min | +20 min | +50% |
| Cancellation Rate | 6.2% | 11.6% | +5.4% | +87% |

**1. Business Overview & Revenue Erosion**
**Total Orders:** 149K (Cumulative).

The "**June Cliff**": Monthly revenue dropped from a peak of **7.8M (March) to 2.9M ** in June, failing to recover through September.

Geographic Epicenter: Bengaluru saw the highest impact, contributing 33.18% of total orders but suffering the highest volume of churn (15,170 customers).

**2. Customer Sentiment & Churn**

**Customer Base:** Total of 105K unique customers, with 87K active Pre-Crisis and only 32K during the Crisis.

**Top Complaint Categories:**

   Food Safety Issue: 472 reports.
   
   Bad Taste: 326 reports.

   Late Deliveries: 321 reports.
   
   Sentiment Shift: Avg Sentiment Score crashed from 0.89 (Pre-Crisis) to -0.18 (Crisis).
   
**3. Operational Bottlenecks**

**SLA Avg Delay:** 12.35 minutes (reaching a peak of 20.74 mins in June).

**Cancellation Rate**: Stabilized at 7.4%, with Ahmedabad and Bengaluru showing the highest volatility.

**Vehicle Performance:** Cars showed the lowest SLA compliance (17.8%), while Bikes and Scooters remained slightly more resilient (~21%).

**4. Restaurant Partner Risk**

**Risk Distribution:** 56.7% of partners are now classified as High Risk.

**Partner Exodus:** Total of 11.4K partners analyzed, with a significant portion of "Active Customers" dropping off in major hubs like Mumbai and Delhi.

---
## 🛠️ Methodology & Technical Implementation
**The Analytical Framework**

**1.Phase Segmentation:** Used DAX to bifurcate data into Pre-crisis and Crisis phases based on the June 1st cutoff.

**2. SLA Analysis:** Calculated SLA Compliance % by comparing actual delivery time vs. promised time.

**3. Sentiment Quantization:** Transformed 69K reviews into a sentiment index scale of -1 to 1.

**Key DAX Metrics Used**

**◆ Drop %:** (Pre-Crisis Orders - Crisis Orders) / Pre-Crisis Orders

 **◆ SLA Compliance:** Percentage of orders delivered within the promised window.
 
**◆ Customer Status:** Categorized users as Churned (Pre-Crisis but NOT Crisis) vs. Retained (Both phases).

## 💡 Strategic Recommendations
◆ Priority 1: The "Bengaluru Recovery": Focus 40% of the recovery budget on Bengaluru, as it holds the highest density of "Recoverable" churned customers.

◆ Priority 2: Operational Redundancy: Since Cars failed significantly during the crisis (17.8% SLA), shift the fleet mix toward 2-wheelers for better urban agility.

◆ Priority 3: Quality Control: Terminate the bottom 5% of restaurants (e.g., Kolkata Paratha Central, Sri Thali Clouds) who consistently drove the "Food Safety" complaints.

◆ Priority 4: Trust Rebuilding: Launch a "Safety First" campaign targeting the 47K Positive Review leavers who churned solely due to the June outage.

---
# 🛠️ Technical Implementation

### Tools & Technologies Used

**Data Visualization:**
- **Power BI Desktop:** Interactive dashboards, 6 comprehensive pages
- **Visual Types:** Cards, charts, tables, donut charts, heatmaps, slicers
- **DAX Functions:** CALCULATE, SWITCH, IF, DIVIDE, DISTINCTCOUNT, SUMMARIZE

**Data Analysis:**
- **DAX Measures:** 50+ custom measures for segmentation, risk scoring, ROI
- **Calculations:** Statistical aggregations, trend analysis, probability scoring
- **Modeling:** Customer lifetime value, churn probability, recovery potential

  ---
  ### Dashboard Structure

**Page 1: Home**
- Quick navigation to all analysis sections
<img width="1907" height="920" alt="image" src="https://github.com/Lakshmi-799/QuickBite-Express-Crisis-Impact-and-Recovery-Analysis/blob/main/home.png" />

**Page 2: Executive Summary**
- KPI cards: Total orders, Avg Delivery Time, Avg rating, cancellations, Drop%
- Revenue by months and Crisis
- Total Orders by Crisis Phase
- Total oders and cancellation rate by month
- Top affected cities
- Revenue breakdown by component
<img width="1917" height="922" alt="image" src="https://github.com/Lakshmi-799/QuickBite-Express-Crisis-Impact-and-Recovery-Analysis/blob/main/businessOverview.png" />



**Page 3: Customer Impact Analysis**
- Customer segmentation donut
- City distribution
- Dropped Customers in city level
- High-value customer impact
  <img width="1916" height="926" alt="image" src="https://github.com/Lakshmi-799/QuickBite-Express-Crisis-Impact-and-Recovery-Analysis/blob/main/customer%20analysis.png" />


**Page 5: Operational Insights**
- SLA compliance trends in monthly
- Cancellation Rate and Total orders in Cities
- SLA Compalince by vehicle type
- Cancellation rates by city
- Monthly operational metrics table
  <img width="1920" height="912" alt="image" src="https://github.com/Lakshmi-799/QuickBite-Express-Crisis-Impact-and-Recovery-Analysis/blob/main/Delivery.png" />


**Page 6: Restaurant Partnership Analysis**
- Pre Crisis and Crisis customers by Cuisine type
- Cancellation rate by Restaurant 
- Top and bottom Restaurant by orders
- Restaurant risk categorization
- Active and Dropped Customers by City
  <img width="1916" height="906" alt="image" src="https://github.com/Lakshmi-799/QuickBite-Express-Crisis-Impact-and-Recovery-Analysis/blob/main/Patnership.png" />


**Page 7: Customer Sentiment Analysis**
- Average Rating by Month
- Review volume timeline
- Negative reviews
- Top Restaurant Rating and Reviews
<img width="1915" height="923" alt="image" src="https://github.com/Lakshmi-799/QuickBite-Express-Crisis-Impact-and-Recovery-Analysis/blob/main/Reviews%26rating.png" />
