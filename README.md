# Olist Late Delivery Early-Warning Analysis

**Operations + Marketing analytics project**
Author: Sandun Lakshan Ranathunga

## The question
Which regions and sellers lose Olist the most revenue because of late deliveries, and what should Operations and Marketing each do about it?

## Key findings
- **8.1%** of 96,470 delivered orders arrived after the promised date.
- Late orders are about **6 times more likely to get a bad review** (54.0% vs 9.2%). Average review score: 4.29 on time vs 2.57 late.
- The damage starts after 3 days. Average review score: 3.77 (1-3 days late), 2.32 (4-7 days late), 1.73 (8+ days late).
- Only **5,164 orders** were more than 3 days late, but they hold about **90%** of the revenue at risk (574,359 of 639,252).
- The problem is **regional**. Late rates are highest in AL (23.9%), MA (19.7%), PI (16.0%), CE (15.3%) and SE (15.2%). The north-east five states average 17.4%, against 7.8% elsewhere.
- Product category is **not** the cause. Late orders are much unhappier in all 26 categories with 500+ orders.
- Distance is only a small factor. Orders within one state are late 6.0% of the time, orders between states 9.0%.
- Olist already promises about 7.6 days more in the north-east. The problem is a group of very slow orders, not the average delivery time.

## Recommendations
**Operations**
- Focus on the five north-east states first.
- Track orders still in transit after their expected date, and investigate the slowest 10% of orders with carriers and sellers.
- Put the top sellers by revenue at risk on a watch list.
- Target: no order more than 3 days late.

**Marketing**
- Send an apology message and a small voucher to customers whose order will be more than 3 days late.
- Test it first: send the voucher to half of the late orders, then compare reviews and repeat purchases after 1 to 2 months.

## Voucher scenarios (what-if)
Voucher cost is assumed at 10% of order value (79,956 for the 5,164 late orders).

| Case | Share of at-risk revenue recovered | Net gain |
|---|---|---|
| Worst | 10% | -22,520 |
| Normal | 25% | +63,634 |
| Best | 40% | +149,788 |

The plan breaks even if it recovers about 14% of the at-risk revenue.

## Definitions
- **Late order:** delivered after the estimated delivery date.
- **Unhappy customer:** review score of 1 or 2.
- **Revenue at risk:** item revenue from orders that were late and got an unhappy review.
- Full definitions are in `business_brief.md`.

## Limits
- "Revenue at risk" is not proven lost money. Customers had already paid.
- Recovery rates and voucher cost are assumptions and need a real test.
- The data is from 2016 to 2018, and most customers bought only once, so repeat purchase analysis is weak.
- The results show that late delivery goes together with bad reviews, but other causes (seller, price) were not tested at the same time.
- This data cannot show why the north-east is slow (carrier, seller, or region).

## Project files
- `notebook/03_analysis.ipynb`: full analysis in Python
- `outputs/dashboard.html`: dashboard (open in a browser)
- `outputs/`: chart images
- `business_brief.md`: problem, goals, and KPI definitions

## Data
Brazilian E-Commerce Public Dataset by Olist, on Kaggle (search for the name). The data files are not included in this repository. To rerun the analysis, download the dataset and put the CSV files in a folder called `data`.

## Tools
Python (pandas, matplotlib), HTML/CSS


Built with AI assistance (Claude). I chose the project goal, ran the analysis on my own computer, and wrote the interpretation and recommendations in "My interpretation" myself. Claude wrote most of the code and the rest of the text.