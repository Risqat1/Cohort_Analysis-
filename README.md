# Cohort Analysis Dashboard

## TABLE OF CONTENT
- [PROJECT OVERVIEW](#Cohort Analysis-overview)
- [DATA SOURCE](#data-source)
- [TOOLS](#tools)
- [OBJECTIVES](#objectives)
- [METHODOLOGY](#methodology)
- [DATA ANALYSIS](#data-analysis)
- [DASHBOARD](#dashboard)
- [OBSERVATIONS](#observations)
- [RECOMMENDATIONS](#recommendations)


### Cohort Analysis OVERVIEW
This project analyzes weekly user retention across cohorts to identify churn and engagement patterns to track how long users remain active during their first 6 weeks after signup.
The analysis (as of 2021-02-07) was done using SQL for data extraction and Power BI for visualization. The goal is to deliver a clear, actionable picture of retention trends that can guide product and growth decisions.
This works showcases my ability to handle real world data challenges and deliver actionable insights through data storytelling and visualization.


### DATA SOURCE
The dataset was gotten as a project during my internship.


### TOOLS
  The tools used for this project are;
  - SQL
  - Microsoft Power BI

### OBJECTIVES
- Objectives:
The primary goal was to calculate and visualize weekly retention rates for user cohorts, identify trends in user engagement and churn and communicate insights in a visual and analytical format that supports data-driven decision-making.
- Monitor Retention Trends: Track user activity from Week 0 (sign-up) through Week 6 to uncover patterns of engagement and drop-off.
- Monitor Churn Trends: Identify the weeks where user loss is most pronounced to guide targeted retention strategies.
- Enable Informed Decisions: Deliver insights and visualizations that help product, marketing, and growth teams enhance user experience, reduce churn, and increase customer lifetime value.
Retention matters: in today’s competitive e-commerce space, keeping users is often cheaper than acquiring new ones. Research shows that improving retention by just 5% can increase profits by 25–95%, making this analysis vital for sustainable growth.


### METHODOLOGY
1.Data Exploration: Began with the subscription table to understand its structure (user_pseudo_id, subscription_start_date, subscription_end_date). Ran checks for missing values, duplicates, and inconsistencies that could distort retention calculations.

2.Single Cohort Test: Built a baseline query for one cohort (users who joined during the week of 2021-01-04). Standardized the start dates to weekly buckets and measured retention from Week 0 to Week 6 by checking if subscriptions were still active.

3.Scaling to Multiple Cohorts: Expanded the query to calculate retention for every weekly cohort. Each row represented a cohort (cohort_week), while columns captured retention across Week 0 to Week 6. Used conditional aggregation to measure activity levels and calculate retention percentages.

4.Data Export: Once the SQL produced the required results, exported the dataset to CSV/Google Sheets for easier visualization and integration with BI tools.

5.Visualization: Created a heatmap to highlight retention across cohorts (rows = cohort start week, columns = retention week).

6.Insights & Recommendations: Analyzed the visuals to pinpoint major drop-off weeks, identify strong-performing cohorts, and connect patterns to potential business drivers (onboarding, pricing, campaign timing).


### DATA ANALYSIS
-	Key Performance Indicators (KPIs):
      - Total value: 1M
      - Avg Retention: 91%
      - Avg Churn: 9%
      - Critical Drop-Off:35.32%
      - Total Drop-off:7.19%
    

### DASHBOARD
<img width="1098" height="639" alt="Screenshot 2025-09-05 185927" src="https://github.com/user-attachments/assets/b7335cd7-2efd-45b6-a106-79f714f11ff3" />
<img width="1126" height="645" alt="Screenshot 2025-09-05 190212" src="https://github.com/user-attachments/assets/2d6ef6a4-517a-4fdf-a2c8-d5abe32642c1" />



### OBSERVATIONS
⦁	 Customer Retention by cohort:
Retention starts at 100% in week 1 and drops by week 6, with Nov 2020 declining to 85% while dec 2020 and Jan 2021 remain more stable between 97% and 91%.

⦁	 Customer Churn by cohort:
Churn is relatively low in week1(1-6%) across all cohorts. From Week 2-6, it gradually increases reaching 8-15%, with Nov 2020 showing the highest rise, while dec 2020 and Jan 2021 remain more stable.

⦁	 Drop Off by cohort:
The highest drop off occurs in week 2 at 8% with subsequent weeks showing smaller declines between 5% - 1% across all cohorts.

⦁	Average Retention by cohort:
 Retention starts strong at 95% in week 1 and gradually declines to 89% by Week 6.



### RECOMMENDATIONS
- Reduce early churn (Weeks 1–3) with personalized onboarding, re-engagement campaigns, and A/B testing of pricing/promotions.
-  Leverage AI-driven personalization to predict churn and automate retention strategies.
-  	Integrate cohort data with product usage and customer feedback for deeper insights and smarter decisions.

