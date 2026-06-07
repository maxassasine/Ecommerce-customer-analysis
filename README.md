# Olist E-Commerce Customer Analysis

Analysis of Brazilian e-commerce customer behaviour using transactional data
from the Olist marketplace (2016–2018).

**Dataset:** 99,441 customers | R$ 16.0M revenue | 27 states | 112,650 order items

---

## Critical Finding

> **0% repeat purchase rate across 99,441 customers.**
> Every customer made exactly one purchase during the observation window.
> All revenue is driven purely by new acquisition — no retention is occurring.

---

## Key Insights

| Finding | Detail |
|---------|--------|
| Revenue growth | 24x growth in 13 months (Oct 2016 → Nov 2017) |
| Black Friday peak | R$ 987,648 in November 2017 |
| Top category | Health & Beauty — R$ 1,258,681 |
| Top state | São Paulo — R$ 5.0M+ (dominates all other states) |
| Delivery performance | Avg actual: 11.8 days vs estimated: 23.3 days |
| Early deliveries | 93.5% of orders delivered ahead of schedule |
| CLV segments | High / Mid / Low Value — evenly distributed (~33% each) |

---

## Analysis Performed

- **Customer Lifetime Value (CLV)** — quantile-based segmentation into High, Mid, Low value tiers
- **Category Performance** — AOV and revenue ranking across all product categories
- **Repeat Purchase Analysis** — customer-level order count distribution
- **Geographic Distribution** — state-level revenue and customer concentration
- **RFM Scoring** — Recency, Frequency, Monetary analysis
  - *Note: Frequency = 1 for all customers on this dataset; segmentation driven by R and M only*
- **Monthly Revenue Trend** — growth trajectory and seasonality identification
- **Delivery Analysis** — actual vs estimated delivery days across 95,956 orders

---

## Business Recommendations

1. **Retention programme** — post-purchase email sequence (Day 3, 7, 14, 30) + loyalty programme
   - Target: convert 15% of one-time buyers to repeat customers
   - Estimated impact: +15–20% revenue
2. **Geographic expansion** — pilot campaigns in Bahia, Ceará, Pernambuco
   - Estimated impact: +10–15% new customer base
3. **Category cross-sell** — Health & Beauty ↔ Watches & Gifts targeting
   - Estimated impact: +8–12% average order value
4. **Segment personalisation** — VIP treatment for High Value, vouchers for Mid, trials for Low

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| Python (pandas, numpy) | Data cleaning, transformation, scoring |
| SQLite (in-memory) | 7 SQL queries for aggregation and analysis |
| Matplotlib / Seaborn | Static visualisations |
| Plotly | Interactive HTML charts |
| Jupyter Notebook | Analysis environment |

---

## Files

| File | Description |
|------|-------------|
| `E-Commerce.ipynb` | Complete analysis notebook |
| `1_segment_distribution.png` | CLV customer segment pie chart |
| `2_top_categories.png` | Top 10 categories by revenue |
| `4_geographic_distribution.png` | Top 10 states by revenue |
| `chart1_monthly_revenue.html` | Interactive monthly revenue trend |
| `chart2_rfm_segments.html` | Interactive RFM segment distribution |
| `chart3_delivery_time.html` | Interactive delivery time histogram |
| `chart4_clv_segments.html` | Interactive CLV segment donut chart |

---

## Conclusion

The analysis reveals a business with strong acquisition momentum — 24x revenue
growth in 13 months — but a complete absence of retention. Delivery performance
is excellent (93.5% early), yet repeat purchases remain at zero, suggesting that
speed alone does not drive loyalty. The primary opportunity is a structured
post-purchase retention programme targeting conversion of one-time buyers into
repeat customers.
