# Product Metrics Calculator

## Overview

This guide helps product managers define, calculate, and track essential product metrics for data-driven decision making.

---

## Core Product Metrics

### 1. Monthly Active Users (MAU)

**Definition:**
Number of unique users who performed a key action in the last 30 days.

**Formula:**
```
MAU = Count of unique users with activity in last 30 days
```

**What counts as "activity":**
- Login
- Core feature usage
- Content creation
- Purchase/transaction
- Define based on your product's value proposition

**When to use:**
- Measure overall product health
- Track growth trends
- Compare periods
- Set growth goals

**Example:**
```
January MAU = 45,000 users
February MAU = 52,000 users
Growth = ((52,000 - 45,000) / 45,000) × 100 = 15.6%
```

---

### 2. Daily Active Users (DAU)

**Definition:**
Number of unique users who performed a key action in the last 24 hours.

**Formula:**
```
DAU = Count of unique users with activity in last 24 hours
```

**When to use:**
- Products with daily use expectation
- Monitor short-term trends
- Identify day-of-week patterns
- Measure engagement intensity

---

### 3. DAU/MAU Ratio (Stickiness)

**Definition:**
Percentage of monthly users who return daily. Measures product stickiness.

**Formula:**
```
Stickiness = (DAU / MAU) × 100
```

**Interpretation:**
- **> 20%:** Very sticky (e.g., Facebook, WhatsApp)
- **10-20%:** Good stickiness (e.g., LinkedIn)
- **< 10%:** Low stickiness (normal for some products)

**Example:**
```
DAU = 15,000
MAU = 50,000
Stickiness = (15,000 / 50,000) × 100 = 30% (Great!)
```

---

### 4. User Retention

**Definition:**
Percentage of users who return to the product after their first visit.

**Cohort Retention Formula:**
```
Day N Retention = (Users active on Day N / Users acquired on Day 0) × 100
```

**Example Cohort Table:**

| Days Since Signup | Cohort Size | Active Users | Retention % |
|------------------|-------------|--------------|-------------|
| Day 0 | 1,000 | 1,000 | 100% |
| Day 1 | 1,000 | 400 | 40% |
| Day 7 | 1,000 | 250 | 25% |
| Day 30 | 1,000 | 150 | 15% |
| Day 90 | 1,000 | 100 | 10% |

**Good retention benchmarks:**
- **Day 1:** 40-50%
- **Day 7:** 20-30%
- **Day 30:** 10-15%

---

### 5. Churn Rate

**Definition:**
Percentage of users/customers who stop using the product.

**Formula:**
```
Churn Rate = (Users Lost / Total Users at Start) × 100
```

**Example:**
```
Start of month: 1,000 users
End of month: 950 users
Lost: 50 users

Churn Rate = (50 / 1,000) × 100 = 5%
```

**Monthly Churn Benchmarks:**
- **< 2%:** Excellent (B2B SaaS)
- **2-5%:** Good
- **5-7%:** Acceptable for consumer
- **> 7%:** Concerning, investigate!

**Revenue Churn:**
```
Revenue Churn = (MRR Lost / Starting MRR) × 100
```

---

### 6. Customer Acquisition Cost (CAC)

**Definition:**
Cost to acquire one new customer.

**Formula:**
```
CAC = Total Sales & Marketing Costs / Number of New Customers
```

**Example:**
```
Marketing spend: $50,000
Sales spend: $30,000
New customers: 400

CAC = ($50,000 + $30,000) / 400 = $200 per customer
```

**What to include:**
- Advertising spend
- Marketing salaries
- Sales salaries
- Marketing tools/software
- Content creation costs

---

### 7. Customer Lifetime Value (LTV)

**Definition:**
Total revenue expected from a customer over their lifetime.

**Simple Formula:**
```
LTV = (Average Revenue Per User × Average Customer Lifetime)
```

**More Accurate Formula:**
```
LTV = (ARPU × Gross Margin) / Churn Rate
```

**Example:**
```
ARPU = $50/month
Gross Margin = 80%
Churn Rate = 5%/month (0.05)

LTV = ($50 × 0.80) / 0.05 = $800
```

---

### 8. LTV:CAC Ratio

**Definition:**
How much value a customer generates compared to acquisition cost.

**Formula:**
```
LTV:CAC = LTV / CAC
```

**Interpretation:**
- **3:1 or higher:** Healthy, scalable
- **1:1:** Breaking even, unsustainable
- **< 1:1:** Losing money on each customer

**Example:**
```
LTV = $800
CAC = $200
LTV:CAC = 800 / 200 = 4:1 (Great!)
```

---

### 9. Conversion Rate

**Definition:**
Percentage of users who complete a desired action.

**Formula:**
```
Conversion Rate = (Conversions / Total Visitors) × 100
```

**Common Conversions:**
- Sign up
- Free-to-paid
- Purchase
- Feature adoption

**Example:**
```
Website visitors: 10,000
Sign-ups: 500

Conversion Rate = (500 / 10,000) × 100 = 5%
```

**Benchmark Conversion Rates:**
- **Landing page:** 2-5%
- **Free trial to paid:** 10-25%
- **E-commerce:** 2-3%
- **B2B SaaS:** 3-5%

---

### 10. Net Promoter Score (NPS)

**Definition:**
Measures customer loyalty and satisfaction.

**Formula:**
```
NPS = % Promoters - % Detractors
```

**Scoring:**
- **9-10:** Promoters (loyal enthusiasts)
- **7-8:** Passives (satisfied but unenthusiastic)
- **0-6:** Detractors (unhappy customers)

**Example:**
```
Survey responses: 100
Promoters (9-10): 60
Passives (7-8): 30
Detractors (0-6): 10

NPS = 60% - 10% = 50
```

**NPS Benchmarks:**
- **> 50:** Excellent
- **30-50:** Good
- **0-30:** Needs improvement
- **< 0:** Crisis

---

## Engagement Metrics

### 11. Feature Adoption Rate

**Formula:**
```
Adoption Rate = (Users using feature / Total active users) × 100
```

**Example:**
```
Total active users: 10,000
Users of new feature: 3,500

Adoption Rate = (3,500 / 10,000) × 100 = 35%
```

---

### 12. Time to Value (TTV)

**Definition:**
Time from sign-up to first meaningful action.

**What to measure:**
- Time to complete onboarding
- Time to first "aha moment"
- Time to first transaction

**Example:**
```
Average time from sign-up to first use: 3.5 days

Goal: Reduce to < 24 hours
```

---

### 13. Session Duration

**Formula:**
```
Average Session Duration = Total time in app / Number of sessions
```

**Example:**
```
Total session time: 50,000 minutes
Number of sessions: 10,000

Average = 50,000 / 10,000 = 5 minutes per session
```

---

### 14. Activation Rate

**Definition:**
Percentage of users who complete onboarding and experience core value.

**Formula:**
```
Activation Rate = (Activated users / Total sign-ups) × 100
```

**Define "activated" for your product:**
- Completed profile
- Connected integration
- Invited team member
- Made first purchase
- Completed tutorial

---

## Business Metrics

### 15. Monthly Recurring Revenue (MRR)

**Formula:**
```
MRR = Number of customers × Average revenue per customer
```

**Components:**
- **New MRR:** From new customers
- **Expansion MRR:** From upsells/cross-sells
- **Churned MRR:** Lost from cancellations
- **Net New MRR:** New + Expansion - Churned

**Example:**
```
Start MRR: $100,000
New MRR: +$15,000
Expansion MRR: +$5,000
Churned MRR: -$8,000

End MRR: $100,000 + $15,000 + $5,000 - $8,000 = $112,000
Growth: 12%
```

---

### 16. Annual Recurring Revenue (ARR)

**Formula:**
```
ARR = MRR × 12
```

**When to use:**
- Annual contracts
- Enterprise sales
- Long-term planning
- Fundraising

---

### 17. Revenue Per User (ARPU/ARPA)

**Formula:**
```
ARPU = Total Revenue / Total Active Users
```

**Example:**
```
Monthly revenue: $100,000
Active users: 2,000

ARPU = $100,000 / 2,000 = $50 per user
```

---

### 18. Payback Period

**Definition:**
Time to recover customer acquisition cost.

**Formula:**
```
Payback Period = CAC / (ARPU × Gross Margin)
```

**Example:**
```
CAC = $200
ARPU = $50
Gross Margin = 80%

Payback = $200 / ($50 × 0.80) = 5 months
```

**Benchmark:** < 12 months ideal

---

## Metrics Calculator Template

### Spreadsheet Structure

```
| Month | MAU | DAU | New Users | Churned | MRR | CAC | LTV |
|-------|-----|-----|-----------|---------|-----|-----|-----|
| Jan   |     |     |           |         |     |     |     |
| Feb   |     |     |           |         |     |     |     |
| Mar   |     |     |           |         |     |     |     |
```

### Calculated Fields

```
Stickiness = DAU / MAU
User Growth = (Current MAU - Previous MAU) / Previous MAU
Churn Rate = Churned / Starting Users
LTV:CAC = LTV / CAC
MRR Growth = (Current MRR - Previous MRR) / Previous MRR
```

---

## How to Choose the Right Metrics

### By Product Stage

**Early Stage (Pre-Product Market Fit):**
- Focus: Retention, engagement, activation
- Key metrics: Day 1/7/30 retention, activation rate
- Goal: Find product-market fit

**Growth Stage:**
- Focus: Acquisition and activation
- Key metrics: MAU growth, CAC, conversion rate
- Goal: Scale efficiently

**Mature Stage:**
- Focus: Monetization and efficiency
- Key metrics: LTV:CAC, MRR growth, NPS
- Goal: Optimize and expand

---

### By Product Type

**B2B SaaS:**
- MRR/ARR
- Churn rate
- CAC payback period
- LTV:CAC ratio

**Consumer Mobile App:**
- DAU/MAU
- Retention curves
- Session duration
- Feature adoption

**E-commerce:**
- Conversion rate
- Average order value
- Cart abandonment
- Customer lifetime value

**Marketplace:**
- GMV (Gross Merchandise Value)
- Take rate
- Buyer/Seller balance
- Frequency of purchases

---

## Metric Dashboard Template

### Weekly Dashboard

**Growth:**
- MAU: [Current] ([% change] vs last week)
- New users: [Count]
- Churn: [Rate]

**Engagement:**
- DAU/MAU: [Ratio]
- Session duration: [Minutes]
- Feature X adoption: [%]

**Revenue:**
- MRR: $[Amount] ([% growth])
- ARPU: $[Amount]

**Quality:**
- NPS: [Score]
- Support tickets: [Count]
- Uptime: [%]

---

## Common Metric Mistakes

**DON'T:**
❌ Track too many metrics (focus on 5-7 key ones)  
❌ Only look at vanity metrics (total downloads)  
❌ Ignore cohort analysis  
❌ Compare unlike time periods  
❌ Forget to segment (power users vs casual)  
❌ Look at metrics in isolation  
❌ Change metric definitions frequently  

**DO:**
✅ Define metrics clearly  
✅ Track trends over time  
✅ Segment by user type  
✅ Compare cohorts  
✅ Set targets and goals  
✅ Review metrics regularly  
✅ Share metrics with team  

---

## Resources

- [Lean Analytics](http://leananalyticsbook.com/)
- [Amplitude Blog](https://amplitude.com/blog)
- [Mixpanel Benchmarks](https://mixpanel.com/benchmarks/)
- [SaaS Metrics Guide](https://www.forentrepreneurs.com/saas-metrics-2/)
