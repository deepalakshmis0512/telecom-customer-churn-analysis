# Telecom Customer Analytics: Call Center Performance & Customer Churn Dashboard

##  Project Overview
This project delivers an end-to-end business intelligence and data analytics solution developed in Power BI for a major telecom corporation. The analytical framework is split into two strategic streams: optimizing frontline customer service workflows through Call Center Performance Analytics, and identifying financial risk exposure through data-driven Customer Churn & Risk Analysis.

---

## Part A: Call Center Performance Analytics 

### ⚙️ Data Pre-processing & Feature Engineering
* **Data Cleansing:** Standardized text fields, eliminated duplicate entries, and utilized Power Query's Trim function to remove trailing whitespaces from structural columns.
* **Format Standardization:** Transformed the average talk duration from an un-calculable time stamp into a uniform integer measuring total elapsed seconds using specialized split-column delimiter transformations in Power Query.
* **Agent Performance Tiering:** Implemented conditional logic to dynamically categorize agent response latency into three strict operational tiers: GOOD (under 40 seconds), NEEDS IMPROVEMENT (40 to 79 seconds), and POOR (80 seconds or deeper).

### Core Operational Insights & Observations
* **Streaming Resolution Bottlenecks:** Out of 4,504 total calls, 408 concluded without resolution. Cross-filtering identified Streaming Services as the leading source of customer friction, pinpointing an immediate need for targeted technical support training.
* **Agent Efficiency Disparities:** Performance tracking isolated individual latency bottlenecks. Becky demonstrated peak operational efficiency with the fastest average response rate of 65.33 seconds, while Joe recorded the slowest at 70.99 seconds.
* **Systemic Technical Knowledge Gaps:** Talk duration analysis revealed that unresolved calls averaged 223 seconds, which is virtually identical to the length of successfully resolved calls at 225 seconds. This shows that agents are exhausting significant call time without successfully resolving the underlying customer issues.

---

## Part B: Customer Churn & Risk Analysis 

###  Lifecycle Tenure Segmentation
To effectively track customer attrition across chronological milestones, raw customer tenure datasets were mathematically grouped into structured, annual 12-month fiscal blocks using optimized conditional row logic.

###  Strategic Customer Churn Observations
* **Macro Churn Footprint:** Out of 7,032 total active accounts, 1,869 customers transitioned into churn status, establishing a critical company-wide customer churn rate of 26.58%.
* **Financial Risk Exposure:** The cumulative structural revenue loss stemming directly from the churned user segment is projected at a substantial 2.86 Million Rupees.
* **Payment Pipeline Friction:** Transactional gateway analysis indicated a severe operational vulnerability within the Electronic Check payment option, which alone accounted for 57.3% of all churned accounts.
* **Infrastructure Deficiencies:** High-speed network segmentation revealed that 69% of exiting subscribers were bound to Fiber Optic internet packages, highlighting potential service reliability issues or uncompetitive pricing models.
* **Technical Support Thresholds:** Customer escalation tickets showed a direct correlation with user attrition. Exactly 100% of subscribers who recorded 8 or 9 individual technical troubleshooting requests completely churned out of the company ecosystem.
* **Volatile Onboarding Window:** Attrition heavily peaks during the initial adoption lifecycle phase, with nearly 1,000 accounts churning within the very first 0-11 month tenure window.

---

##  Tool Stack & Architecture
* **BI Architecture Engine:** Power BI Desktop
* **Data Transformation Engine:** Power Query Editor
* **Data Source Layer:** Microsoft Excel Workbooks
