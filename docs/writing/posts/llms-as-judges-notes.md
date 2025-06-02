---
authors:
- arianpasquali
categories:
- AI Evaluation
comments: true
date: 2025-04-30
description: Explore why relying solely on LLMs as judges isn't enough. Understand
  the importance of user preference over automated metrics.
draft: false
slug: llms-as-judges-notes
tags:
- LLMs
- AI Evaluation
- User Preference
- Automated Metrics
- Generative AI
---

# LLMs as Judges: Why Automated Metrics Aren't Enough

LLMs as Judges are just tools, not absolute truths.
In the context of generative AI systems, evals are sometimes misunderstood. Some people think that adding another framework, or LLM-as-judge metric will solve the problems and save the day.

I don't really care how high your "Factuality" or "Correctness" metrics are if users don't like the answers your system generates. If these metrics don't correlate with user preference, you have a bigger problem to solve.

LLM-as-judge are simply tools pointing to where we should look deeper.

Automated metrics help us identify weak spots in our systems that deserve human attention. That's it.

No fancy evaluation framework will magically solve your product problems.

What matters is the process. Build one that helps you monitor, annotate, measure what real users actually like and iterate. This process will be different in each organisation. How you sample the data to give to domain experts to validate and what "a correct answer" actually means in your case will depend on your context and internal processes. 

Remember, Evals aren’t static datasets or metrics. 

They’re a living process that enables you to apply the scientific method. 

Observe, annotate, create hypothesis, design experiments, measure, repeat.