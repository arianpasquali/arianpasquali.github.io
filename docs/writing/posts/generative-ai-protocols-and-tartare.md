---
authors:
- arianpasquali
categories:
- Applied AI
comments: true
date: 2025-04-17
description: Explore the shift from prompt engineering to context engineering in AI,
  emphasizing domain-specific evaluation workflows for robust AI systems.
draft: false
slug: generative-ai-protocols-and-tartare
tags:
- Generative AI
- Context Engineering
- Domain-Specific Evaluation
- AI Development
- AI Models
---

# From Prompt to Context Engineering: Why Evaluation is the Real AI Differentiator

Yesterday I had a fantastic dinner in London with Samuel Colvin the mind behind Pydantic (one of the most ubiquitous Python frameworks) and now focusing on PydanticAI and Logfire, Laura Modiano Strategic Partnerships Developer in Europe at OpenAI, David Soria Parra - Anthropic engineer behind the Model Context Protocol - Joon-sang Lee CEO of Pentaform, and industry legends Jason Liu and Ivan Leo - creators of [instructor](https://lnkd.in/ePaNSdQN) and Andreas Stathopoulos.

![Dinner](img/dinner.png)


I had a realization: everyone building generative AI agents and assistants is writing remarkably similar code. We're all building redundant data plumbing systems to manage context from data sources to agents, backends, and UIs.

Enought of AI data plumbing. The future and what will make or break your AI agents engineering is domain-specific evaluation.

Let’s acknowledge that we are at the infancy of this tech. As we get more mature, solutions like Anthropic's Model Context Protocol (MCP) are standardizing how we manage context and communicate AI with data sources more efficiently. If you are living under a rock and don’t know MCP please check [here](https://lnkd.in/eYr47tRc). 

We're evolving beyond prompt engineering concatenating strings to become what I like to call “context engineers”. Our primary job is finding the most relevant context to place in front of LLMs to answer user needs.

This context engineering for AI agents is fundamentally repetitive across domains. We're all:
- Deriving user questions into research plans using chain-of-thought reasoning
- Searching for relevant context
- Synthesizing answers

What struck me is where applied AI engineers should actually be focusing their time: building effective domain-specific evaluation workflows.

As I discussed in my previous posts, the AI adoption bottleneck for enterprise is not model capabilities, is the ability to prove (with statistical rigor) the accuracy of these systems to the specific domain. 

I have been expending most of my time building evaluation pipelines for user validation and it is hard. Not everyone has the luxury of having millions of users to AB test. At the enterprise level, the time you can borrow from domain experts for validation is scarse.

We need to shift our energy from repetitive data plumbing to building robust evaluation workflows and feedback loops. We should be assessing our systems' confidence when handling knowledge-specific topics and measuring accuracy with rigor.

This is where I want to allocate the majority of project budgets going forward. With MCP's exponential adoption across the industry, the plumbing problem is being solved. The differentiator will be how well we can evaluate and improve our systems in specific domains.

What are your thoughts? Are you seeing this shift in your AI projects? 

Also, I highly recommend checking [PydanticAI](https://ai.pydantic.dev/) 
And the AI Observality platform [Logfire](https://lnkd.in/e28Rieqs)