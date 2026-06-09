# british-airways-data-analysis-

# ✈️ British Airways Terminal 3 — Lounge Eligibility Analysis

A data science project analysing British Airways' summer flight schedule to model lounge demand, forecast revenue, and deliver actionable recommendations for Terminal 3 lounge operations.

> Built as part of the **British Airways Data Science Virtual Experience** on Forage.

---

## 📋 Project Overview

British Airways serves thousands of passengers daily from Terminal 3. Not all passengers are equal when it comes to lounge access — eligibility depends on cabin class and loyalty tier. This notebook answers the core operational question:

**How many passengers are eligible for each lounge tier, when do they arrive, and what is the financial impact?**

---

## 🗂️ Contents

```
british_airways_terminal_3_analysis.ipynb   # Main analysis notebook
ba_lounge_analysis.png                      # Dashboard of 6 visualisations
Executive_Summary.txt                       # One-page executive justification
British Airways Summer Schedule Dataset...  # Output Excel workbook (multi-sheet)
```

---

## 🔍 Analysis Steps

| Step | Description |
|------|-------------|
| 1 | **Data Loading** — Import the BA summer schedule CSV |
| 2 | **Exploratory Data Analysis** — Shape, nulls, data types, unique flights |
| 3 | **Categorical Summaries** — Aggregate by haul type, time of day, and arrival region |
| 4 | **Tier Percentage Calculations** — Compute eligibility rates for Tier 1/2/3 |
| 5 | **Lookup Table** — Mean passengers by Haul × Time-of-Day combination |
| 6 | **Hourly Demand Analysis** — Identify peak hours for lounge usage |
| 7 | **Revenue & Cost Modelling** — Daily and annual P&L per tier |
| 8 | **Visualisations** — Six-panel dashboard covering all key dimensions |

---

## 🏷️ Lounge Tier Definitions

| Tier | Lounge | Access Basis | Revenue Rate |
|------|--------|-------------|-------------|
| **Tier 1** | Concorde Room | First Class cabin | £90 / pax |
| **Tier 2** | First / Gold Lounge | Business Class + Gold status | £55 / pax |
| **Tier 3** | Club Lounge | Premium Economy + Silver status | £30 / pax |

Operating cost: **£19.80 per passenger**

---

## 📊 Key Findings

- **Peak demand:** 07:00–08:00 with ~1,280 lounge users in a single hour
- **Tier 2 utilisation:** Running at 100% capacity — expansion needed
- **Model accuracy:** Predictions within 3% of actual BA data (Long-haul: predicted 41%, actual 43.9%)
- **Annual profit (current):** ~£262.8 million

### Recommendations

- ✅ **Build** a Tier 1 Concorde Room — projected 2-month payback period; £52m/year return on a £7–10m investment
- ✅ **Expand** Tier 2 capacity by at least 30%
- ✅ **Implement** dynamic staffing to save ~£500k/year
- 📈 **Total potential with investments:** ~£326.8m annual profit

---

## 🛠️ Tech Stack

```python
pandas       # Data wrangling and aggregation
numpy        # Numerical operations
matplotlib   # Chart generation
seaborn      # Styling
```

Developed in **Google Colab**.

---

## 🚀 Getting Started

1. Clone or download this repository
2. Open `british_airways_terminal_3_analysis.ipynb` in Jupyter or Google Colab
3. Upload the BA Summer Schedule CSV when prompted
4. Run all cells top to bottom

---

## 📄 Outputs

After running the notebook you will have:

- **`ba_lounge_analysis.png`** — A 6-chart dashboard (lounge demand by haul, eligibility by time of day, tier distribution, hourly demand curve, top 10 regions, daily revenue by tier)
- **Excel workbook** with sheets: `full_sheet`, `lookup_table`, `summary_haul`, `summary_time`, `arrival_region`, `summary_hours`
- **`Executive_Summary.txt`** — A plain-text executive brief ready for stakeholder sharing

---

## 👤 Emmanuel.j.Lelo 

Data Science Virtual Experience — British Airways × Forage

