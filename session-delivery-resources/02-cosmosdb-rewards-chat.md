# Demo 2: Azure Cosmos DB Rewards App

The Zava Tech team is modernizing their Customer Rewards Program by introducing a self-serve AI-powered chat app. Today, customers have no direct way to check balances or redeem rewards on their own. The new app allows them to manage their rewards, ask questions about earning and cashing out points, and get real-time personalized responses.

The workload is demanding:

* On a typical day, \~10,000 customers are active.
* During campaigns like “double points” days, activity surges past 100,000 users.
* The program evolves weekly, with new rewards and tiering rules added on the fly.

To meet these challenges, Zava’s developers require a **scalable, globally distributed, AI-ready database** that can adapt as fast as the business.

## Why Cosmos DB

* **Multitenancy support:** The chat app allows customers with multiple accounts to see all their rewards in one place. Cosmos DB’s flexible partitioning model makes this seamless.
* **Schema flexibility:** Cosmos DB’s JSON model allows Zava to add or remove fields without schema migrations or downtime.
* **Global distribution with low latency:** Data is automatically distributed across regions, ensuring customers get responsive experiences anywhere in the world.
* **Hybrid retrieval for AI:** Developers can combine scalar, range, and geospatial filters with vector similarity search and keyword search in a single query for powerful AI workflows.
* **Performance at scale:** Cosmos DB scales elastically without compromising throughput or latency.

## Setup

This demo can be run on Azure or locally. It's recommended to deploy on Azure for consistency.

1. Visit repository and verify you're on the `ai-tour` branch before you fork/clone/open in Codespace.
2. [Follow the getting started instructions](https://github.com/AzureCosmosDB/banking-multi-agent-workshop/tree/ai-tour/python#getting-started)

## Demo Steps

## Talking Points