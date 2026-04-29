# Case Study — Short Video Trends 2025 EDA

## Problem

Short-form video performance is shaped by platform behavior, creator reach, regional variation, posting time, content style, and engagement quality.

This project turns a short-video analytics dataset into a practical EDA workflow that helps answer:

- Which platforms and countries contribute the most activity and views?
- How do engagement and view metrics behave across different segments?
- Which creator, hashtag, device, and traffic-source patterns are worth monitoring?
- How concentrated are total views across creators?
- What follow-up dashboard or modeling work would be useful?

## Dataset

**Main file:** `youtube_shorts_tiktok_trends_2025.csv`

The dataset uses one row per short-form video and combines:

- platform and country fields
- creator and content fields
- hashtags and category fields
- device and traffic-source fields
- timing fields
- performance and engagement metrics

The notebook is designed to run on Kaggle or locally without changing the core analysis code.

## Approach

The workflow focuses on clear, reusable exploratory analysis:

1. Load the dataset with a portable path resolver.
2. Inspect dataset shape, schema coverage, missingness, duplicates, and core metrics.
3. Prepare numeric metrics and derived fields for analysis.
4. Compare platform, country, creator, hashtag, device, traffic-source, and time-based patterns.
5. Use log-scaled and clipped distributions where heavy-tailed metrics would otherwise be hard to read.
6. Review creator concentration using cumulative view share.
7. Summarize practical takeaways for dashboards and follow-up modeling.

## Main takeaways

- The dataset provides broad coverage across short-video analytics dimensions.
- Engagement and view metrics are heavy-tailed, which makes log-scaled views useful for interpretation.
- Creator-level total views are distributed across a broader creator base rather than showing an extreme 80/20 concentration pattern.
- Country and platform combinations provide useful regional comparison angles.
- Device, upload-hour, category, language, season, traffic-source, and content-style fields support practical segmentation.
- Monthly activity and views make the dataset suitable for trend-monitoring dashboard work.

## Production and portfolio value

This notebook is best positioned as a polished EDA and analytics workflow. It can be extended into:

- a Streamlit dashboard,
- a content trend monitoring report,
- a high-engagement classification notebook,
- reusable creator, country, and platform reporting artifacts.

## Next steps

- Build an interactive dashboard with filters for platform, country, category, creator tier, and time period.
- Add baseline modeling for high-engagement or high-view outcomes.
- Export selected summary tables to `artifacts/`.
- Create a compact report version for non-technical readers.
