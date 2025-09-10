# Demo 2: Azure Cosmos DB Rewards App

[🎬 Watch the video](https://aka.ms/AAxuglj)

The Zava Tech team is modernizing their Customer Rewards Program by introducing a self-serve AI-powered chat app. Today, customers have no direct way to check balances or redeem rewards on their own. The new app allows them to manage their rewards, ask questions about earning and cashing out points, and get real-time personalized responses.

The workload is demanding:

* On a typical day, ~10,000 customers are active.
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

This demo can be run on Azure, Codespaces or locally. It's recommended to deploy on Azure for consistency. Please note that this demo is **Python only**

1. Visit repository and verify you're on the `ai-tour` branch before you fork/clone/open in Codespace.
2. [Follow the getting started instructions](https://github.com/AzureCosmosDB/banking-multi-agent-workshop/tree/ai-tour/python#getting-started)

## Preparation

In the Browser:

1. Open the Cosmos DB Data Explorer in the Azure Portal.
2. Open demo app, select `Kian Lambert` and `Zava Personal`, then login. These values should pre-populate on loading.
3. Open Container App Log Stream.

| Demo | Goal(s) | Technologies | Recommended Time |
|---|---|---|---|
| Overview | Walk through Chat interface, Show Cosmos DB LangGraph integration |  Python, LangGraph | 90s  |
| Schema Flexibility | Demonstrate how schema changes don't require app changes | Cosmos DB NoSQL |  90s |

## Overview (30 seconds)

1. Starting in the chat interface, "What Zava personal offers are available in Europe?".
2. The Redemption agent should say that there are no offers available in Europe.
3. Show the agents being called in logstream, point out how the redemption agent is answering the question
4. (Optional) Walk through the agent code in `rewards_agents.py` and the vector search query in `azure_cosmos_db.py` (around line 56)

### Talking points

- LangGraph
- Agent Architecture
- Agent Responsibilities

## Schema flexibility (no migrations)

In this demo Zava is expanding to Europe. You'll be adding this region to a few of the offer terms. This is what the offer term data looks like:

```json
  {
    "id": "OfferTerm2",
    "tenantId": "Zava Personal",
    "offerId": "Offer2",
    "region": ["North America"],
    "name": "Zava Vacation Saver Terms",
    "text": "Travel redemptions may include blackout dates, and taxes or fees may apply separately.",
    "type": "Term",
    "accountType": "Personal",
    "vector": [...]
  }
```

1. In the Cosmos DB Explorer, navigate to `OffersData` > `Items`
2. Add `"Europe"` to the `region` field in 1-2 `OfferTerm` items.
3. In the chat app, create a new chat session.
4. Ask what offers are available to users again: "What Zava personal offers are available in Europe?".
5. Response should include regional offers.

### Talking points

- In Cosmos DB Each document can have different fields — in this case, offers with region information.
- Cosmos DB’s flexible partitioning model makes mutlitenancy seamless so customers with multiple accounts to see all their rewards in one place.