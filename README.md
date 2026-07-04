# Apple-Social-Media-Analytics-M.S-EXCEL
Excel-based analytics project exploring Apple's social media performance — engagement, platform comparison, hashtag/content strategy, campaign effectiveness, and follower retention — built from a synthetic dataset of ~300 posts across six platforms.

## Dataset

The core dataset (`Posts` sheet, replicated across several workbooks) contains one row per post with:

| Column | Description |
|---|---|
| `PostID` | Unique post identifier |
| `Platform` | YouTube, LinkedIn, Instagram, Twitter, TikTok, etc. |
| `Date` | Post date |
| `ContentType` | Image, Video, Carousel, Tweet |
| `Hashtags` | Comma-separated hashtags used |
| `Likes`, `Shares`, `Comments` | Engagement counts |
| `Clicks`, `Reach`, `Impressions` | Reach/traffic metrics |
| `Campaign` | Associated marketing campaign |

A companion `Engagement Summary` sheet tracks weekly follower/ad-spend data per platform (`New_Followers`, `Unfollows`, `Total_Followers`, `Net_followers_gain`, `Engagement_Rate`, `Ad_Spend`), and a campaign table (`Task 5.1.2`) holds campaign metadata (`Start_Date`, `End_Date`, `Objective`, `Ad_Spend`, `Impressions`, `Engagement_Uplift`, pre/during-campaign engagement).

## Repository structure

```
Apple Social Media Analytics/
├── 1 Data Preprocessing & Cleaning.xlsx
├── 2 Engagement Analysis.xlsx
├── 3 Platform Analysis.xlsx
├── 4 Hashtag & Content Strategy.xlsx
├── 5 Campaign Effectiveness task.xlsx
├── 6 Follower Retention & Loyalty task.xlsx
└── task 7.xlsx
```

### 1. Data Preprocessing & Cleaning
Raw `Posts` data plus cleaning steps: splitting `Platform`/`Date`, isolating numeric engagement columns, and parsing multi-value `Hashtags` into individual tags (tasks 1.1–1.4).

### 2. Engagement Analysis
Computes per-post engagement rate and aggregates it by content type and hashtag (average clicks per hashtag, average engagement rate per hashtag/campaign) — tasks 2.1–2.4.

### 3. Platform Analysis
Pivot-style comparisons of average engagement rate by platform and campaign, net follower growth by platform, and average engagement rate vs. ad spend by platform — tasks 3.1–3.4.

### 4. Hashtag & Content Strategy
Post-count and average-engagement breakdowns by hashtag, and average engagement rate by campaign × content type — tasks 4.1–4.4.

### 5. Campaign Effectiveness
Compares pre-campaign vs. during-campaign engagement, computes engagement uplift, campaign ROI, and net follower gains attributable to each campaign — tasks 5.1–5.2.

### 6. Follower Retention & Loyalty
Weekly net follower gains by platform, rolling averages to smooth growth trends, peak-growth weeks, and a correlation of ad spend vs. follower growth — tasks 6.1–6.4.

### 7. (task 7.xlsx)
Placeholder / in-progress worksheet.

## Tools
- Microsoft Excel (pivot tables, formulas: engagement rate, uplift, ROI, rolling averages)

## Notes
- Data is synthetic/sample data used for analytics practice, not real Apple performance data.
- Some intermediate sheets (e.g. `task 4.4`, `task 6.1`–`6.3`) contain pivot tables built from the `Engagement Summary` / `Posts` sheets in the same workbook.
