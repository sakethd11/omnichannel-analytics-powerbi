# Omnichannel Analytics Dashboard | Power BI

An end-to-end Power BI analytics project that brings together **customer engagement, voice interactions, AI-assisted sales, and AI system performance** into a single interactive reporting solution.

The dashboard is built around a fictional organization, **MaDIq Labs**, with two analytical products: **VoxIQ** and **SalesIQ AI**.

> **Note:** This project uses synthetic/demo data and fictional business information for learning and portfolio purposes.

---

## 📊 Dashboard Showcase

### Executive Overview
<img width="6012" height="3430" alt="01_Executive_Overview png" src="https://github.com/user-attachments/assets/2c07cb23-9903-4af5-bfee-2bfb063d14d3" />

### VoxIQ — Voice Analytics
<img width="6012" height="3430" alt="02_VoxIQ_Analytics png" src="https://github.com/user-attachments/assets/d2e98e17-a47d-46b2-840d-022e45452494" />

### SalesIQ AI
<img width="6012" height="3430" alt="03_SalesIQ_AI png" src="https://github.com/user-attachments/assets/0fb5984a-b7ee-4230-96e0-f77ff221f418" />

### AI Performance
<img width="6012" height="3430" alt="04_AI_Performance png" src="https://github.com/user-attachments/assets/b63a311e-bc8c-4f33-821b-b7217ff24aa7" />

---

## 🔎 What the Dashboard Covers

### Executive Overview

The first page provides a high-level view of platform activity and business performance.

**Key metrics and analysis:**

* Total Engagements
* Engagement Rate
* Revenue Pipeline
* Conversion Rate
* Engagement Growth
* AI Performance
* Monthly engagement trends
* Conversion trends
* Product engagement share
* Product-level comparison
* Dynamic key insights

Users can filter the analysis by **Product, Region, Quarter, and Year/Month**.

### VoxIQ — Voice Analytics

This page focuses on customer voice interactions and call performance.

**Analysis includes:**

* Voice Calls
* Connected Calls
* Average Talk Time
* Call Success Rate
* Voice-to-Conversion Rate
* Unsuccessful Calls
* Call outcome distribution
* Calls by time of day
* Language distribution
* Average talk time by language
* Regional call performance

A time-of-day heatmap is included to identify periods with higher call activity.

### SalesIQ AI

This page examines the usage and effectiveness of AI-assisted sales interactions.

**Analysis includes:**

* Total Interactions
* Suggestions Generated
* Suggestions Used
* Adoption Rate
* Objection Assistance
* AI Confidence
* Average Session Duration
* Suggestions by use case
* Objection assistance by use case
* Customer sentiment
* Customer segments
* Top sales representative performance

### AI Performance

The final page focuses on the operational and technical performance of the AI platform.

**Analysis includes:**

* AI Accuracy
* Response Time
* Compliance Score
* Confidence Score
* Interactions Processed
* System Uptime
* Accuracy and confidence trends
* Product comparison
* AI efficiency
* Processing volume
* Workload and uptime

---

## 🧹 Data Preparation

Multiple CSV sources were brought into Power BI and prepared using **Power Query**.

The transformation workflow included:

* Importing multiple source files
* Standardizing column headers
* Setting appropriate data types
* Cleaning categorical values
* Preparing date and datetime fields
* Creating fields required for time-based analysis
* Standardizing product and business terminology
* Validating the transformed data before reporting

---

## 🗂️ Data Model

The report uses shared dimensions to provide consistent filtering across the different analytical areas.

Core dimensions include:

* **Date**
* **Product**
* **Region**

Additional supporting/helper tables were incorporated where required for specialized calculations, comparisons, and visual behaviour.

This structure allows common filters to work consistently across voice, sales, engagement, and AI performance analysis.

---

## 🧮 DAX & Analytical Calculations

The report uses reusable DAX measures for the main KPIs rather than depending entirely on visual-level calculations.

Calculations cover areas such as:

* Engagement
* Conversion
* Revenue pipeline
* Voice performance
* Sales interaction adoption
* AI performance
* Previous-month comparisons
* Month-over-Month changes
* Product comparisons
* Dynamic text-based insights

Some of the DAX functions used include:

`CALCULATE` · `DIVIDE` · `DATEADD` · `SELECTEDVALUE` · `SWITCH` · `REMOVEFILTERS` · `FORMAT`

---

## ⚙️ Interactive Features

The dashboard includes several interactive reporting features:

* Dynamic slicers
* Cross-filtering between visuals
* Month-over-Month KPI comparisons
* Dynamic insight cards
* Product performance comparisons
* Time-of-day analysis
* Customer segmentation
* Sales representative analysis
* AI efficiency analysis
* Consistent navigation across report pages

---

## 📈 Key Analytical Areas

The report enables users to explore performance across dimensions such as:

| Dimension  | Examples                            |
| ---------- | ----------------------------------- |
| Product    | VoxIQ, SalesIQ AI                   |
| Geography  | Regional performance                |
| Time       | Year, Month, Quarter                |
| Voice      | Calls, outcomes, language           |
| Sales      | Interactions, suggestions, adoption |
| Customer   | Segment, sentiment                  |
| AI         | Accuracy, confidence, response time |
| Operations | Processing volume, uptime           |

---

## 💡 Key Learning Areas

Building the report involved working with calculations that behave differently depending on the active filter context.

Some of the important areas explored during development were:

* DAX filter context
* Time intelligence
* Measure dependencies
* Helper/disconnected tables
* Cross-filtering behaviour
* KPI validation
* Debugging DAX calculations
* Data consistency across multiple sources
* Designing dashboards for both summary and detailed analysis

This project helped bridge the gap between creating individual Power BI visuals and developing a complete analytical reporting solution.

---

## 🛠️ Technology Stack

* **Microsoft Power BI Desktop**
* **Power Query**
* **DAX**
* **Data Modelling**
* **Data Visualization**
* **KPI Development**
* **Time Intelligence**
* **Data Validation**
* **CSV Data Sources**

---

## 📁 Repository Contents

```text
omnichannel-analytics-powerbi/
│
├── dashboards/
│   └── Omnichannel Analytics Power BI Dashboard.pbix
│
├── datasets/
│   ├── Automation Events.csv
│   ├── CRM Updates.csv
│   ├── Customer Calls.csv
│   ├── Field Sales.csv
│   ├── SalesIQ AI Interactions.csv
│   └── AI Performance Logs.csv
│
├── documentation/
│   ├── MaDIq Labs Dashboard Explanation.pdf
│   ├── MaDIq Labs Technical Explanation.pdf
│   └── .gitkeep
│
└── screenshots/
    ├── 01_Executive_Overview
    ├── 02_VoxIQ_Analytics
    ├── 03_SalesIQ_AI
    └── 04_AI_Performance
```

---

## 📚 Documentation

Additional project material is available in the repository:

* [Dashboard Explanation](documentation/)
* [Technical Documentation](documentation/)
* [Source Datasets](datasets/)
* [Power BI Dashboard](dashboards/)

The documentation provides additional details about the dashboard design, data preparation, modelling approach, KPI calculations, DAX logic, and visualization decisions.

---

## 🚀 Opening the Project

To explore the dashboard:

1. Open the `dashboards` folder.
2. Download the `.pbix` file.
3. Open it using **Microsoft Power BI Desktop**.
4. Keep the datasets available locally if you need to refresh the report.
5. Use the report navigation and slicers to explore the different analytical pages.

---

## ⚠️ Disclaimer

This project is intended for **learning and portfolio purposes**.

MaDIq Labs, VoxIQ, and SalesIQ AI are fictional names. The datasets included in this repository are synthetic/demo data and do not represent the operations, customers, or performance of any real organization.

---

## 👤 About Me

**Saketh Degala**

Data Analytics | Business Intelligence | Power BI | SQL | Python | Excel

I am interested in using data analytics and business intelligence tools to transform raw data into meaningful insights and interactive reporting solutions.

---

## 🔗 Repository

[View the complete project on GitHub](.)

---
