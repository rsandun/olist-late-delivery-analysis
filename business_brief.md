# Business Brief: Olist Late Delivery Early-Warning System

## 1. Business context
Olist is a Brazilian online marketplace that connects small sellers with customers. Sellers ship the products, so Olist does not fully control delivery, but its reputation depends on it. The data covers real (anonymised) orders from 2016 to 2018.

## 2. Problem
Late deliveries are likely to cause unhappy customers and lost sales. Operations and Marketing both feel the damage, but nobody knows how big it is, where it is concentrated, or whether it can be predicted early.

## 3. Main question
Which sellers, product categories, and regions lose Olist the most revenue because of delivery problems, can we predict late orders at the time of purchase, and what should Operations and Marketing each do about it?

## 4. Goals
1. Measure how big the delivery problem is.
2. Find where it is concentrated (sellers, categories, states).
3. Show how late delivery affects customer reviews, after checking other causes.
4. Predict which orders will be late using only information known at purchase time.
5. Recommend actions for Operations and Marketing, with estimated money impact.

## 5. Audience
- # Business Brief: Olist Late Delivery Early-Warning System

## 1. Business context
Olist is a Brazilian online marketplace that connects small sellers with customers. Sellers ship the products, so Olist does not fully control delivery, but its reputation depends on it. The data covers real (anonymised) orders from 2016 to 2018.

## 2. Problem
Late deliveries are likely to cause unhappy customers and lost sales. Operations and Marketing both feel the damage, but nobody knows how big it is, where it is concentrated, or whether it can be predicted early.

## 3. Main question
Which sellers, product categories, and regions lose Olist the most revenue because of delivery problems, can we predict late orders at the time of purchase, and what should Operations and Marketing each do about it?

## 4. Goals
1. Measure how big the delivery problem is.
2. Find where it is concentrated (sellers, categories, states).
3. Show how late delivery affects customer reviews, after checking other causes.
4. Predict which orders will be late using only information known at purchase time.
5. Recommend actions for Operations and Marketing, with estimated money impact.

## 5. Audience
- Head of Operations: wants to know which sellers and regions to fix.
- Head of Marketing: wants to know which customers to protect and how much to spend.

## 6. KPI definitions
| KPI | Definition |
|---|---|
| Delivery time (days) | Delivered date minus purchase date |
| Late order | Delivered date is later than the estimated delivery date |
| Late rate | Late orders divided by delivered orders |
| Average delay (days) | Average days late, for late orders only |
| Unhappy customer | Review score of 1 or 2 |
| Unhappy rate | Unhappy customers divided by reviewed orders |
| Revenue | Sum of item prices (freight kept separate) |
| Revenue at risk | Revenue from late orders that received an unhappy review |
| Repeat customer rate | Customers with 2 or more orders divided by all customers (using customer_unique_id) |

## 7. Scope and rules
- Only delivered orders are used for delivery KPIs.
- Currency is Brazilian real (BRL).
- Repeat customers are counted with customer_unique_id, not customer_id.

## 8. Known limits (draft, will update)
- The data is old (2016 to 2018).
- Most customers buy only once, so repeat purchase results will be weak.
- We can show that late delivery goes together with bad reviews, but we cannot fully prove it is the only cause.
- Voucher results are estimates, not a tested result.Head of Operations: wants to know which sellers and regions to fix.
- Head of Marketing: wants to know which customers to protect and how much to spend.

## 6. KPI definitions
| KPI | Definition |
|---|---|
| Delivery time (days) | Delivered date minus purchase date |
| Late order | Delivered date is later than the estimated delivery date |
| Late rate | Late orders divided by delivered orders |
| Average delay (days) | Average days late, for late orders only |
| Unhappy customer | Review score of 1 or 2 |
| Unhappy rate | Unhappy customers divided by reviewed orders |
| Revenue | Sum of item prices (freight kept separate) |
| Revenue at risk | Revenue from late orders that received an unhappy review |
| Repeat customer rate | Customers with 2 or more orders divided by all customers (using customer_unique_id) |

## 7. Scope and rules
- Only delivered orders are used for delivery KPIs.
- Currency is Brazilian real (BRL).
- Repeat customers are counted with customer_unique_id, not customer_id.

## 8. Known limits (draft, will update)
- The data is old (2016 to 2018).
- Most customers buy only once, so repeat purchase results will be weak.
- We can show that late delivery goes together with bad reviews, but we cannot fully prove it is the only cause.
- Voucher results are estimates, not a tested result.# Business Brief: Olist Late Delivery Early-Warning System

## 1. Business context
Olist is a Brazilian online marketplace that connects small sellers with customers. Sellers ship the products, so Olist does not fully control delivery, but its reputation depends on it. The data covers real (anonymised) orders from 2016 to 2018.

## 2. Problem
Late deliveries are likely to cause unhappy customers and lost sales. Operations and Marketing both feel the damage, but nobody knows how big it is, where it is concentrated, or whether it can be predicted early.

## 3. Main question
Which sellers, product categories, and regions lose Olist the most revenue because of delivery problems, can we predict late orders at the time of purchase, and what should Operations and Marketing each do about it?

## 4. Goals
1. Measure how big the delivery problem is.
2. Find where it is concentrated (sellers, categories, states).
3. Show how late delivery affects customer reviews, after checking other causes.
4. Predict which orders will be late using only information known at purchase time.
5. Recommend actions for Operations and Marketing, with estimated money impact.

## 5. Audience
- Head of Operations: wants to know which sellers and regions to fix.
- Head of Marketing: wants to know which customers to protect and how much to spend.

## 6. KPI definitions
| KPI | Definition |
|---|---|
| Delivery time (days) | Delivered date minus purchase date |
| Late order | Delivered date is later than the estimated delivery date |
| Late rate | Late orders divided by delivered orders |
| Average delay (days) | Average days late, for late orders only |
| Unhappy customer | Review score of 1 or 2 |
| Unhappy rate | Unhappy customers divided by reviewed orders |
| Revenue | Sum of item prices (freight kept separate) |
| Revenue at risk | Revenue from late orders that received an unhappy review |
| Repeat customer rate | Customers with 2 or more orders divided by all customers (using customer_unique_id) |

## 7. Scope and rules
- Only delivered orders are used for delivery KPIs.
- Currency is Brazilian real (BRL).
- Repeat customers are counted with customer_unique_id, not customer_id.

## 8. Known limits (draft, will update)
- The data is old (2016 to 2018).
- Most customers buy only once, so repeat purchase results will be weak.
- We can show that late delivery goes together with bad reviews, but we cannot fully prove it is the only cause.
- Voucher results are estimates, not a tested result.