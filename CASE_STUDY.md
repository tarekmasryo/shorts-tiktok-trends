# 🧠 Case Study — YouTube Shorts & TikTok Trends 2025 (EDA)

## Problem
Turn a “one row per video” short‑form dataset into **decision-ready insights** about:
- what drives engagement,
- how trends evolve over time,
- where performance differs by platform, country, creator, and device.

## Data
- **File:** `youtube_shorts_tiktok_trends_2025.csv`
- **Grain:** one row per short video
- **Signals:** views, likes, comments, shares, saves, dislikes + contextual fields (platform, country, device, hashtags, creator)

Local + Kaggle loading is handled via `repo_utils/pathing.py` to keep the notebook portable.

## Approach
- **Schema sanity checks:** types, missingness, duplicates
- **Feature engineering:** engagement totals/ratios, per‑1k metrics, time buckets
- **EDA views:**
  - Distributions with log scaling for heavy tails
  - Correlations across engagement signals
  - Coverage matrix (**Country × Platform**)
  - Monthly momentum (growth, cumulative curves)
  - Leaderboards (creators, hashtags)
  - Pareto analysis (view concentration)

## Key insights (examples)
- Short‑form performance is **heavy‑tailed** (few videos capture most views).
- A small fraction of creators typically drives a large fraction of total reach (Pareto effect).
- Engagement behavior varies by **platform** and **region** (views vs. shares vs. saves).
- Posting time and content categories can correlate with visibility and engagement.

## Decisions & Takeaways
- Use **ranked views + engagement rate** together to avoid “views-only” bias.
- Compare countries/platforms via normalized metrics (per‑1k) for fairer benchmarks.
- Track both **spiky** and **sustained** trends with monthly aggregates.

## Next steps
- Train a baseline model to predict **high-engagement** videos.
- Add additional years to measure multi‑year shifts.
- Convert the notebook into an interactive dashboard (Streamlit / Spaces).
