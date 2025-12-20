# Quarterly Sales Performance Dashboard (CRM Analytics)

## Project Background

This project is based on a mid-sized B2B technology company specializing in **computer hardware solutions for large enterprise clients**. The company operates on a direct sales model, where sales agents manage long-cycle opportunities supported by regional sales managers.

In 2017, the company implemented a new **CRM system** to track sales opportunities, deal stages, and outcomes. While the CRM successfully captured transactional data, leadership lacked visibility into historical performance because 2017 sales data existed only within the platform and had not been consolidated into an analytical or reporting format.

From the perspective of a data analyst working within the organization, this created challenges for sales leadership, including limited visibility into quarterly trends, difficulty evaluating individual and manager performance, and reduced ability to make data-driven decisions around coaching, forecasting, and resource allocation.

Insights and recommendations are provided on the following key areas:

- **Quarterly Sales Performance & Conversion Trends**
- **Individual Sales Agent Effectiveness**
- **Manager-Level Performance Impact**
- **Revenue Concentration & Growth Constraints**

The SQL queries used to inspect and clean the data for this analysis can be found here: [link]

Targeted SQL queries addressing specific business questions can be found here: [link]

An interactive dashboard used to explore quarterly sales trends can be found here: [link](https://docs.google.com/spreadsheets/d/1MXS3myei8jcwDWGrGIxTzHA2rDkymO5gXy9UlNBX0_o/edit?usp=sharing)

---

## Data Structure & Initial Checks

The CRM database used for this analysis consists of **four core tables**, containing opportunity-level data for all sales activity in 2017. The total dataset includes several thousand opportunity records.

The tables are structured as follows:

- **Opportunities Table:** Opportunity ID, deal status (Won/Lost/Open), close date, revenue indicators  
- **Sales Agents Table:** Sales agent identifiers and attribution  
- **Managers Table:** Manager-to-agent mapping  
- **Calendar Table:** Date fields used for quarterly aggregation  

Initial data checks focused on:

- Validating opportunity status consistency  
- Ensuring correct manager and sales agent attribution  
- Verifying quarterly date assignments  
- Removing duplicates and incomplete records  

These checks ensured the analysis was based on clean, reliable CRM data suitable for executive reporting.

[Entity Relationship Diagram included in repository]

---

## Executive Summary

### Overview of Findings

Sales performance in 2017 was driven primarily by **opportunity volume rather than conversion efficiency**. While total wins fluctuated quarter-over-quarter, win rates remained consistently strong at approximately **60%**, indicating stable sales execution.

The analysis revealed **significant performance variance at both the individual and manager levels**, highlighting clear opportunities for targeted coaching, process standardization, and scalable revenue growth.

<img width="792" height="584" alt="Screenshot 2025-12-18 123401" src="https://github.com/user-attachments/assets/a91d0109-5d49-4a58-9243-4eb4fb3e2217" />


---

## Insights Deep Dive

### Category 1: Quarterly Sales Performance

* **Q4 2017 closed with 1,196 won opportunities**, a decline of 61 deals (-4.9%) compared to Q3 (1,257 wins).
  
* **Win rate remained stable at 60.3%**, despite the reduction in total wins.
  
* Q1 recorded 531 wins, while Q2 and Q3 each exceeded 1,250 wins.
  
* Performance data shows clear **seasonality**, with Q1 consistently underperforming relative to later quarters.

<img width="811" height="86" alt="Category 1 a" src="https://github.com/user-attachments/assets/2460fee8-034e-440f-ae29-0168ae13688d" />
<img width="661" height="391" alt="Category 1 b" src="https://github.com/user-attachments/assets/da195e36-1198-4c0e-b7ad-cc9f8a8c8cb3" />


---

### Category 2: Individual Sales Agent Performance

* **Darcel Schlecht emerged as the top-performing sales agent in Q4**, closing the highest number of opportunities.
  
* **Garnet Kinder recorded the lowest performance with 16 closed deals**, accounting for approximately 1.3% of total Q4 wins.
  
* The performance gap between top and bottom agents exceeded a **6× difference**.
  
* Over 40% of agents fell into a mid-tier performance range (30–55 wins per quarter).

<img width="673" height="597" alt="Category 2" src="https://github.com/user-attachments/assets/080881a2-4cb2-4ae6-a843-0ec43871e906" />



---

### Category 3: Manager-Level Performance

* **Summer Sewald’s team generated the highest total number of closed-won opportunities**, totaling **828 wins**. Q4 performance reached **249 wins** at a **64.7% win rate**, up **27 wins compared to the previous quarter**.  

* **Cara Losch’s team recorded the lowest overall sales wins**, with **480 total wins**. Q4 closed with **137 wins** at a **58.8% win rate**, down **10 wins from the prior quarter**.  

* Teams under high-performing managers showed greater consistency in quarterly output.  

* Manager-level variance directly influenced overall revenue outcomes.  <br>

[Summer Sewals]<br>
<img width="761" height="540" alt="Summer Sewald" src="https://github.com/user-attachments/assets/8b4360e4-a32d-44ec-a973-658ee4f36970" /><br>
[Cara Losch]<br>
<img width="755" height="531" alt="Cara Losch" src="https://github.com/user-attachments/assets/c851b0bf-3b53-46e7-b897-b89e4af1a3e5" />

---

### Category 4: Revenue Concentration & Growth Constraints

* The **top 5 sales agents generated over 20% of total Q4 wins**.
  
* The **bottom 25% of agents contributed less than 10%** of total closed deals.
  
* With a 60.3% win rate, a **10% increase in qualified opportunities** would have resulted in approximately **120 additional closed deals** in Q4.
  
* Growth constraints are primarily driven by **opportunity volume**, not conversion effectiveness.
<img width="792" height="584" alt="Screenshot 2025-12-18 123401" src="https://github.com/user-attachments/assets/0cd5f10f-6218-4153-9c6e-696c9dee3e83" />

---

## Recommendations

Based on the insights above, we recommend the **Sales Leadership and Revenue Operations teams** consider the following actions:

* Performance data shows Summer Sewald’s team consistently outperformed others.  
  **Standardize and scale best practices from Summer Sewald’s team to reduce variability and improve overall sales consistency.**

* Garnet Kinder closed only 16 deals in Q4, significantly below the team average.  
  **Implement targeted coaching, territory review, and lead-quality assessment to improve underperforming agent output.**

* Cara Losch’s team recorded the lowest total wins among managers.  
  **Conduct a manager-level enablement review to improve coaching cadence, pipeline management, and resource allocation.**

* Stable win rates indicate strong sales execution.  
  **Increase qualified opportunity generation to drive immediate revenue growth without changing existing sales processes.**

* Revenue is concentrated among a small group of top performers.  
  **Reduce dependency risk by improving mid-tier agent performance through scalable training and standardized workflows.**

---

## Assumptions and Caveats

Throughout the analysis, the following assumptions and limitations were considered:

* Opportunities missing manager attribution were excluded from manager-level analysis.
  
* Open opportunities without a close date were not included in quarterly win calculations.
  
* Seasonal trends were based solely on 2017 data and may not reflect future market conditions.
  
* Revenue impact was inferred from win counts due to the absence of deal value fields.

---

## Portfolio Strength Statement

This project demonstrates my ability to:

- Translate CRM data into **quantified, actionable business insights**
- Analyze performance at the **agent, manager, and organizational level**
- Build dashboards designed for **non-technical stakeholders**
- Support **data-driven decision-making** in sales and marketing contexts
