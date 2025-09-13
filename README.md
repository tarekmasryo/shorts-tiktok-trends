# 🎬 YouTube Shorts & TikTok Trends 2025 — EDA Tutorial  

---

## 📌 Project Overview  
This project explores **short-form video trends** on **YouTube Shorts** and **TikTok** during **2025**.  

The notebook is designed as a **beginner-friendly tutorial** for Exploratory Data Analysis (EDA). It walks through how to load, clean, and explore the dataset while building visual insights into creators, hashtags, platforms, and audience behaviors.  

---

## 📊 Dataset  
**File:** `youtube_shorts_tiktok_trends_2025.csv`  

Includes trend-level data across YouTube Shorts & TikTok:  
- 📹 Video metadata: title, category, language, duration, upload hour.  
- 📈 Performance: views, likes, comments, shares, saves, dislikes.  
- 🔄 Engagement metrics: engagement rate, like/share/save ratios, velocity, completion.  
- 🌍 Context: country, platform, device type, device brand, event season, hashtags, creator/channel.  

---

## 🔧 Methodology (Step-by-Step)  

**1. Data Cleaning & Prep**  
- Inspect dataset size (rows × columns), dtypes, missing values, duplicates.  
- Standardize schema and convert numeric types.  
- Derive engagement metrics (total engagement, rates, per-1k metrics).  
- Create time buckets (monthly aggregates).  

**2. Exploratory Analysis**  
- Correlation heatmaps of engagement metrics.  
- Distribution plots (views, duration, engagement rates).  
- Coverage matrix: **Country × Platform**.  
- Monthly views: trends, percentage change, cumulative curves.  
- Leaderboards: top creators, top hashtags, Pareto (80/20 rule).  

**3. Visualization & Storytelling**  
- Bar, line, pie, violin, and scatter plots.  
- Highlight differences across platforms, countries, devices, and content styles.  
- Show heavy-tailed distributions with log scaling for clarity.  

**4. Insight Extraction**  
- Which platforms dominate views in 2025.  
- Engagement patterns (likes, shares, saves, comments).  
- How few creators drive the majority of views (Pareto effect).  
- Differences by country, device type, posting hour, category, and language.  
- Distinction between short-lived vs. sustained viral trends.  

---

## 🧠 Features Examined  
- **Core metrics:** views, likes, comments, shares, saves, dislikes.  
- **Engagement ratios:** engagement rate, like/share/save rates, engagement per 1k views.  
- **Temporal features:** publish date, year-month, trend duration, engagement velocity.  
- **Contextual features:** country, platform, device type, device brand, category, language, event season.  
- **Content style:** title length, emoji presence.  

---

## 📈 Results & Insights (Examples)  
- **Heavy-tailed distributions:** Most views are concentrated in a small set of viral videos.  
- **Pareto principle:** ~20% of creators drive ~80% of total views.  
- **Platform dynamics:** Engagement rates differ noticeably between YouTube Shorts and TikTok.  
- **Country & platform coverage:** Adoption is uneven across regions, some countries skew heavily to one platform.  
- **Behavioral patterns:** Posting hour, device type, and content category affect visibility and engagement.  
- **Trend life cycle:** Some topics spike fast but fade quickly, others show slower, sustained momentum.  

---

## 🗺️ Visual Gallery  
- 📊 Dataset size overview (rows × columns, top countries).  
- 🔥 Monthly views & growth trends.  
- 🎭 Engagement rate distributions (boxplots & violin).  
- 🌍 Country × Platform heatmaps.  
- 🏆 Top creators and hashtags leaderboards.  
- 📈 Pareto curve (creators vs. views).  
- 📱 Device & traffic source breakdowns.  
- ✍️ Title length & emoji impact on engagement.  

---

## 💡 Next Steps  
- Build a simple model to predict **high-engagement trends**.  
- Add more years of data to track multi-year dynamics.  
- Explore cross-platform **recommendation patterns**.  
- Create interactive dashboards (Streamlit / HuggingFace Spaces) for deeper exploration.  

