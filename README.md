# 📉 Sales Decline Root-Cause Analysis

A one-page Power BI dashboard that investigates a sharp 69% year-over-year sales drop and traces it down to its true root cause — separating a real business problem from a false alarm.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-217346?style=for-the-badge&logo=microsoft&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

---

## ❓ Problem

Company-wide sales in **March 2015 were down 69%** compared to March 2014 ($32.9K → $10.3K) — the single largest month-over-month drop across the entire 2014–2017 dataset, despite the company growing steadily overall ($484K → $733K over the same period). A drop this size, taken at face value, would normally trigger a serious business review.

## 🔍 Investigation

Rather than reporting the number as-is, I drilled down step by step to isolate the actual cause:

1. **Region check** → Central, East, and West sales were flat or growing. Only **South** region had dropped.
2. **Category check** → Within South, Furniture and Office Supplies were stable. Only **Technology** had collapsed, falling **-98%** ($28.5K → $528).
3. **Order-level check** → Discount rate stayed identical (20% both years). Order count barely moved (5 orders → 2 orders) — too small a change to explain a 98% revenue drop on its own.

## ✅ Root Cause & Solution

The 2014 figure was inflated by a **small number of unusually large one-off orders** that simply didn't recur in 2015. This wasn't a decline in demand, fewer customers, or a pricing issue — it was a **small-sample statistical artifact**, correctly identified and explained instead of being escalated as a false crisis.

**Recommendation:** No corrective action needed on the March 2015 numbers. Since South Technology revenue depends heavily on a handful of large transactions, that segment's monthly figures should be monitored going forward.

---

## 🖼️ Dashboard

![Dashboard](Main.png)

- **Regional Sales Comparison (Mar 2014 vs 2015)** — isolates South as the only declining region
- **South Region — Sales by Category** — isolates Technology as the only declining category
- **South Technology — Order Details** — shows order count and discount rate barely changed
- **Monthly Sales Trend (2014–2017)** — confirms the business grew steadily overall
- **South Region — March Sales Summary** — raw before/after totals

---

## 🛠️ Tools Used

Power BI Desktop · Power Query · DAX · [Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final) (Kaggle)

## ⚠️ Limitations

- The affected segment had a very small sample size (5 vs 2 orders) — this finding shouldn't be generalized to higher-volume categories
- No customer-level ID to confirm if the same client placed the large 2014 orders — this is an inference based on order value, not a confirmed match

---

## 🚀 How to View

1. Download Link [**sales_drop_analysis.pbix**](https://github.com/Sushrut001/Sales-Decline-Root-Cause-Analysis/blob/main/powerbi.pbix)
2. Open in [Power BI Desktop (free)](https://www.microsoft.com/en-us/power-platform/products/power-bi/downloads)

No Power BI installed? Just view the screenshot above.

---

## 🙌 Contact

📩 [sushrutworks@gmail.com](mailto:sushrutworks@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/sushrutt/)
💻 [Portfolio](https://sushrut-portfolio.netlify.app/)
