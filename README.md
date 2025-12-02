# 📊 PhonePe Payments Funnel Analysis

This repository contains an exploratory data analysis (EDA) of PhonePe’s payments funnel using daily transaction & traffic data.  
The goal is to understand how users move through key steps of the payment journey and identify where drop-offs happen.

---

## 🧾 Dataset Overview

The main data source is an Excel file: `PhonePe Dataset.xlsx`, which contains **two sheets**:

### 1. `Page Sessions`
Funnel-level metrics for the payments journey:

- **Date**
- **List of Senders** – number of users who initiated a payment
- **Amount Entry** – users who entered the amount
- **UPI PIN Page** – users who reached the PIN entry step
- **Successful Transfers** – completed payments
- **Total Traffic / List of Senders**
- **Overall Conversion**
- **Overall Conversion – Same Day Last Week**
- **Step-wise Ratios**
  - `List of Senders / Amount Entry`
  - `Amount Entry / UPI PIN Page`
  - `UPI PIN Page / Successful Transfers`
- **Same-day-last-week metrics**
  - `T/L same day last week`
  - `L/A same day last week`
  - `A/U same day last week`
  - `U/S same day last week`

These columns together describe how many users are retained or dropped at each stage of the payment funnel, and how that changes over time.

### 2. `Total Traffic`
Daily traffic split by payment type:

- **Date**
- **P2P** – person-to-person payments
- **Retail** – merchant/retail payments
- **Total Traffic**
- **P2P same day last week**
- **Retail same day last week**

This sheet is useful for understanding volume trends, seasonality, and week-on-week changes in traffic.

---

## 🎯 Objectives

In this project, the dataset can be used to:

- Analyze the **end-to-end payment funnel**:
  - Sender → Amount Entry → UPI PIN → Successful Transfer
- Compute **conversion rates** at each stage and overall
- Identify **drop-off points** in the funnel
- Compare **current performance vs. same day last week**
- Study **P2P vs Retail** traffic behavior and trends
- Build visuals that explain:
  - Funnel conversion
  - Daily trends
  - Week-on-week changes
