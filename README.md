# 🍔 QuickBite Express Crisis Analysis Dashboard

> 📊 A Power BI dashboard built to understand how a business crisis hit QuickBite Express — a food delivery startup — across revenue, customer behavior, restaurant performance, delivery operations, and customer sentiment.

---

## 📌 Project Overview

QuickBite Express is a Bengaluru-based food-tech startup (founded in 2020) that connects customers with nearby restaurants and cloud kitchens. In June 2025, QuickBite faced a major crisis. A viral social media incident involving food safety violations at partner restaurants, combined with a week-long delivery outage during the monsoon season, triggered massive customer backlash. Competitors capitalized with aggressive campaigns, worsening the situation.

This dashboard pulls together the operational, financial, and customer-side data into one report so the business could actually see what happened and where to focus recovery efforts, instead of guessing.

---

## 🎯 What Management Needed to Know

- 📉 How badly did revenue and order volume actually drop?
- 👥 Which customers were affected the most?
- 🍽️ Which restaurant partners took the biggest hit?
- 🚚 Did delivery performance and SLA compliance fall apart?
- ⭐ How did ratings and sentiment change over time?
- 💡 Where should recovery efforts be focused first?

---

## 🔍 Findings

### 📉 1. Monthly Orders: Compare total orders across pre-crisis (Jan–May 2025) vs crisis (Jun–Sep 2025). How severe is the decline? 

Orders were steady through the first five months of 2025, then dropped sharply from June onward and stayed down. Total orders went from **114K (pre-crisis)** to **35K (crisis)** — a decline of nearly **70%**.

The drop wasn't a blip — it held through the rest of the observed period, which suggests customer trust didn't come back quickly on its own.

---

### 🌍 2. Which top 5 city groups experienced the highest percentage decline in orders during the crisis period compared to the pre-crisis period?

<img width="502" height="222" alt="image" src="https://github.com/user-attachments/assets/ca781cbf-66d6-406a-88b4-b2ccf256b3d2" />


Bengaluru recorded the highest decline (70.23%), closely followed by Mumbai, Ahmedabad, Pune, and Delhi. The small variation between cities indicates the crisis impacted the platform consistently across all major markets.

---

### 🍽️ 3. Among restaurants with at least 50 pre-crisis orders, which top 10 high-volume restaurants experienced the largest percentage decline in order counts during the crisis period? 

<img width="552" height="257" alt="image" src="https://github.com/user-attachments/assets/ed5c00c2-f109-4d0e-b41c-a56b34a1cdee" />


Royal Curry Mahal was the most affected restaurant, with a 94% decline in orders. Overall, the top-performing restaurants experienced declines ranging from 83% to 94%, indicating that the crisis had a severe impact on restaurant partners across the platform.


---

### ❌ 4. Cancellation Analysis: What is the cancellation rate trend pre-crisis vs crisis, and which cities are most affected? 

Cancellation rate nearly doubled, from **6.1%** pre-crisis to **11.9%** during the crisis, and the increase was consistent across every city:

<img width="477" height="265" alt="image" src="https://github.com/user-attachments/assets/f4ffc69c-87b8-4632-90b2-a3d0b0f2bc1a" />


The cancellation rate increased across every city during the crisis, with Bengaluru (7.19%), Kolkata (7.14%), and Chennai (7.04%) recording the highest rates. The consistent rise across all locations suggests that the increase was driven by platform-wide operational issues rather than isolated city-specific problems.

---

### 🚚 5. Delivery SLA: Measure average delivery time across phases. Did SLA compliance worsen significantly in the crisis period?

<img width="592" height="266" alt="image" src="https://github.com/user-attachments/assets/97808a09-3866-4ffd-86bc-42ed5ae6fa13" />

SLA compliance declined in the crisis period , noticeably:

- Average delivery time went from **39.5** to **60.1 minutes**
- SLA compliance dropped from **43.6%** to **12.2%**
- Average delivery delay rose from **2 minutes** to **17.6 minutes**


Slower deliveries and worse SLA compliance line up exactly with the rise in cancellations and drop in ratings — this looks like the main operational driver behind the crisis.

---

### ⭐ 6. Ratings Fluctuation: Track average customer rating month-by-month. Which months saw the sharpest drop?

<img width="492" height="233" alt="image" src="https://github.com/user-attachments/assets/f536e84d-615c-4349-adcb-5a4b5ffdfc9a" />


Customer ratings remained consistently above **4.3** before the crisis but dropped sharply to **2.6** in **June** and continued to decline, reaching **2.3(lowest)** by **September**. The sudden fall aligns with the onset of the crisis, indicating a significant decline in customer satisfaction.

---

### 💬 7. Sentiment Insights: During the crisis period, identify the most frequently occurring negative keywords in customer review texts. (Hint: Use a Word Cloud visual in Power BI to visualize the findings.) 

<img width="392" height="463" alt="image" src="https://github.com/user-attachments/assets/502a3f07-9632-4292-bdec-0620f8c782d3" />

The most common customer complaint was that food **"could be hotter" (4,814 mentions)**, followed by concerns about **food quality, food safety, cold food, pricing, and packaging**. The feedback suggests that product quality and order experience were the primary drivers of customer dissatisfaction during the crisis.

---

### 💰 8. Revenue Impact: Estimate revenue loss from pre-crisis vs crisis (based on subtotal, discount, and delivery fee). 

| Metric             | Value |
|--------------------|--------|
| Pre-Crisis Revenue | **₹37.6M** |
| Crisis Revenue     | **₹10.9M** |
| Revenue Loss       | **₹26.7M** |
| Revenue Decline    | **70.9%**  |

Revenue fell by over **71%** during the crisis, dropping from **₹37.6M** to **₹10.9M**. The decline reflects the combined impact of lower customer demand, higher cancellations, and reduced business activity.

---

### 👥 9. Loyalty Impact: Among customers who placed five or more orders before the crisis, determine how many stopped ordering during the crisis, and out of those, how many had an average rating above 4.5? 

Active customers declined from **87K** before the crisis to **32K** during the crisis, a decrease of **62.7%**. Along with the **68.9%** drop in total orders, this suggests that the crisis affected not only new customer acquisition but also the existing customer base, resulting in lower customer engagement and retention.

---

### 🔬 10. Customer Lifetime Decline: Which high-value customers (top 5% by total spend before the crisis) showed the largest drop in order frequency and ratings during the crisis? What common patterns (e.g., location, cuisine preference, delivery delays) do they share?

The crisis also impacted the platform's most engaged customers. Active customers in the **high-value** segment **dropped from 4K to 1K (70.8%)**, while only **23 customers were retained**. Several customers with five or more pre-crisis orders placed no orders during the crisis.

---

## 💡 What I'd Recommend

**🚚 Fix delivery first.** This is where most of the damage traces back to — better partner allocation during peak hours, route optimization, real-time delay alerts for the ops team.

**🤝 Win back trust directly.** Compensate customers who were affected by delays or cancellations, be upfront about what's being fixed, and get customer support response times down.

**🍽️ Support restaurant partners**, especially the ones that lost the most — promotional support, regular quality checks, and help with prep-time efficiency.

**📦 Cut down cancellations** by flagging high-risk orders before they happen, giving customers better order tracking, and proactively notifying them when something's delayed instead of leaving them to find out.

**💬 Keep watching feedback in real time** — ratings and sentiment, not just after the fact, so the next issue gets caught before it turns into another crisis.


---

# 🖼️ Dashboard Preview

## 📈 Executive Summary
<img width="1433" height="802" alt="image" src="https://github.com/user-attachments/assets/091fb7f3-da53-4210-8112-7f1cf65e1fae" />


## 👥 Customer Insights
<img width="1423" height="797" alt="image" src="https://github.com/user-attachments/assets/5e9cc441-7133-47cb-8703-2066c05d53d9" />


## 🍽️ Restaurant Performance
<img width="1441" height="807" alt="image" src="https://github.com/user-attachments/assets/95f3066b-812f-4934-a602-9d660955220f" />


## 🚚 Operations & Delivery
<img width="1423" height="797" alt="image" src="https://github.com/user-attachments/assets/49bf6926-edaa-4edb-a160-ce62f3658f8f" />


## 💬 Customer Feedback & Sentiment
<img width="1427" height="797" alt="image" src="https://github.com/user-attachments/assets/e1693f83-5a29-4c3a-a184-e8a6a893426a" />


---

## 📂 Model Structure

<img width="1756" height="806" alt="image" src="https://github.com/user-attachments/assets/94463612-7251-479b-9aab-6260fa413ec6" />







**Daksh Jakhar**
