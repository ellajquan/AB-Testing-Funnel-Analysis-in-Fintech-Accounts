# Email A/B Framework for Boosting Bank Funding Activation in Fintech Accounts

> **Objective** – Identify the email strategy (template × segment × schedule) that maximises  
>  • **Open-rate**  
>  • **Bank-link rate**  
>  • **First-funding rate**  
>  • Down-funnel **activation** (1–2+ trades) Measures how many users make it through each ordered step (e.g., Open → Link → Fund) 
> 480 k unfunded fintech users, 12 behavioural segments, 10 email templates, 2 delivery frequencies, 5-week A/B campaign.
Designed and executed a 480 k user email A/B framework, running 24 treatment cells across 10 templates; applied χ² and CUPED methods to detect a +14 pp lift in open-rate and a +1.9 pp lift in first-funding versus matched controls. Built end-to-end data-manipulation & visualization pipeline in Python (pandas, seaborn, plotly) that aggregated >25 M email-event rows into dynamic dashboards, exposing segment-level engagement drivers in real time. Conducted full-funnel analysis—open → link → fund → trade—with cohort retention curves and drop-off heat-maps, pinpointing the “link-to-fund” step as the highest-ROI leverage point for product follow-ups.

---
![funnel](https://github.com/user-attachments/assets/9289cb88-7f58-4e47-8c4b-8ec94da4b07e)

## Repository layout
```bash
email-funding-experiment/
├── notebooks/              # EDA & visual narrative
├── src/
│   ├── 01_prepare_dataset.py
│   ├── 02_eda_open_rate.py
│   ├── 03_link_fund_models.py
│   ├── 04_time_series.py
│   └── 05_ab_test.py
│   └── 06_funnel_analysis_template-level_lift_latency_curves_causal_forest.py 
├── reports/
│   ├── figures/            # auto-saved plots
│   └── tables/             # final metric tables
└── README.md
```
