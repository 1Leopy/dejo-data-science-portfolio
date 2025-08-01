# 😊 Customer Satisfaction Analysis

## 🧠 Project Overview
This project explored customer behavior, satisfaction patterns, and key improvement areas based on a dataset of 500 mall customers. The analysis aimed to uncover actionable business insights that can help improve retention, reduce return rates, and boost overall satisfaction.

---

## 🎯 Objectives

1. Identify the key drivers of customer satisfaction or dissatisfaction.
2. Highlight surprising or unexpected findings in the data.
3. Recommend practical business strategies based on insights.

---

## 📄 Dataset Notes

- **ReturnRate:** Ratio of goods returned relative to total purchases (inverse relationship with satisfaction).
- **LoyaltyProgram:** Indicates if a customer is enrolled in a rewards or discount-based loyalty scheme.
- The dataset is sorted by `CustomerID`, which does **not** reflect time-based order.

---

## 👥 Demographic Summary

- **Total Customers:** 500
- **Gender Split:** 53.2% Female, 46.8% Male — a fairly balanced distribution.
- **Age Distribution:**
  - Majority: Adults (35–54)
  - Others: Equal mix of Young Adults (18–34) and Older Adults (55–69)
- **Average Ratings:** Across all satisfaction metrics, average rating was approximately **3/5** — considered average/good.
- **Total Purchase Value:** $532,525.37
- **Loyalty Program Participation:** Slightly above 50% of customers were enrolled.

---

## 🔍 Key Findings

### ✅ Top Drivers of Satisfaction:

- **Delivery Time**
  - Fast delivery positively correlated with **Customer Service Rating** (+0.039)
  - Delays linked to higher **Return Rates** (-0.042), possibly due to unmet expectations or product dissatisfaction upon late arrival.

- **Discount Usage**
  - Encouraged higher spending (correlation with `TotalPurchase`: +0.089)
  - Lowered product return rate (correlation with `ReturnRate`: -0.039)

- **Loyalty Program**
  - Strongly associated with discount usage (correlation: +0.66)
  - Loyalty program users often engage more with promotions, suggesting a strong value loop.

### 😮 Surprising Observation:

- Overall correlations between variables were quite **low or scattered**, indicating complex or non-linear relationships — worth exploring with more advanced modeling in future.

---

## 🛠️ Recommendations for the Business

1. **Improve Delivery Efficiency** — Key to increasing satisfaction and reducing returns.
2. **Boost Discount Offers** — Positively influences both spending and retention.
3. **Expand the Loyalty Program** — Drives discount engagement and builds brand commitment.
4. **Improve Product Quality** — Investigate reasons behind returned products.
5. **Enhance the Website UX/UI** — While weakly correlated, better experience may indirectly boost engagement.
6. **Factor in Customer Volume When Interpreting Results** — For example, gender-based insights should be normalized due to slight female majority.

---

## 🧠 Takeaway

This project demonstrates how EDA, correlation analysis, and a bit of business empathy can go a long way in helping businesses understand their customers. Insights gained here can inform product, logistics, and marketing strategies for a more satisfying customer journey.
