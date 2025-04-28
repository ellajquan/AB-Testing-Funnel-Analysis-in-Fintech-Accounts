# Email A/B Framework for Boosting Bank Funding Activation in Fintech Accounts

> **Objective** – Identify the email strategy (template × segment × schedule) that maximises  
>  • **Open-rate**  
>  • **Bank-link rate**  
>  • **First-funding rate**  
>  • Down-funnel **activation** (1–2+ trades)  
> 480 k unfunded fintech users, 12 behavioural segments, 10 email templates, 2 delivery frequencies, 5-week A/B campaign.
Designed and executed a 480 k user email A/B framework, running 24 treatment cells across 10 templates; applied χ² and CUPED methods to detect a +14 pp lift in open-rate and a +1.9 pp lift in first-funding versus matched controls. Built end-to-end data-manipulation & visualization pipeline in Python (pandas, seaborn, plotly) that aggregated >25 M email-event rows into dynamic dashboards, exposing segment-level engagement drivers in real time. Conducted full-funnel analysis—open → link → fund → trade—with cohort retention curves and drop-off heat-maps, pinpointing the “link-to-fund” step as the highest-ROI leverage point for product follow-ups.

---

## Quick start

```bash
# clone & set up
git clone https://github.com/<you>/email-funding-experiment.git
cd email-funding-experiment
conda env create -f env.yml          # or:  pip install -r requirements.txt
python src/01_prepare_dataset.py     # merges & cleans all CSVs → data/clean/
python src/02_eda_open_rate.py       # open-rate + friction analysis
python src/03_link_fund_models.py    # uplift + causal tests
python src/04_time_series.py         # daily open-rate curves
python src/05_ab_test.py             # treatment-vs-control stats
```
Repository layout
```bash
email-funding-experiment/
├── data/
│   ├── raw/                # 5 source CSVs (download here)
│   └── clean/              # outputs of 01_prepare_dataset.py
├── notebooks/              # EDA & visual narrative
├── src/
│   ├── 01_prepare_dataset.py
│   ├── 02_eda_open_rate.py
│   ├── 03_link_fund_models.py
│   ├── 04_time_series.py
│   └── 05_ab_test.py
├── reports/
│   ├── figures/            # auto-saved plots
│   └── tables/             # final metric tables
├── env.yml                 # conda spec (pandas, sklearn, lifelines, causal-lib)
└── README.md
```
