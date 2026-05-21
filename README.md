# E‑commerce Transactions Analysis

**Identifying loyal customers and the channels & promotions that drive repeat purchases**


##  Project Overview

This analytics project focuses on a **global software retailer** selling subscriptions and add-ons across four product categories:
- **Analytics** (data visualization)
- **Design** (creative software, prototyping)
- **Collaboration** (team communication, project management)
- **AI** (machine learning, automation tools)

**Primary Objective:** Identify **loyal customers** (repeat buyers) and determine which **channels** and **promotional campaigns** drive their repeat purchases.

## 🎪 Business Objectives

### Primary Goals
1. **Track** sales and loyal-customer volumes over time
2. **Highlight** revenue drivers and repeat-purchase patterns
3. **Analyze** how discounts and pricing influence sales performance
4. **Deliver** clear, actionable insights for stakeholder decisions

### Secondary Goals
- Increase customer retention through targeted channel strategies
- Optimize discount campaigns to maximize repeat purchases
- Improve product bundling and cross-selling (add-on attach rates)
- Reduce refund rates by identifying problematic products/channels

## ❓ Guiding Questions

The analysis answers these specific business questions:

### Sales & Time Trends
- How do total sales change by month?
- What percent of monthly sales comes from loyal customers?
- Are there seasonal patterns in subscription purchases?

### Channel Performance
- Which channels bring in the most sales (volume & revenue)?
- Which channels bring the most repeat (loyal) customers?
- Do certain channels have higher refund rates?

### Customer Loyalty & Behavior
- How long do customers wait before their second purchase?
- Which products are most popular with loyal customers?
- Do annual plans bring higher revenue per customer than monthly plans?

### Product & Pricing
- Which products or plans sell the most?
- What is the average selling price (ASP) by country or currency?
- Which add-ons are most often bought with core products (attach rate)?

### Promotions & Discounts
- Which discount codes are used most?
- Do discounts increase repeat purchases or just one-time sales?

### Refund Analysis
- Where do refunds happen most (by product or channel)?
- What refund reasons are most common for loyal vs. new customers?

## 📊 Dataset Description

The dataset contains **transaction-level e-commerce data** for software subscriptions and add-ons:

| Field | Type | Description |
|-------|------|-------------|
| `event_id` | string | Unique transaction identifier |
| `event_type` | string | Purchase, refund, subscription renewal |
| `event_date` | datetime | Timestamp of transaction |
| `customer_id` | string | Unique customer identifier |
| `product_id` | string | Software product or add-on ID |
| `country` | string | Customer country |
| `latitude/longitude` | float | Customer geographic coordinates |
| `region` | string | Geographic region (APAC, EMEA, AMER, etc.) |
| `channel` | string | Sales channel (direct, partner, marketplace, email, social) |
| `payment_method` | string | Credit card, PayPal, invoice, crypto |
| `currency` | string | Transaction currency code |
| `quantity` | integer | Number of licenses/seats purchased |
| `unit_price_local` | float | Price per unit in local currency |
| `discount_code` | string | Promo code applied (e.g., LAUNCH20, ANNUAL10) |
| `discount_local` | float | Discount amount in local currency |
| `tax_local` | float | Tax amount in local currency |
| `net_revenue_local` | float | Net revenue after discount in local currency |
| `fx_rate_to_usd` | float | Exchange rate to USD |
| `net_revenue_usd` | float | Net revenue in USD |
| `is_refunded` | boolean | Whether transaction was refunded |
| `refund_datetime` | datetime | Timestamp of refund |
| `refund_reason` | string | Reason for refund (defective, changed mind, etc.) |

### Product Categories
| Category | Example Products |
|----------|------------------|
| Analytics | DataPro, VisualInsight, TableMaster |
| Design | Creativo, PixelPro, DesignStudio |
| Collaboration | TeamHub, SlackConnect, ProjectFlow |
| AI | MLStudio, AutoML, PredictPro |

### Plan Types
- **Monthly subscription** – Recurring monthly billing
- **Annual subscription** – Upfront yearly payment (typically discounted)
- **One-time purchase** – Perpetual license
- **Add-ons** – Additional features, seats, or storage

## 📈 Key Metrics & Definitions

| Metric | Definition |
|--------|------------|
| **Loyal Customer** | Customer with ≥2 purchases (can include renewals, upgrades, or cross-category buys) |
| **Repeat Purchase Rate** | % of customers who make a second purchase within 12 months |
| **Time to Second Purchase** | Days between first and second transaction |
| **Attach Rate** | % of core product purchases that include a specific add-on |
| **ASP (Average Selling Price)** | Net revenue per unit sold (by country/currency) |
| **Customer Lifetime Value (CLV)** | Total net revenue from a customer (excluding refunds) |
| **Discount Efficiency** | Repeat purchase rate for customers who used a discount vs. those who didn't |
| **Monthly Recurring Revenue (MRR)** | Revenue from active monthly subscriptions |
| **Annual Recurring Revenue (ARR)** | Annualized revenue from subscriptions |

## 🔬 Methodology
