---
icon: hand-wave
layout: central
---

# Welcome to the Agent Project

A practical guide written by practitioners to help get your Agents running securely in production.

Given the many confusing options, [<mark style="background-color:yellow;">https://www.AgentProject.ai</mark>](https://www.agentproject.ai) aims to guide you through the choices, tools, and best practices to ensure your Agent project runs securely in production.

The github repo is here : [https://github.com/AgentProject-AI/agentproject](https://github.com/AgentProject-AI/agentproject)

### Topics covered here

(Please note that these are work-in-progress topics and will be filled out as we get experienced folks helping us out). The team is currently focused on building this out
[<mark style="background-color:yellow;">**[Top 10 AI Agent Security and Governance Controls (OWASP Style)</mark>](security/Top-10-AI-Agent-Security-and-Governance-Controls.md)** :thumbsup:

### Part 1: Foundations of Agent Projects

* **Introduction to Agent AI:**
  * [Key functional areas of an AI agent](foundation-of-agent-projects/the-key-functional-areas-of-an-ai-agent.md)
  * [Different AI agent workflow implementation patterns](foundation-of-agent-projects/different-agent-workflow-patterns.md)
    * What type of AI agents are right for you
  * [How to think about designing and blueprinting agents in your organization using ORI design](foundation-of-agent-projects/how-to-use-outcome-role-and-interaction-ori-to-design-ai-agents-for-your-organization.md)
  * The transformative potential of AI agents in various industries.
  * Understanding the core challenges in building and deploying AI agents.
* **Core Challenges in Agent Projects:**
  * **Reliability**: Managing unpredictable outputs from AI agents and their implications on system design.
  * **Orchestrating**: Multiple agent orchestration to achieve complex goals
  * **Discovery:** How to publish your Agent and make it findable
  * **Trust:** How to trust an Agent across your organization and from the outside
  * **Real-Time and near real-time Processing Demands**: Designing agents for low-latency execution and high throughput applications
  * **Data Handling at Scale:** Efficient processing of large datasets and external knowledge sources
  * **Testing Complexity**: Adapting testing methodologies for non-deterministic Agentic systems.
  * **Agent Observability**: Addressing the complexities of evaluating AI agent performance.



### Part 2: Securing Your Agent Project in Production
* [<mark style="background-color:yellow;">**[Top 10 AI Agent Security and Governance Controls (OWASP Style)</mark>](security/README.md)** :thumbsup:
* **Deployment Strategies:**
  * Considerations for deploying agent applications.
  * Containerization and orchestration.
  * API endpoints for accessing agent services.
  * Implementing caching strategies to optimize performance.
* **Security Strategies:**
  * Resource Access Delegation
  * Controlled access to computing resources
  * Token-based delegation for API and service access
  * Memory and storage allocation permissions
  * Network access controls and limitations
  * Controlled sub-task delegation between agents
  * Permission inheritance rules
  * Chain of authority tracking
* **Monitoring and Logging:**
  * Importance of monitoring and audit logs in AI systems.
  * Setting up logging and metrics for performance tracking.
  * Using tools like LangTrace, OpenLit and Portkey.
  * Collecting data for evaluation and system improvement.
* **Evaluation and Testing**:
  * **Building robust evaluation frameworks**.
  * Goal-based testing for agent projects.
  * AUTs: Profile-based Agent-unit-testing
  * Using automated testing and metrics.
  * Incorporating human feedback in the evaluation loop.
  * Ad-hoc and offline evaluation methods.
* **Ensuring Reliability and Safety:**
  * Addressing common safety issues in agent behavior.
  * Implementing content filtering, input validation, and output sanitization.
  * Using safety guards and monitoring alerts.
  * Best practices for building reliable and safe agent systems.
* **Cost Optimization:**
  * Understanding LLM costs and token optimization.
  * Implementing caching strategies and other cost-saving measures.
  * Choosing cost-effective models and deployment options.
* **Iterative Improvement:**
  * The importance of continuous monitoring and improvement of agent applications.
  * Using data and feedback to refine and optimize agent behavior.
  * Integrating evaluation into the development cycle.


