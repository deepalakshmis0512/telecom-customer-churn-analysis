# Telecom Customer Analytics: Call Center Performance & Customer Churn Dashboard

##  Project Overview
This project focuses on building an end-to-end data analytics and business intelligence solution for a major telecom corporation using Power BI. The analysis is divided into two operational segments: evaluating Call Center performance metrics to optimize customer service workflows, and analyzing historical Customer Churn data to establish risk mitigation strategies and minimize revenue loss.

---

## Part A: Call Center Performance Analytics 

###  Key Performance Indicators (KPIs) & Metrics Evaluated
Call Volume Metrics: Analyzed total inbound calls against successful resolutions to evaluate agent throughput.
Average Speed of Answer (ASA): Measures the average latency in seconds before an agent accepts an incoming call.
Customer Satisfaction (CSAT): Tracks overall customer approval percentages filtered across specialized service topics.
Operational Knowledge Gaps: Evaluated talk durations across both successfully resolved and unresolved tickets to identify training mismatches.

###  Data Pre-processing & Feature Engineering
* **Data Cleansing:** Implemented data validation protocols in Power Query to eliminate empty rows, drop duplicates, and trim trailing whitespaces from structural columns.
* **Time Scale Transformations:** Converted the baseline `AvgTalkDuration` from a time stamp format into a uniform integer value measuring total elapsed seconds using custom delimiter splitting algorithms.
* **Agent Performance Categorization:** Created a conditional metric branch to automatically flag speed-of-answer thresholds into operational tiers:
  * **GOOD:** Answered in less than 40 seconds.
  * **NEEDS IMPROVEMENT:** Answered between 40 and 79 seconds.
  * **POOR:** Response latency exceeding 80 seconds.


Core Operational Insights
Resolution Bottlenecks: Out of 4,504 calls, 408 concluded unresolved. Stacked visualization identified Streaming Services as the leading source of customer friction.

Agent Performance Latency: Individual tracking showed Becky had the fastest average pick-up rate (65.33s), while Joe recorded the slowest (70.99s).

Systemic Knowledge Gap: Unresolved calls (~223s) took virtually identical durations as resolved calls (~225s), indicating a critical training gap where agents exhaust call time without resolving the customer issue.

Customer Churn & Risk Analysis 
Lifecycle Binning (DAX)
To group customer tenures into structured 12-month annual fiscal blocks:


Strategic Customer Churn Observations
Macro Footprint: Out of 7,032 accounts, 1,869 completely churned—establishing a high company-wide baseline churn rate of 26.58%.

Financial Risk Exposure: Total cumulative revenue lost directly to the churned user segment reaches an estimated 2.86 Million Rupees.

Payment Pipeline Friction: Customers utilizing the Electronic Check payment gateway represented a staggering 57.3% of all churned accounts.

Infrastructure Deficiencies: High-speed network analysis revealed that 69% of exiting subscribers used Fiber Optic packages, highlighting possible regional reliability/pricing friction.

Support Escalation Deflection: 100% of subscribers who recorded 8 or 9 separate technical troubleshooting requests completely churned out.

Volatile Onboarding Window: Customer attrition peaks rapidly within the first year, with nearly 1,000 accounts churning in the 0-11 month tenure block.

Tool Stack
BI Architecture Engine: Power BI Desktop

Data Transformation Engine: Power Query Editor

Statistical Language: Data Analysis Expressions (DAX)
