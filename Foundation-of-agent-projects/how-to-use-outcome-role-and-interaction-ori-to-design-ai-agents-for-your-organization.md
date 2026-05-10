# How to use Outcome, Role and Interaction (ORI) to design AI Agents for your organization

In the rapidly evolving landscape of artificial intelligence, designing effective [agent workflow systems](different-agent-workflow-patterns.md) requires a structured methodology that balances complexity with predictability. The **ORI (Outcome > Role > Interaction)** design approach offers a systematic framework for architecting AI agent workflows that are both powerful and practical.&#x20;

### Understanding the ORI Design Hierarchy

The ORI design approach follows a hierarchical structure where each element builds upon the previous:

1. **Outcome**: The desired result or objective of the agent system
2. **Role**: The specific functions and responsibilities assigned to each agent
3. **Interaction**: The protocols and patterns governing how agents communicate and collaborate

This hierarchy ensures that design decisions are driven by clear objectives rather than technological capabilities alone.

## Outcome-based design

There are essentially only two outcome-based designs when you design AI agents.&#x20;

Organizations typically start their AI agent journey with task-based agents due to their lower complexity and higher reliability.



### Task-based agents

Task-based agents represent the foundation of practical AI implementation in most organizations. Their popularity stems from several key advantages:

* **Predictability**: Well-defined task boundaries make behavior more deterministic
* **Measurability**: Clear success criteria for task completion
* **Scalability**: Easier to replicate and deploy across different contexts
* **Maintenance**: Simpler to debug and optimize

![Task based agents are going to be Organization favorites](/images/task_based_agents.png)

A prime example of task-based architecture is the **Monitoring Agent** pattern. These agents are designed to:

* Continuously observe specific metrics or systems
* Process incoming data against predefined criteria
* Trigger appropriate responses or alerts
* Maintain audit trails of their observations and actions



![A type of task based agent : Monitoring Agent](/images/monitoring_agent.png)



### Goal-seeking agents

Goal-seeking agents represent a more sophisticated approach to agent design, suitable for complex scenarios where the path to the desired outcome isn't clearly defined. These agents:

* Operate with greater autonomy
* Adapt to changing environmental conditions
* Make decisions based on multiple variables
* Collaborate dynamically with other agents

![Goal seeking Agent](/images/goal_seeking_agent.png)

Key characteristics of goal-seeking agents include:

1. **Dynamic Strategy Formation**: Agents can formulate and adjust their approaches based on environmental feedback
2. **Multi-Agent Collaboration**: Complex goal achievement often requires coordinated effort among multiple specialized agents
3. **Environmental Awareness**: Continuous monitoring and adaptation to changing conditions
4. **Learning Capabilities**: Improvement of strategies based on past experiences

Here is an  advanced type of goal-seeking agent which is useful for complex scenario use cases where the environment variables are unpredictable

![Simulation Agent, a type of Goal seeking Agent](/images/simulation_agent.png)

### Role-based design

Coming soon..

### Interaction-based design

Coming soon...



