# 📊 Meta Ad Performance Analysis  

## 🔗 Project Links  
- 🔗 Link to [Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMzkzMmM5OTQtOWIxNi00OGM3LWE4MzItNzRlZTFiNDYyNmY2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)
- 🔗 Link to [LinkedIn Post](https://www.linkedin.com/posts/charmi-patel-771815242_powerbi-dataanalytics-marketinganalytics-activity-7450572214657085441-cSKY?utm_source=share&utm_medium=member_desktop&rcm=ACoAADxG9wUBbNzooiZ3O29LUoPwn-wD8seWpN0)

## 📝 Problem Statement  

The business required a performance tracking solution for advertising campaigns running on **Facebook and Instagram**.  

The objective was to gain complete visibility into campaign performance across the entire marketing funnel — from **reach to engagement to conversion and budget utilization**.  

This analysis helps the marketing team to:  

- Identify the most effective platform  
- Track campaign ROI and optimize budget allocation.  
- Understand audience engagement patterns.  

---
## 📜 Scope of the Report
- **In Scope:** 
  - Campaigns running on Facebook and Instagram only.

- **Out of Scope:** 
  - Other platforms (Messenger, Audience Network).
  - Organic engagement (only paid ads will be included).

---

## 📜 Task List  

As a Data Analyst, I worked on the following:  

- Created key performance metrics (KPIs) to measure campaign effectiveness  
- Designed an interactive dashboard based on business requirements  
- Analyzed campaign data to generate actionable insights and recommendations  

---

## 📂 Dataset Understanding  

The dataset represents advertising performance data covering campaigns, ads, users demographics, and ad interaction events. It is modelled after how Facebook/Instagram (Meta) ad platforms capture data. 
The purpose of this dataset is to analyse advertising performance, optimize targeting, and 
measure ROI (Return on Investment) through KPIs such as: 
  - Impressions (how often ads are seen) 
  - Clicks (engagement with ads) 
  - Purchases (conversions) 
  - CPM, CPC, CTR, and ROAS (efficiency metrics) 
  - Audience insights (demographics, location, interests)

---

### 📊 Tables Overview  

#### 📌 ad_events  
- Stores all interaction events (impressions, clicks, shares, comments, purchases)  
- This is the **fact table** in the model because all KPIs are derived from events. 
- Used to analyze when and how users interact with ads.

#### 📌 ads  
- Contains ad-level details  of each ad creative. 
- Defines targeting criteria and which campaign an ad belongs to.
-  Used for platform-level and creative-type-level analysis (e.g., Facebook Video Ads vs Instagram Image Ads).  

#### 📌 campaigns  
- Stores campaign-level information including campaign strategy and budget allocation.  
- Provides timeframe and budget for ads.
- Used to calculate cost-based KPIs (CPC, CPM, ROAS).

#### 📌 users  
- Contains demographic data such as gender, age, and country
- Stores demographic and interest information of users who interact with ads.
- Used for audience segmentation (gender, age, country, location, interests).    
- Helps analyze targeting efficiency (are ads reaching the right audience?).  

---

## 📊 Data Model  

The dataset follows a **star schema**:  
<img width="1098" height="657" alt="image" src="https://github.com/user-attachments/assets/d9e87b20-daed-4e36-a266-559f65fc9968" />


- Fact Table: ad_events  
- Dimension Tables: ads, campaigns, users  

---

## 📊 Dashboard  

### 📶 Overall Analysis View  
Provides a complete funnel view of campaign performance from impressions to purchases  

### 📉 Home Page  
Displays key KPIs such as impressions, clicks, CTR, engagement rate, conversion rate, and purchase rate  
<img width="1546" height="885" alt="First page" src="https://github.com/user-attachments/assets/15fedca4-3f11-4cb8-a725-05058996c5eb" />

Tooltip used to get more insights:

<img width="1559" height="880" alt="1st page - tooltip" src="https://github.com/user-attachments/assets/7a9bac1f-2780-4623-a691-5026fab36112" />

---

## 🎓 Learning from this Project  

- Developed strong understanding of marketing funnel metrics such as **CTR, Engagement Rate, Conversion Rate, and Purchase Rate**  
- Learned how to analyze drop-offs across the funnel and identify performance gaps  
- Gained hands-on experience in building interactive dashboards for business stakeholders  
- Understood how audience targeting, ad creatives, and timing impact campaign success  

---

## ✍🏻 Some Important Insights from the Dashboard  

### 📌 Funnel Performance  

- High impressions and clicks indicate strong reach and visibility  
- CTR (~11.76%) and Engagement Rate (~13.56%) show ads are highly engaging  
- Only a small portion converts into purchases (low purchase rate ~0.61%)  

👉 Insight:  
Campaigns perform strongly at the **top of the funnel**, but there is a significant drop-off at the **conversion stage**  

---
### 📌 KPI Metrics  

- **Impressions: 216K** – Total number of times ads were shown, indicating strong reach  
- **Clicks: 25.4K** – Number of users who clicked on the ads  
- **Shares: 1.3K | Comments: 2.6K** – Additional engagement beyond paid reach  
- **Purchases (Conversions): 1.3K** – Actual customers acquired through ads  
- **Engagements: 29K** – Total interactions (clicks, shares, comments)  

- **CTR (11.76%)** – Strong performance, well above industry average (~1–2%)  
- **Engagement Rate (13.56%)** – Shows high user interaction with ads  
- **Conversion Rate (5.21%)** – Moderate conversion from clicks to purchases  
- **Purchase Rate (0.61%)** – Low conversion from impressions, indicating funnel inefficiency  

- **Total Budget: 2.5M** – Overall campaign spend  
- **Avg Budget per Campaign: 50.7K** – Indicates multiple campaigns were executed  

**Insight:**  
Campaigns perform well in terms of **reach and engagement**, but **conversion efficiency is low**.  
High CTR and engagement show strong ad appeal, while low purchase rate highlights a drop in the final stage of the funnel.  

---

### 👥 Engagement Breakdown  

#### By Gender  
- Female: **13K (43%)**  
- Male: **6K (22%)**  
- Other/Not Specified: **10K (35%)**  

**Insight:**  
Female users contribute the highest engagement, suggesting campaigns can be optimized further for this segment.  

---

#### By Age Group  
- Highest engagement: **20–30 age group**  
- Engagement drops significantly after 35+  

**Insight:**  
The primary audience is **young adults**, especially females aged 18–30.  

---

### 🌍 Geographic Distribution  

- Top countries: **US, India, Brazil, Germany, UK**  

**Insight:**  
- **India & US** → High engagement markets  
- **Germany & UK** → Higher purchasing potential  

---

### ⏰ Time-Based Trends  

#### Weekly Trend  
- Engagement remains consistent across weeks  

#### Hourly Trend  
- Peak engagement: **Afternoon & Evening (15–20 hrs)**  
- Lowest engagement: **Early morning (0–5 hrs)**  

**Insight:**  
Scheduling ads during peak hours can improve overall performance.  

---

### 📅 Calendar Insights  

- Engagement spread across days in June  
- Higher activity observed on **19th–21st and 25th–27th**  

**Insight:**  
Spikes align with campaigns or promotions, indicating **event-based engagement impact**.  

---

### 🎥 Ad Type Performance  

- **Video ads** perform best across CTR, conversion, and engagement  
- **Story ads** generate strong reach  
- **Image & Carousel ads** show slightly lower conversion performance  

**Insight:**  
Focusing more on **Video and Story ads** can improve ROI.  

---

### 📌 Conclusion & Recommendations  

- This analysis shows that while campaigns are effective in generating **awareness and engagement**, there is a clear opportunity to improve **conversion performance**.
- Target audience: **Females aged 18–30**  
- Best-performing formats: **Video > Stories > Carousel/Image**  
- Optimal timing: **Afternoon and evening hours**  
- Optimize budget allocation across high-performing regions and formats  
- Improve **landing pages, offers, and retargeting strategies** to increase conversions  

By addressing these areas, overall campaign performance and ROI can be significantly improved.
