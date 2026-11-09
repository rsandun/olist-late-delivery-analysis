# Olist Late Delivery Impact Analysis

**Operations + marketing analytics project**  
Author: Sandun Lakshan Ranathunga

How do late deliveries affect customers and revenue at a Brazilian online marketplace, and what should Operations and Marketing each do about it?

![Dashboard overview](dashboard_overview.png)

## Summary
Only 8.1% of delivered orders arrive late, but those orders produce most of the unhappy customers. A late order is about 6 times more likely to get a bad review (54.0% vs 9.2%). About 5,000 orders that are more than 3 days late hold roughly 90% of the revenue at risk. The problem is worst by rate in the north-east of Brazil, and biggest in money in São Paulo and Rio de Janeiro.

## Key findings
1. **Late delivery hurts reviews.** Average review score is 4.29 for on-time orders and 2.57 for late orders. Late orders are unhappier in all 26 product categories with 500+ orders, so product type is not the cause.
2. **The damage starts after 3 days.** Average review score: 3.77 (1-3 days late), 2.32 (4-7 days late), 1.73 (8+ days late).
3. **Few orders carry most of the risk.** Revenue at risk is 639,252 (4.8% of 13.2 million). Of that, 574,359 comes from just 5,164 orders that were more than 3 days late.
4. **By rate, the north-east is worst.** Late rates: AL 23.9%, MA 19.7%, PI 16.0%, CE 15.3%, SE 15.2%. These five states average 17.4% late, against 7.8% elsewhere.
5. **By money, São Paulo and Rio de Janeiro matter most.** They hold about half of the revenue at risk (SP 169,918 and RJ 153,947), because they have far more orders.
6. **The north-east problem is slow orders, not slow averages.** Olist already promises about 7.6 days more there (31.1 vs 23.5 days). Orders arrive 9.6 days early on average, yet 17.4% are late, so a group of very slow orders is the cause.
7. **Distance is a small factor.** Orders inside one state are late 6.0% of the time, orders across states 9.0%.
8. **Late rate peaks in busy months:** March 2018 (21.4%), February 2018 (16.0%) and November 2017 (14.3%).

## Charts

**Review score by delay.** The score falls with every extra day, and drops sharply after 3 days.

![Review score by delay](1_review_by_delay.png)

**Late rate by state.** The north-east states are the highest.

![Late rate by state](2_late_by_state.png)

**Late rate by category.** All categories are close together, so product type is not the cause.

![Late rate by category](3_late_by_category.png)

**Top sellers by revenue at risk.** Seller IDs are anonymised in the dataset.

![Top sellers by revenue at risk](4_sellers_at_risk.png)

**Late rate by month.** Peaks in March 2018, February 2018 and November 2017.

![Late rate by month](5_late_by_month.png)

**Revenue at risk by state.** São Paulo and Rio de Janeiro hold about half of it, because they have the most orders.

![Revenue at risk by state](6_risk_by_state.png)

**Promised vs real delivery time.** Olist already promises longer in the north-east, so a longer promise is not the fix.

![Promised vs real delivery time](7_promised_vs_real.png)

**Share of orders vs share of revenue at risk.** Orders more than 3 days late are a small share of orders but most of the risk.

![Share of orders and revenue at risk by delay group](8_risk_share_by_delay.png)

**Voucher scenarios.** The plan loses money in the worst case and gains in the normal and best cases. The recovery rates are assumptions.

![Voucher scenarios](9_voucher_scenarios.png)

## Recommendations
**Operations**
- Start with the five north-east states for rate, and with São Paulo and Rio de Janeiro for money.
- Track orders still in transit after their expected date, and investigate the slowest 10% of orders with carriers and sellers.
- Put the top sellers by revenue at risk on a watch list.
- Target: no order more than 3 days late.

**Marketing**
- Send an apology message and a small voucher to customers whose order will be more than 3 days late.
- Test it first: send the voucher to half of those orders, then compare reviews and repeat purchases after 1 to 2 months.

## Voucher scenarios (what-if)
The voucher is assumed to cost 10% of order value (79,956 for the 5,164 orders). The recovery rates are assumptions, not results.

| Case | Share of at-risk revenue recovered | Net gain |
|---|---|---|
| Worst | 10% | -22,520 |
| Normal | 25% | +63,634 |
| Best | 40% | +149,788 |

The plan breaks even if it recovers about 14% of the at-risk revenue.

## Definitions
| Term | Meaning |
|---|---|
| Late order | Delivered after the estimated delivery date |
| Unhappy customer | Review score of 1 or 2 |
| Revenue at risk | Item revenue from orders that were late and got an unhappy review |
| Delivered orders | Orders with status "delivered" and a delivery date |

More definitions are in `business_brief.md`.

## Limits
- "Revenue at risk" is not proven lost money. Customers had already paid.
- Recovery rates and voucher cost are assumptions and need a real test.
- The data is from 2016 to 2018, and most customers bought only once, so repeat-purchase analysis is weak.
- Late delivery goes together with bad reviews, but other causes (seller, price) were not tested at the same time.
- The data cannot show why the north-east is slow (carrier, seller, or region).
- Data cleaning was light. There was no deep check for duplicates or unusual values.

## Project files
| File / Folder | What it is |
|---|---|
| `03_analysis.ipynb` & `01_data_check.ipynb` | Full analysis notebooks |
| `dashboard.html` | Interactive dashboard (download it and open it in a browser) |
| `business_brief.md` | Problem, goals, and KPI definitions |
| `executive_summary.md` | One-page summary for managers |

## How to rerun
1. Download the Brazilian E-Commerce Public Dataset by Olist from Kaggle. Check its license there.
2. On your computer, make a project folder containing a `data` subfolder for the CSVs.
3. Put the notebooks and CSV files in place, adjusting your notebook data read path if necessary.
4. Install the tools: `pip install pandas matplotlib`
5. Open `03_analysis.ipynb` and click **Run All**.

The data files are not included in this repository.

## Tools
Python (pandas, matplotlib), HTML/CSS

---

