<img width="806" height="768" alt="image" src="https://github.com/user-attachments/assets/91f71b9d-2410-4ee7-8dbe-a6a05e70fe9a" /># Social Media Performance Analysis Documentation

## Project BackGround

I’ve been given a 2024 dataset capturing detailed records of
post-level performance metrics, platform details, content types,
and geographic reach.
The dataset consolidates information about various posts
published across TikTok, Instagram, LinkedIn, and X.com.
It includes metadata such as post type (video, carousel, text),
content category (product promotion, educational,
entertainment), publishing times, and associated hashtags. It
also tracks performance indicators like engagement, views,
impressions, clicks, click-through rates, and post reach across
countries and regions.
Your goal is to build a report that reveals what makes content
successful on different platforms, explains regional trends in
engagement, and informs better content and platform strategy
decisions.

## 📊 Insights and Recommendations are Provided on the Following Key Areas:
📍 Category 1: Platform & Post-Type Performance

🌍 Category 2: Regional Engagement Trends

⏰ Category 3: Timing Optimization

🏷️ Category 4: Hashtag & Content Category Effectiveness

## 🧠 Data Structure & Initial Checks
The company’s primary database contains one comprehensive table:
social_media_posts — with ~150,000 rows of post-level data from 2024–2025. Key fields include:

Platform, Content_Type, Content_Category

Post_Hour, Post_Date, Post_Published_At

Region, Engagement, Views, Impressions, CTR

Video_Views, Live_Stream_Views, Main_Hashtag


<img width="1125" height="653" alt="image" src="https://github.com/user-attachments/assets/d0a0b765-cc75-4f96-920b-084f01017856" />


Initial checks involved:

-Filtering out nulls in Clicks and Click_Through_Rate

-Creating a derived Post_Type (Organic vs Sponsored)

-Extracting Post_Hour and Weekday from timestamps

-Creating a Date Dimension Table for time-based filtering


## 🧭 Executive Summary
## 🔍 Overview of Findings
If you’re a content strategist or social media manager, the key takeaways are:

-Educational content consistently drives the highest engagement across platforms.

-Posting between 11 AM and 4 PM leads to peak interaction, especially on weekdays.

-Sponsored content, while less frequent, tends to yield higher CTRs across most regions.

![Dashboard Snapshot Here]
<img width="1348" height="748" alt="social media nalysis page 1" src="https://github.com/user-attachments/assets/4f6c8aaa-de6a-42ee-b642-0a8c5cfae08b" />
<img width="1330" height="738" alt="social analysis page 2" src="https://github.com/user-attachments/assets/bef5d0a5-6b59-493d-858a-cb99ad9eccb7" />


## 📌 Insights Deep Dive
### 📍 Category 1: Platform & Post-Type Performance
Main Insight 1: Instagram and TikTok lead in total engagement with over 40% share combined.
Main Insight 2: Sponsored posts average a CTR of 2.8+, slightly outperforming organic content.
Main Insight 3: Facebook has the highest impressions but comparatively lower engagement rates.
Main Insight 4: Posts tagged with Product Promotion or Educational content perform better across all platforms.

📊 Visual: Bar Chart – Engagement by Platform & Post Type
<img width="782" height="692" alt="image" src="https://github.com/user-attachments/assets/9bd14579-03f5-47bd-9078-22515c9ada41" />

<img width="807" height="777" alt="image" src="https://github.com/user-attachments/assets/36cd4d71-82a2-4077-82e6-ddcb10b48ffe" />

### 🌍 Category 2: Regional Engagement Trends
Main Insight 1: USA, Japan, and Brazil top the list for both engagement and CTR.
Main Insight 2: Regions like Germany and India show high impressions but lower clicks.
Main Insight 3: Japan recorded the highest CTR at 3.07, suggesting high content relevance.
Main Insight 4: Regional video viewership is highest in North America and South America.

📊 Visual: ZoomCharts Map + Regional Table + Bar Chart for Views
<img width="782" height="652" alt="image" src="https://github.com/user-attachments/assets/01fe1f15-5a53-4268-8787-211e5c09f1ca" />

### ⏰ Category 3: Timing Optimization
Main Insight 1: Posts at 11 AM and 4 PM show the highest engagement.
Main Insight 2: Weekdays (especially Tuesdays and Thursdays) outperform weekends.
Main Insight 3: TimeSeries charts show afternoon posting drives consistent video views.
Main Insight 4: There is a weak correlation between Post_Hour and Engagement, suggesting it's more about content type than exact hour.

📊 Visual: TimeSeries ZoomChart + Heatmap or Hourly Area Chart
<img width="806" height="768" alt="image" src="https://github.com/user-attachments/assets/1a0c01fc-da68-4428-a467-04eade01efbd" />
<img width="806" height="765" alt="image" src="https://github.com/user-attachments/assets/b3d240ad-3a43-48ff-b6aa-fc000c83f27d" />


### 🏷️ Category 4: Hashtag & Content Category Effectiveness
Main Insight 1: Posts using hashtags related to “#CustomerStory” and “#ProductDemo” performed well.
Main Insight 2: Hashtag usage increased CTRs by 8–10% on average when combined with Sponsored posts.
Main Insight 3: Educational and Product-related categories lead in impressions and clicks.
Main Insight 4: Scatter plot shows moderate correlation between content category and engagement rate.

📊 Visual: Matrix Chart (Hashtag vs CTR), Scatter Plot – Category vs Engagement
<img width="378" height="686" alt="image" src="https://github.com/user-attachments/assets/0ab18cd6-cef2-4f1c-8ff5-43232671f1d1" />

## Recommendations
Based on the above findings, we recommend the Marketing & Content Team to:

-Focus efforts on Educational and Product Promotion content as they consistently perform across all regions.

-Schedule posts between 11 AM – 4 PM on weekdays to maximize engagement.

-Prioritize sponsored content for important campaigns — it yields higher CTRs in regions like Japan and Canada.

-Invest in video and live stream content for North & South American markets where viewership is highest.

-Use effective hashtags and test combinations with click-oriented CTAs.

## Assumptions and Caveats
-Missing Click Data (~15%) was left as null due to lack of pattern for imputation.

-All "Sponsored" classifications were based on keyword rules in Content_Type.

-Engagement metrics are not normalized by follower base — this may skew platform-level comparisons.

-Some timestamps were converted to local region time manually (for regional analysis).

-Hashtag performance assumed only the main hashtag per post due to data limitations.
