# Demo 4: Accounts Receivable with SQL in Microsoft Fabric

[🎬 Watch the video](https://aka.ms/AAxud0p)

One year after modernizing their Accounts Receivable app with Azure SQL, Zava’s finance team faced new challenges:  

- They were building dashboards and reports manually.  
- Compliance reviews required combining financial data with other corporate datasets.  
- Executives wanted self-service insights without waiting for IT.  

## Why Fabric Databases

To address this, the team evaluated SQL Mirroring vs. SQL in Fabric. While both great options, they migrated to SQL in Fabric because it provides OLTP + analytics in one SaaS platform so that they can gracefully retire the old app.

- **Direct integration** into Fabric’s analytics and governance.  
- **High compliance assurance** for financial data.  
- **Native Power BI and AI experiences** for self-service analytics.  

## Preparation

The SQL Scripts for the demo are in the repository, you will use the same data from the prior demo for this demo.

1. Confirm SQL database in Fabric is available in the Fabric capacity region.
1. Confirm Data Agents is enabled for your tenant.
1. Confirm Copilot tenant switch is enabled.
1. Confirm Cross-geo processing for AI is enabled.
1. Confirm Cross-geo storing for AI is enabled.
1. Create a Fabric workspace.
1. Create a SQL database in the workspace created.
1. Open the SQL database and run the seed scripts (you cannot do this in the sql analytics endpoint).
1. Create a Lakehouse
1. In the Lakehouse, add a shortcut to SQL in Fabric.
1. Create a Data Agent
1. Add SQL shortcut to data agent as a data source.
1. Select all tables as a data source.

## Setup

1. (Optional, in case you're short on time) Run a query to show some data.

| Demo | Goal(s) | Technologies | Recommended Time |
|---|---|---|---|
| Overview | Walk through data |  Copilot for SQL | 90s  |
| Data Agents | Demonstrate how schema changes don't require app changes | Fabric Data Agents |  90s |
| Power BI | Demonstrate how schema changes don't require app changes | Fabric Data Agents |  90s |

## Overview and SQL Copilot

1. Run a simple query
2. Open Copilot and ask "Which vendors have an overdue invoice of $5000 or higher"
3. Add query to the query editor and run the query.

## Data Agents

1. Note the data source, and point out that you can select individual tables to be used in the chat.
2. Ask: What is the total amount of overdue invoices by vendor and which vendor has the highest overdue balance or something similar, just be sure to test it before the session.
3. Show the SQL query that is generated in the response.

## Copilot for Power BI

1. Open up Power BI
2. Open Copilot in Power BI
3. Select one the existing prompts to generate a report.