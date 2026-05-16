# Tata-Simulation-
# Tata Data Analytics Job Simulation - Online Retail Performance Dashboard

## 📌 Project Overview
This repository contains a complete retail analytics solution developed as part of the **Tata Insights & Edge Data Analytics Job Simulation** via Forage. The project simulates a real-world scenario where the Tata leadership team requires deep business intelligence insights to drive strategic decision-making. 

Using Tableau and a dataset of over 500k operational transactions, I designed and built an executive dashboard focused on four critical business metrics: chronological revenue trends, global market share, high-value customer identification, and bulk demand distribution.

---

## 📊 Dataset & Business Architecture
The analysis is built on the **Online Retail Dataset**, tracking international transactional data. 

### Core Tech Stack
* **Data Processing & Analytics:** Tableau Desktop / Tableau Public
* **Data Source:** Raw Transactional Ledger (CSV Format, ~45MB, 541,909 rows)
* **Key Calculated Fields:** $$\text{Revenue} = \text{Quantity} \times \text{UnitPrice}$$

---

## 🔍 Executive Insights & Question Breakdown

### 📈 Question 1: Revenue Trends Over Time
* **Objective:** Provide senior leadership with a clear view of the business's financial trajectory across the year to identify seasonal patterns.
* **Granularity:** Configured by Month/Quarter (`Invoice Date`) against total `Revenue`.
* **Key Insight:** The data reveals a steady baseline revenue performance through the first three quarters of the year, followed by an exponential **surge starting in October, peaking drastically in November**. This points heavily to a high dependency on Q4 holiday shopping and end-of-year wholesale restocking.
* **Visualization Placeholder:** * https://github.com/amnabi-h/Tata-Simulation-/blob/main/Question%201.png *

### 🌍 Question 2: Market Penetration (Revenue by Country)
* **Objective:** Map out the global distribution of revenue to isolate the top 10 performing international markets (excluding outliers if necessary).
* **Granularity:** Evaluated by `Country` against total aggregated `Revenue`.
* **Key Insight:** The **United Kingdom stands as the absolute dominant core market**, accounting for the vast majority of total global revenue. Secondary high-performing clusters are firmly rooted in Western Europe, led by **the Netherlands, Ireland, Germany, and France**, indicating strong baseline regional expansion channels.
* **Visualization Placeholder:** * https://github.com/amnabi-h/Tata-Simulation-/blob/main/Question%202.png *

### 👥 Question 3: High-Value Customer Identification (Top 10 Customers)
* **Objective:** Identify and rank the top 10 individual customer accounts by total revenue generated to enable targeted loyalty programs and VIP client management.
* **Granularity:** Evaluated by `Customer ID` sorted descending by total `Revenue`.
* **Key Insight:** The analysis uncovers a classic Pareto distribution where a **small, highly concentrated group of institutional or wholesale buyers (identified by unique Customer IDs) contribute disproportionately to total revenue**. Safeguarding these accounts through dedicated account management is vital for maintaining steady cash flow.
* **Visualization Placeholder:** * https://github.com/amnabi-h/Tata-Simulation-/blob/main/Question%203.png *

### 📦 Question 4: Product Demand Distribution (Quantity by Country)
* **Objective:** Analyze demand by charting the physical volume of items sold globally to optimize supply chain and logistics fulfillment strategies.
* **Granularity:** Evaluated by `Country` mapped against total physical `Quantity` (excluding the UK to clearly visualize secondary markets).
* **Key Insight:** When looking past the core UK market, countries like **the Netherlands and Germany show massive demand spikes in physical units**. This confirms that these regions are buying lower-cost products in massive bulk quantities, which tells our logistics teams exactly where to optimize regional warehouse stock levels.
* **Visualization Placeholder:** *[Insert image link or upload `question_4.png` here]*

---

## 💡 Strategic Business Recommendations
Based on the dashboard visualizations, the following actionable strategies have been formulated for the Tata corporate leadership team:

1. **Inventory & Warehouse Scaling:** To capitalize on the dramatic Q4 sales spikes discovered in Question 1, logistics teams must aggressively scale up inventory holding levels by late August/September to completely eliminate stockouts during peak demand.
2. **VIP Loyalty Architecture:** Implement a dedicated corporate loyalty structure or volume-based pricing agreements specifically targeted at the Top 10 high-value B2B accounts identified in Question 3 to ensure long-term retention.
3. **Targeted European Logistics:** Establish localized distribution hubs or partner channels in the Netherlands and Germany to directly support the high-volume bulk item demand identified in Question 4, dramatically reducing cross-border shipping costs and transit times.

---

## 🛠️ How to View and Run the Project

1. **Option 1 (Interactive):** View my interactive dashboard directly via my [Tableau Public Profile](YOUR_TABLEAU_PUBLIC_LINK_HERE).
2. **Option 2 (Local Run):**
   * Clone this repository to your local machine.
   * Open the `tata.twb` file using **Tableau Desktop** or **Tableau Public**.
   * If prompted for a broken data connection, redirect the file pathway to the dataset located inside the `/data` folder of this repository.

---
*Disclaimer: This project was completed as part of an open data job simulation provided by Tata via Forage to demonstrate core analytical execution and dashboard engineering capabilities.*
