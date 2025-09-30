<p align="center">
<img src="img/Banner-MS-AI-Tour-26.png" alt="decorative banner" width="1200"/>
</p>

# [Microsoft AI Tour 2026](https://aitour.microsoft.com)

## BRK461: Whats new in Microsoft databases: empowering ai-driven app dev

If you will be delivering this session, check the [session-delivery-sources](./session-delivery-resources/) folder for slides, scripts, and other resources.

### Session Description

This session explores the latest innovations in Microsoft’s database portfolio, focusing on how Azure Database for PostgreSQL, Azure Cosmos DB, Microsoft SQL, and Microsoft Fabric empower organizations to build AI-driven applications. Through the story of Zava, a rapidly evolving retailer, attendees will learn how to modernize fragmented data estates, integrate AI capabilities, and deliver scalable, secure, and intelligent solutions across retail, rewards, and finance scenarios. The session features practical demos, real-world architectures, and actionable guidance for developers and data professionals seeking to accelerate AI adoption with Microsoft databases.

### Learning Outcomes

By the end of this session, learners will be able to:

- Identify the strengths and use cases of Azure Database for PostgreSQL, Azure Cosmos DB, Microsoft SQL, and Microsoft Fabric for AI-driven app development. 
- Understand how to integrate native AI capabilities (vector search, agentic frameworks, REST endpoints) into modern applications.
- Design data architectures that support scalability, security, and rapid innovation across diverse workloads.

### Technologies Used and Covered

1. Azure Database for PostgreSQL
2. Azure Cosmos DB
3. Microsoft SQL
4. Microsoft Fabric


### Session Resources

| Resources          | Links                             | Description        |
|:-------------------|:----------------------------------|:-------------------|
| Additional Resources for this session | https://learn.microsoft.com | Links specific to this session |
| Postgres Agentic Shop Demo | https://github.com/Azure-Samples/postgres-agentic-shop | Retail app demo using PostgreSQL and AI agents |
| Cosmos DB Multi-Agent Workshop | https://github.com/AzureCosmosDB/banking-multi-agent-workshop/tree/ai-tour | Rewards chat app demo using Cosmos DB and AI agents |
| Semantic Kernel Connectors | https://learn.microsoft.com/en-us/semantic-kernel/concepts/vector-store-connectors/out-of-the-box-connectors/postgres-connector | Integrate PostgreSQL with Semantic Kernel |
| LangChain Integration | https://learn.microsoft.com/azure/postgresql/flexible-server/generative-ai-develop-with-langchain | Build agentic apps with LangChain and PostgreSQL |
| Azure AI Foundry Agent Service | https://learn.microsoft.com/azure/ai-services/content-safety/overview | Managed platform for building and deploying AI agents |

### Continued Learning Resources
| Resources          | Links                             | Description        |
|:-------------------|:----------------------------------|:-------------------|
| AI Tour 2026 Resource Center | https://aka.ms/AITour26-Resource-Center | Links to all repos for AI Tour 26 Sessions |
| Azure AI Foundry Community Discord | [![Microsoft Azure AI Foundry Discord](https://dcbadge.limes.pink/api/server/ByRwuEEgH4)](https://discord.gg/Pwpvf3TWaw)| Connect with the Azure AI Foundry Community! |
| Learn at AI Tour | https://aka.ms/LearnAtAITour | Continue learning on Microsoft Learn |

### 🌐 Multi-Language Support

Additional Languages coming soon!

## Content Owners

<table>
<tr>
    <td align="center"><a href="http://github.com/paladique">
        <img src="https://github.com/paladique.png" width="100px;" alt="Jasmine Greenawa
"/><br />
        <sub><b> Jasmine Greenaway
</b></sub></a><br />
            <a href="https://github.com/paladique" title="talk">📢</a> 
    </td>
    <td align="center"><a href="http://github.com/iemejia">
        <img src="https://github.com/iemejia.png" width="100px;" alt="Ismaël Mejía Useche
"/><br />
        <sub><b>Ismaël Mejía Useche
</b></sub></a><br />
            <a href="https://github.com/iemejia" title="talk">📢</a> 
    </td>
</tr></table>

## 

## Responsible AI 

Microsoft is committed to helping our customers use our AI products responsibly, sharing our learnings, and building trust-based partnerships through tools like Transparency Notes and Impact Assessments. Many of these resources can be found at [https://aka.ms/RAI](https://aka.ms/RAI).
Microsoft’s approach to responsible AI is grounded in our AI principles of fairness, reliability and safety, privacy and security, inclusiveness, transparency, and accountability.

Large-scale natural language, image, and speech models - like the ones used in this sample - can potentially behave in ways that are unfair, unreliable, or offensive, in turn causing harms. Please consult the [Azure OpenAI service Transparency note](https://learn.microsoft.com/legal/cognitive-services/openai/transparency-note?tabs=text) to be informed about risks and limitations.

The recommended approach to mitigating these risks is to include a safety system in your architecture that can detect and prevent harmful behavior. [Azure AI Content Safety](https://learn.microsoft.com/azure/ai-services/content-safety/overview) provides an independent layer of protection, able to detect harmful user-generated and AI-generated content in applications and services. Azure AI Content Safety includes text and image APIs that allow you to detect material that is harmful. Within Azure AI Foundry portal, the Content Safety service allows you to view, explore and try out sample code for detecting harmful content across different modalities. The following [quickstart documentation](https://learn.microsoft.com/azure/ai-services/content-safety/quickstart-text?tabs=visual-studio%2Clinux&pivots=programming-language-rest) guides you through making requests to the service.

Another aspect to take into account is the overall application performance. With multi-modal and multi-models applications, we consider performance to mean that the system performs as you and your users expect, including not generating harmful outputs. It's important to assess the performance of your overall application using [Performance and Quality and Risk and Safety evaluators](https://learn.microsoft.com/azure/ai-studio/concepts/evaluation-metrics-built-in). You also have the ability to create and evaluate with [custom evaluators](https://learn.microsoft.com/azure/ai-studio/how-to/develop/evaluate-sdk#custom-evaluators).

You can evaluate your AI application in your development environment using the [Azure AI Evaluation SDK](https://microsoft.github.io/promptflow/index.html). Given either a test dataset or a target, your generative AI application generations are quantitatively measured with built-in evaluators or custom evaluators of your choice. To get started with the azure ai evaluation sdk to evaluate your system, you can follow the [quickstart guide](https://learn.microsoft.com/azure/ai-studio/how-to/develop/flow-evaluate-sdk). Once you execute an evaluation run, you can [visualize the results in Azure AI Foundry portal ](https://learn.microsoft.com/azure/ai-studio/how-to/evaluate-flow-results).
