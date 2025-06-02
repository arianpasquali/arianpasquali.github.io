---
authors:
- arianpasquali
categories:
- AI Evaluation
comments: true
date: 2025-04-21
description: Explore how misalignment between LLM-as-Judge metrics and user preferences
  can impact evaluation accuracy and user satisfaction.
draft: false
slug: llms-as-judges-and-user-preference-correlation
tags:
- LLM
- AB Testing
- User Preferences
- Evaluation Metrics
- AI
---

# When LLM-as-Judge Metrics and User Preferences Diverge: Lessons from Real-World Evaluation

Why you should deeply understand what your LLM-as-a-Judge metric is actually measuring

When our automated evaluation metrics showed only 55% correctness for our LLM-generated answers, but users consistently preferred our system over 70% of the time, we knew something was off.

After deep analysis , we found that our Ragas-inspired correctness metric was actually penalizing our system for being 'too informative'. The metric counts additional facts beyond the ground truth as 'False Positives' - effectively punishing more comprehensive answers.

We changed the focus for another metric that according to our AB testing together with correlation analysis provided a more accurate picture.

This metric now categorises answers as:
- Subsets of expert validated answers (consistent but less comprehensive)
- Supersets of expert validated answers (consistent with additional information)
- Fully consistent/equivalent to expert validated answers
- In disagreement with expert validated answers

Using this approach, our actual factual accuracy jumps to 78%, much closer to what our user preference AB tests suggested.

Key takeways

1. 𝗕𝗲 𝗰𝗮𝗿𝗲𝗳𝘂𝗹 𝘄𝗶𝘁𝗵 𝗟𝗟𝗠-𝗮𝘀-𝗮-𝗝𝘂𝗱𝗴𝗲 𝗺𝗲𝘁𝗿𝗶𝗰𝘀: they may not align with what users actually value. Always calibrate your metrics with AB testing results. What the users prefer is more important than any LLM judge. 

2. 𝗔𝗹𝘄𝗮𝘆𝘀 𝘃𝗲𝗿𝗶𝗳𝘆 𝗰𝗼𝗿𝗿𝗲𝗹𝗮𝘁𝗶𝗼𝗻 between automated LLM metrics and user preferences through AB testing

Finally, the most accurate metric isn't always the most complex one. It's the one that best predicts user satisfaction. I cannot stress enough how you should focus on AB tests for that. 

Proper user AB testing is more important than any LLM-as-a-Judge metric.

Revisit and challenge your ground truth and your metrics periodically. Challenge the domain expert to validate and revisit your ground truth dataset whenever you detect misalignments like this.