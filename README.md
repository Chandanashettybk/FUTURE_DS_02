# FUTURE_DS_02

📊 Facebook Ads Campaign Performance Dashboard
📝 Project Overview

This project is an interactive Power BI dashboard built from a real Facebook Ads dataset.
The goal is to help marketers and business owners answer key questions such as:

✅ How well did the ad campaign perform overall?

✅ Which ads had the highest engagement?

✅ What was the Click-Through Rate (CTR), Cost per Click (CPC), and Return on Investment (ROI)?

✅ Which age groups or demographics responded the best?

✅ What improvements can we make for future campaigns?

The dashboard gives both a high-level executive overview and detailed drill-down insights.

📂 Dataset

The dataset (fb ads.xlsx) contains information about ad campaigns, including:

1. ad_id – Unique identifier for each ad

2. campaign_id / fb_campaign_id – Campaign-level grouping

3. reporting_start / reporting_end – Reporting period

4. impressions – Number of times the ad was shown

5. clicks – Number of times users clicked the ad

6. spent – Total spend in that period

7. total_conversion – Total number of conversions

8. approved_conversion – Approved/validated conversions

9. demographics – Age, gender, etc. for audience segmentation

🛠 Data Cleaning Steps

Removed duplicates in ad_id.

Handled missing values in campaign_id and fb_campaign_id.

Converted numeric columns (impressions, clicks, spent, conversions) to valid numbers.

Replaced negatives with 0 since impressions/clicks can’t be negative.

Applied logical rules:

clicks <= impressions

approved_conversion <= total_conversion

Missing values in clicks/spend/conversions were filled with 0.

Dates were standardized to dd/mm/yyyy.

📈 Measures (DAX)

Some of the KPIs calculated in Power BI:

Total Impressions = SUM(Impressions)

Total Clicks = SUM(Clicks)

CTR % = Clicks ÷ Impressions

CPC (Cost per Click) = Spend ÷ Clicks

CPM (Cost per 1000 Impressions) = Spend ÷ Impressions × 1000

CVR % (Conversion Rate) = Conversions ÷ Clicks

Approval Rate % = Approved ÷ Conversions

CPA (Cost per Approved Conversion) = Spend ÷ Approved




📊 Dashboard Features

Executive Overview Page

KPI Cards for Impressions, Clicks, CTR, Spend, Conversions, ROI, etc.

Trend charts for Spend, Clicks, and Impressions over time

Top-Performing Ads

Bar charts showing best ads by Clicks, CTR, CPA

Conditional formatting to highlight good/bad performers

Audience Insights

Stacked charts for engagement by Age & Gender

Slicers for Age, Gender, Campaign, and Date

Drill-through & Tooltips

Drill into any ad_id to see daily trends

Tooltips show mini KPI summaries

🚀 Insights from the Dashboard

Campaign performance fluctuates by age group → younger segments show higher CTR.

Some ads had high spend but low CTR → opportunity to improve creatives.

ROI improves when budget shifts toward high-performing demographics.

Cost per Conversion can be reduced by focusing on approved conversion efficiency.

📌 How to Use

Clone the repo or download files.

🎯 Key Learnings

* Hands-on practice with data cleaning and logical validation.

* Built advanced Power BI measures with DAX.

* Learned how to structure KPI dashboards for business decisions.

* Practiced storytelling with data for actionable insights.
Open fb ads.xlsx in Power BI.

Import the DateTable.csv (for proper date hierarchy).

Apply the DAX measures provided.

Explore the dashboard interactively!
