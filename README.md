#  Credit Card Financial Dashboard

A real-time financial analytics pipeline built using **PostgreSQL (Dockerized)** and **Power BI** to monitor credit card transactions, customer behavior, and revenue trends.

This project transforms raw CSV transaction and customer data into dynamic, insight-driven dashboards that track KPIs such as revenue, interest, transaction volume, and demographic performance.

---

##  Project Overview

Traditional spreadsheet-based analysis lacks scalability and real-time capability.  
This project implements:

- A containerized PostgreSQL database
- Structured SQL-based data transformation
- Power BI dashboards for advanced financial reporting
- KPI tracking with DAX measures

The result is a reproducible, analytics-ready financial intelligence system.

---

##  Architecture

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|------------|
| Database | PostgreSQL (Docker Container) |
| Visualization | Power BI Desktop |
| Data Processing | SQL (Data Cleaning & Transformation) |
| Environment | Docker Desktop, PowerShell |
| Version Control | Git & GitHub |

---

##  Insights & Analysis

**Silver > Platinum Reality**  
Blue and Silver card tiers are responsible for the overwhelming majority of portfolio revenue (~$47M combined), while Platinum contributes only ~$1M.  

This indicates:
- Premium positioning does not necessarily translate to revenue dominance.
- Mid-tier products drive scalability and consistent transaction flow.

---

###  2. The Q4 Surge

Transaction volume and revenue both peaked in **Q4**, reaching **$806M in total transaction volume**.

Implications:
- Strong seasonal spending behavior
- Potential holiday-driven financial activity
- Forecasting models should incorporate quarterly seasonality

---

###  3. Job Profile Revenue Dynamics

**Business professionals generate the highest revenue (~$18M).**  
However, **Blue-collar workers hold the highest total income pool (~$588M)** but contribute only ~$7M in revenue.

This highlights:
- A conversion inefficiency within the blue-collar segment
- Untapped monetization potential
- Opportunity for targeted engagement strategies

---

###  4. Transaction Mode Dominance

Physical **Swipe transactions (~$36M)** significantly outperform:
- Chip (~$17M)
- Online (~$4M)

This suggests:
- Strong reliance on in-store spending
- Lower digital transaction penetration
- Potential growth opportunity in online payment adoption

---

###  5. The Gender Revenue Gap

In Q4, **female customers outperformed male customers by approximately $5M in revenue.**

Possible interpretations:
- Higher seasonal engagement among female customers
- Different spending behavior patterns
- Marketing campaigns may be resonating more strongly with this segment

---

###  6. The Blue-Collar Paradox

Despite having the **largest cumulative income base (~$588M)**, blue-collar workers generate only a small share of total revenue (~$7M).

This indicates:
- High saving or lower discretionary spending behavior
- Limited credit utilization
- Cross-selling and product education opportunities

---

###  7. Category Driver — Bills as #1 Segment

The highest revenue category is **Bills (~$14M)**.

Key takeaway:
- The platform functions primarily as a utility-driven financial tool
- Customers prioritize recurring obligations over discretionary purchases

---

### 8. Regional Revenue Concentration

**Texas and New York alone contribute approximately $13M combined**, dominating the revenue leaderboard.

Implications:
- Revenue concentration risk
- Geographic dependency
- Expansion potential in underperforming states

---

##  Executive Summary

The portfolio demonstrates:

- Strong mid-tier card dependency  
- Seasonal revenue volatility (Q4 spike)  
- Under-monetized income segments  
- Physical transaction dominance  
- Regional revenue concentration  

These insights provide a foundation for:
- Targeted marketing strategies  
- Credit utilization optimization  
- Digital transaction growth initiatives  
- Predictive seasonal forecasting  

##  Database Setup (Dockerized PostgreSQL)

Run PostgreSQL container:

```bash
docker run --name cc-db-container \
-e POSTGRES_PASSWORD=your_password \
-p 5432:5432 \
-d postgres

