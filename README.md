# NorthStar Logistics - Supply Chain & Inventory Analysis

## 📊 Project Overview

NorthStar Logistics is a mid-sized distribution firm facing rising shipping costs and delivery delays. As a Data Analyst, I was tasked with migrating their manual Excel tracking to a dynamic Power BI solution.

The goal of this project was to identify cost drivers, improve On-Time Delivery (OTD) rates, and analyze inventory risks ("Dead Stock").

#### ❓ Business Problem & Questions

Management required answers to the following key operational questions:

- Shipment Performance: What is our On-Time Delivery %? Are we meeting SLAs?

- Financial Health: How will a 10% increase in carrier rates impact our bottom line?

- Inventory Management: Which products are "Dead Stock" (High inventory, low sales)?

- Basket Analysis: When customers buy a Monitor, what else do they buy?

#### 🛠️ Technical Solution

1. Data Modeling (Star Schema)

I transformed raw CSV flat files into a robust Star Schema to optimize performance:

Fact Tables: Shipments_Data, Inventory_Snapshot

Dimension Tables: Products, Customers, DateTable

Relationships: One-to-Many relationships utilizing a centralized Date Table for Time Intelligence.

2. Advanced DAX Features

Market Basket Analysis: Used INTERSECT and CALCULATETABLE to identify co-shipped products.

Parameter Modeling: Created a "What-If" parameter to simulate shipping cost increases (0-50%) dynamically.

Inventory Risk Matrix: Calculated Sell-Through Rate % vs Days on Hand (DOH) to visualize stock efficiency.

3. Dashboard Design

Page 1: Executive Overview: High-level KPIs (OTD %, Revenue, Costs) and shipping trends.

Page 2: Operations & Inventory: Scatter chart analysis for inventory risk and granular order detail.

#### 📸 Dashboard Visuals

<img width="1608" height="852" alt="Northstart logistics 1" src="https://github.com/user-attachments/assets/78b29e27-0fda-47bc-8bb3-d872fe6e8940" />

#### Key Insights Discovered

Efficiency: Identified that "Furniture" category shipments have a 15% higher late rate than "Electronics".

Cost Savings: The "What-If" simulation revealed that a 10% carrier rate hike would increase monthly operational costs by $12,500, prompting a vendor renegotiation.

Cross-Selling: Analysis showed that 60% of "Monitor" orders include a "Docking Station," suggesting a bundle opportunity.

<img width="1612" height="852" alt="Northstart logistics 2" src="https://github.com/user-attachments/assets/31f88875-006a-4a64-a3d3-d630b36a2dd4" />

### 👨‍💻 Author's Note (For Recruiters)

This project demonstrates my ability to translate raw logistics data into actionable business intelligence.

## Key Skills Demonstrated:

Data Modeling: Star Schema design, Relationship management.

DAX: CALCULATE, SUMX, INTERSECT, SELECTEDVALUE, Time Intelligence.

Visualization: Custom tooltips, Drill-throughs, Conditional Formatting, Analytics Lines.

Business Acumen: KPIs definition (OTD, COGS, DOH) and Scenario Planning.
