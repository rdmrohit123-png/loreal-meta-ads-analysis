# 📊 L'Oréal Meta Ads Performance Analysis
### Python · Pandas · Matplotlib · Seaborn · JupyterLab

![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0-lightblue?style=flat-square&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7-orange?style=flat-square)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-teal?style=flat-square)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)

---

## 📈 Visualisations Produced

> 13 charts built across 4 analytical phases — from exploration to strategy.

| Phase | Chart | Type | Key Insight |
|---|---|---|---|
| Phase 1 | ROAS by Campaign | Bar Chart | Revitalift leads at 12.6x |
| Phase 2 | Spend vs Revenue by Campaign | Grouped Bar | All campaigns profitable |
| Phase 2 | ROAS by Target Audience | Horizontal Bar | Women 25–34 top at 10.0x |
| Phase 2 | CTR vs Conversion Rate | Scatter Plot | High CTR ≠ high conversion |
| Phase 2 | ROAS Heatmap — Country × Campaign | Heatmap | Italy + Revitalift = 14.4x |
| Phase 3 | Monthly Spend vs Revenue | Line Chart | Revenue gap widens over time |
| Phase 3 | Monthly ROAS Trend | Line Chart | Stable 7.3x–8.7x range |
| Phase 3 | Monthly CTR vs Conversion Rate | Dual-Axis Line | Metrics diverge in Feb & Apr |
| Phase 3 | Monthly ROAS by Campaign | Multi-Line | Revitalift dominant every month |
| Phase 4 | KPI Dashboard | Metric Cards | €8.2M revenue · 8.1x ROAS |
| Phase 4 | Strategic Recommendations | Visual Slide | 5 budget reallocation actions |

---

## 🧭 Project Overview

This project presents a **full-funnel marketing analytics deep dive** into L'Oréal Group's Meta (Facebook/Instagram) advertising performance across **5 European markets** from **January to May 2024**.

The analysis covers **500 daily ad records** across 5 campaigns, 6 audience segments, and 5 ad formats — examining spend efficiency, audience behaviour, creative performance, and monthly trends to deliver **data-backed strategic recommendations**.

> 🎯 **Business Question:** Which campaigns, audiences, ad formats, and markets are delivering the strongest return on ad spend — and where should L'Oréal reallocate its Meta budget?

---

## 📁 Repository Structure

```
loreal-meta-ads-analysis/
│
├── Loreal_Analytics.ipynb                        # Main Jupyter Notebook
├── loreal_meta_ads_performance_jan_jun_2024.csv  # Dataset (500 rows)
├── README.md                                     # This file
│
└── charts/                                       # All exported visualisations
    ├── roas_by_campaign.png
    ├── spend_vs_revenue.png
    ├── roas_by_audience.png
    ├── ctr_vs_convrate.png
    ├── roas_heatmap.png
    ├── monthly_spend_revenue.png
    ├── monthly_roas.png
    ├── monthly_ctr_convrate.png
    ├── campaign_roas_trend.png
    ├── kpi_dashboard.png
    └── recommendations.png
```

---

## 📦 Dataset Summary

| Field | Detail |
|---|---|
| **Source** | Synthetic Meta Ads dataset modelled on real L'Oréal Group brand structure |
| **Period** | January 2024 – May 2024 |
| **Records** | 500 daily ad performance rows |
| **Columns** | 15 (Date, Campaign, Audience, Country, Impressions, Clicks, Spend, Conversions, Revenue, Likes, Shares, Comments, Ad Format, Product Category) |
| **Campaigns** | Garnier Vitamin C · L'Oréal Men Expert · L'Oréal Paris Revitalift · Maybelline Fit Me · NYX Cosmetics Digital |
| **Markets** | France · Germany · Italy · Spain · UK |
| **Ad Formats** | Video · Carousel · Single Image · Stories · Reels |

---

## 🔑 Key KPIs Tracked

| KPI | Formula | Why It Matters |
|---|---|---|
| **ROAS** | Revenue ÷ Spend | Primary efficiency metric |
| **CTR** | Clicks ÷ Impressions × 100 | Ad creative engagement |
| **CPA** | Spend ÷ Conversions | Cost to acquire one customer |
| **CPM** | Spend ÷ Impressions × 1000 | Reach efficiency |
| **Conversion Rate** | Conversions ÷ Clicks × 100 | Funnel quality |

---

## 📊 Analysis Phases

### Phase 1 — Data Loading, Cleaning & Exploration
- Loaded and validated 500-row dataset
- Converted date formats, checked for nulls and duplicates (0 found)
- Engineered 6 KPI columns (ROAS, CTR, CPA, CPM, Conversion Rate, CPC)
- Generated campaign-level aggregated summary table

### Phase 2 — Campaign & Audience Deep Dive
- Compared spend vs revenue across all 5 campaigns
- Ranked audience segments by ROAS and conversion rate
- Evaluated ad format performance (ROAS, CPA, CTR)
- Built **ROAS Heatmap** across Country × Campaign dimensions

### Phase 3 — Time Trend Analysis
- Aggregated daily data into monthly performance buckets
- Tracked ROAS, CTR and conversion rate month-by-month
- Plotted multi-line campaign ROAS trends to identify consistency vs volatility

### Phase 4 — Insights & Strategic Recommendations
- Built 4-metric KPI dashboard card
- Automated Top & Bottom performer identification
- Produced 5 actionable strategic recommendations with supporting data

---

## 🏆 Key Findings

```
📈 Overall ROAS       :  8.1x  (every €1 spent returned €8.10)
💰 Total Revenue      :  €8,246,863
🎯 Best Campaign      :  L'Oréal Paris Revitalift  — 12.6x ROAS
👥 Best Audience      :  Women 25–34               — 10.0x ROAS
📱 Best Ad Format     :  Stories                   —  9.1x ROAS
🌍 Best Market        :  Italy (Revitalift)         — 14.4x ROAS
⚠️  Underperformer    :  L'Oréal Men Expert         —  4.3x ROAS
```

---

## 💡 Strategic Recommendations

| # | Recommendation | Rationale |
|---|---|---|
| 1 | **Scale Revitalift budget by 20–30%** | 12.6x ROAS consistent across all 5 markets |
| 2 | **Pause or redesign Men Expert creatives** | 4.3x ROAS — below portfolio average |
| 3 | **Double down on Women 25–34 targeting** | 10.0x ROAS · 54,686 total conversions |
| 4 | **Shift budget from Single Image → Stories & Reels** | 9.1x vs 7.0x ROAS gap |
| 5 | **Run geo-targeted push in Italy & France** | Revitalift hits 14.4x and 14.2x ROAS respectively |

---

## 🛠️ Tools & Libraries

```python
import pandas as pd        # Data manipulation & aggregation
import numpy as np         # Numerical computations
import matplotlib.pyplot   # Chart creation
import seaborn as sns      # Heatmaps & statistical plots
```

**Environment:** JupyterLab · Python 3.10 · macOS

---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/loreal-meta-ads-analysis.git
cd loreal-meta-ads-analysis

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# 3. Launch Jupyter
jupyter lab

# 4. Open and run the notebook
# → Loreal_Analytics.ipynb
# → Run All Cells (Kernel → Restart & Run All)
```

---

## 👤 Author

**Rohit Pal**
MSc Digital Marketing & Artificial Intelligence — SKEMA Business School, Paris
Specialising in Marketing Analytics · Performance Marketing · AI-Driven Strategy

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/YOUR_PROFILE)
[![Email](https://img.shields.io/badge/Email-Contact-red?style=flat-square&logo=gmail)](mailto:rdmrohit123@gmail.com)

---

## 📄 Disclaimer

> This project uses a **synthetic dataset** modelled on the structure of real Meta Ads performance data for L'Oréal Group brands. All figures are simulated for educational and portfolio purposes. No proprietary or confidential data has been used.

---

*Built as part of an independent marketing analytics portfolio project · November 2024*
