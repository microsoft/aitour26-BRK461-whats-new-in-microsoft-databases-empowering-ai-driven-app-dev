# Demo 3: Accounts Receivable Web App with Azure SQL

[🎬 Watch the video](https://aka.ms/AAxuglg)

Zava’s finance team manages a growing network of wholesale vendors. Their existing tools created bottlenecks when processing invoices, tracking payments, and generating financial reports. Compliance and auditability were difficult to maintain, slowing down innovation.

## Why Azure SQL

With Azure SQL, Zava modernized their AR system:

- **Secure by default**: Temporal tables track every change, Row-Level Security (RLS) enforces access policies, and Always Encrypted protects sensitive fields.
- **Developer productivity**: SQL’s structured queries simplify data access while Copilot and built-in tuning tools accelerate endpoint creation.
- **AI-ready**: The team can ask questions in natural language, with results translated into SQL queries by an AI agent.

## Setup

This demo can be run on Azure or locally. It's recommended to deploy on Azure for consistency.

1. Visit repository and verify you're on the `AI-Tour` branch before you fork/clone.
2. [Follow the getting started instructions]()
3. Download the MSSQL for VSCode extension.
4. After deployment, connect your database to the MSSQL extension.

## Preparation

1. Open the app in the browser
2. Open in VS Code (you can do this with or without the code)
3. Verify your database is connected to MSSQL and that GitHub Copilot is functional with the `@mssql` extension.
4. In the extension, right click on the database and select Chat in Ask mode.
5. You should see `@mssql` chat query editor pop up and GitHub Copilot greeting in the chat along with confirmation that your database is connected.
6. In the GitHub Copilot chat window ask, "Which 3 vendors have the highest credit limit?"
7. Add the response query into the empty query page and run the query.

| Demo | Goal(s) | Technologies | Recommended Time |
|---|---|---|---|
| GitHub Copilot | Demonstrate developer productivity and NL2SQL | VS Code, MSSQL extension, GitHub Copilot  |  90s |
| AR Web App | Demonstrate same output from GitHub Copilot | Langchain |  90s |

## GitHub Copilot

1. In the extension, right click on the database and select Chat in Ask mode.
1. You should see `@mssql` chat query editor pop up and GitHub Copilot greeting in the chat along with confirmation that your database is connected.
1. In the GitHub Copilot chat window ask, "Which 3 vendors have the highest credit limit?"
1. Add the response query into the empty query page and run the query.

## Accounts Receivable App

1. Ask the same question: "Which 3 vendors have the highest credit limit?"
2. The app should respond with the same vendor list.
3. Show the rest of the app, mention that the manager of the vendor relationship team is currently logged in, and note that when others log in they will only see the vendors assigned to them, thanks to row level security.
4. Mention that everything in this app was built in house and the team has been experimenting with ways to give the AR team more control over analyzing the financial data.

