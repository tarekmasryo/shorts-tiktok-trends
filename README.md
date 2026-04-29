# 🎬 Short Video Trends 2025 — YouTube Shorts & TikTok EDA

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](#)
[![Notebook](https://img.shields.io/badge/Format-Jupyter%20Notebook-orange)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A practical exploratory analysis of short-form video trends across platforms, countries, creators, hashtags, devices, traffic sources, and time.

---

## 📌 What’s inside

- 📓 A polished EDA notebook:
  - `short-video-youtube-tiktok-trends-eda.ipynb`
- 📊 Analysis across:
  - platforms
  - countries
  - creators
  - hashtags
  - devices
  - traffic sources
  - posting time and monthly trends
- 📈 Practical visualizations for heavy-tailed engagement and view metrics.
- 🧭 Portable data loading for Kaggle and local runs.
- 🧱 Lightweight repo layout with `data/raw/`, `artifacts/`, and helper utilities.

---

## 📂 Dataset

**Main file:** `youtube_shorts_tiktok_trends_2025.csv`

The dataset is structured for short-video analytics and includes platform-style performance metrics plus creator, content, timing, device, traffic-source, and engagement fields.

Core groups covered:

| Group | Examples |
|---|---|
| Performance metrics | `views`, `likes`, `comments`, `shares`, `saves`, `dislikes` |
| Engagement metrics | `engagement_rate`, ratios, velocity-style signals |
| Platform and geography | `platform`, `country` |
| Creator and content | creator/channel fields, hashtags, category, language |
| Timing | publish date, upload hour, monthly trend fields |
| Context | device type, device brand, traffic source, season, content style |

> The raw CSV is not committed to this repository. For local runs, place it under `data/raw/`.

---

## 🧭 Notebook structure

The notebook follows a clear EDA flow:

1. **Setup & imports**
2. **Data loading**
3. **Basic information and data health checks**
4. **Feature engineering**
5. **Platform, country, creator, hashtag, and timing analysis**
6. **Creator concentration analysis**
7. **Segmentation views by device, category, language, traffic source, and content style**
8. **Key takeaways and next-step recommendations**

---

## 🚀 Run locally

Create an environment and install the dependencies:

```bash
python -m venv .venv
```

Activate it:

```bash
# Windows
.venv\Scripts\activate
```

```bash
# macOS/Linux
source .venv/bin/activate
```

Install requirements:

```bash
pip install -r requirements.txt
```

Then place the dataset here:

```text
data/raw/youtube_shorts_tiktok_trends_2025.csv
```

Open the notebook and run it top to bottom.

---

## 🧪 Run on Kaggle

1. Open the notebook on Kaggle.
2. Add the dataset from the Kaggle sidebar.
3. Run:

```text
Restart Session
Run All
Save Version
```

The notebook searches for the CSV inside `/kaggle/input` automatically, so it does not depend on a hard-coded Kaggle folder name.

---

## 📊 Key analysis areas

- 🌍 Country and platform coverage
- 📱 Device and traffic-source breakdowns
- 🏷️ Hashtag and creator views
- ⏱️ Upload-hour and monthly trend behavior
- 📈 Heavy-tailed view and engagement distributions
- 🧮 Creator concentration in total views
- 🧩 Segmentation angles for dashboard and modeling follow-up

---

## ✅ Key takeaways

- The dataset provides a broad short-video analytics view across platforms, countries, creators, hashtags, devices, traffic sources, and timing dimensions.
- Core schema and data health checks confirm that the main analytical fields are available and suitable for exploratory analysis.
- Engagement and view metrics are heavy-tailed, so log-scaled views and clipped distributions improve readability and interpretation.
- Creator-level views are distributed across a broader creator base rather than following an extreme 80/20 concentration pattern.
- Platform activity and views evolve monthly, making the dataset suitable for trend-monitoring dashboards.
- Device, upload-hour, category, language, season, traffic-source, and content-style fields provide practical segmentation angles.

---

## 🗂️ Repository layout

```text
.
├── short-video-youtube-tiktok-trends-eda.ipynb
├── data/
│   └── raw/
│       └── .gitkeep
├── artifacts/
│   └── .gitkeep
├── repo_utils/
│   ├── __init__.py
│   └── pathing.py
├── CASE_STUDY.md
├── CHANGELOG.md
├── requirements.txt
├── LICENSE
└── README.md
```

---

## 🧠 Follow-up ideas

- Build an interactive Streamlit dashboard with filters for platform, country, category, creator tier, and time period.
- Add a baseline model for high-engagement trend classification.
- Create reusable reporting views for creator, country, and platform comparisons.
- Export selected tables and figures into `artifacts/` for downstream dashboards or presentations.

---

## 📄 License

MIT License. See [LICENSE](LICENSE) for details.

Copyright © Tarek Masryo.
