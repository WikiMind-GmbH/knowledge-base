# Introduction to AI Agents

**Artificial Intelligence (AI) agents** are computer programs or systems that go beyond using a single large language model (LLM) or other AI models in isolation. While LLMs can generate human-like text and make predictions based on learned patterns, AI agents add an additional layer of autonomy and decision-making. Specifically, agents can:

1. **Perceive and interpret** their environment or context (e.g., receiving inputs from users, sensors, or APIs).  
2. **Reason and plan** dynamically, determining how best to use available models, tools, or data sources to accomplish objectives.  
3. **Act** by initiating tasks, calling APIs, or interacting with external systems to achieve specific goals.

By combining multiple models—or even multiple modes of input—AI agents can self-direct, continuously learn, and adapt to changing conditions. This transforms AI systems from purely reactive tools into proactive, versatile problem-solvers, driving innovation in areas like automation, customer support, and complex decision-making.

---

## Why Models Alone Aren’t Enough

While a single LLM can generate meaningful text and answer questions based on training data, real-world scenarios often demand **action** and **interaction** beyond text generation. Consider these practical examples:

1. **Customer Support Automation**  
   - **LLM-Only:** Can answer FAQs or provide generic troubleshooting steps.  
   - **Agent Added:** The agent can pull real-time data from internal CRM systems to check order status or user details, create support tickets automatically, and even escalate issues.

2. **Personal Scheduling Assistant**  
   - **LLM-Only:** Can suggest generic meeting times or give tips on time management.  
   - **Agent Added:** Directly accesses calendar APIs, proposes actual open time slots, and sends invitations to relevant contacts.

3. **E-Commerce Advisor**  
   - **LLM-Only:** Can offer product recommendations based on past training data.  
   - **Agent Added:** Connects to real-time inventory systems, fetches current prices, applies discount codes, and processes orders on behalf of the user.

4. **Data-Driven Decision Support**  
   - **LLM-Only:** Can provide summaries of best practices or general guidelines.  
   - **Agent Added:** Dynamically queries databases, generates custom analytical reports, and creates visualizations that drive actionable business insights.

In each of these scenarios, **LLMs are powerful for generating and interpreting language**, but **agents are necessary to combine that understanding with real-world actions**—pulling fresh data, interacting with external systems, and orchestrating complex processes. This synergy enables a **truly intelligent and autonomous AI solution** that moves beyond static responses to deliver tangible, context-aware outcomes.

---

## Overview of Different Kinds of AI Agents

AI agents can be categorized based on how they perceive and act within their environments, the complexity of their internal models, and their learning capabilities.

Antrophic has the following useful definition:

>At Anthropic, we draw an important architectural distinction between workflows and agents:
>
> Workflows are systems where LLMs and tools are orchestrated through predefined code paths.  
> Agents, on the other hand, are systems where LLMs dynamically direct their own processes and tool usage, maintaining control over how they accomplish tasks.


In this repo we will explore both types of agentic systems in detail.

Start with:

[Workflows](workflows/)

Then continue with:

[Agents](agents/)

## General Advice

When considering solutions involving LLMs, we recommend starting with the simplest possible approach and only increasing complexity when necessary. Sometimes, this might mean not using LLMs at all or forgoing agentic systems altogether. Both AI in general and agentic systems in particular often involve trade-offs between complexity, latency, and cost in pursuit of better task performance, so consider carefully whether those trade-offs are worth making.

While AI systems can be tremendously powerful when greater complexity is needed, not every use case is so complex that a conventional software solution wouldn't suffice. Reflect on whether you truly need AI in the first place. An AI-powered calculator, for example, makes little sense. If you determine that AI capabilities are indeed essential, start by exploring whether a single LLM call might solve the problem. In many scenarios, a single LLM call—possibly with retrieval and in-context examples—proves sufficient. Move on to agentic systems only if those simpler methods are inadequate.

When agentic systems do become necessary, keep in mind that predefined workflows offer predictability and consistency for well-defined tasks, whereas agents excel in situations requiring flexibility and model-driven decision-making at scale.
