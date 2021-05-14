---
layout: post
title: Recipes for Building an Open-Domain Chatbot
categories: [NLP, chatbots, Papers]
---

When was the last time you had a great conversation? A good conversation requires 
various skills: engaging talking points, exhibiting empathy etc. This article explores the 
the development of large scale models that can learn these skills for a open-domain chat. 
For more details, read the original [paper](https://www.aclweb.org/anthology/2021.eacl-main.24.pdf). 

## Task

A great conversational chatbot need to have smooth conversations that include the following traits: following 
the interlocuter and providing new points for discussions, exhibiting prior knowldege, empathy, personality, 
all while maintaining a consister persona.

### Metrics

- Automatic Evaluations:
    The automatic evaluation of the individual components included 4 different metrics:
    - Retriever: hits@1 for depth K (hits@1/K). This implies recall@1 while ranking among K candidates
    - Generator:
    - Retrieve and Refine (RetNRef):
    - Safety: 

- Self-chat Evaluations:


- Full Evaluations:


$$ \begin{equation} H(x) = -\sum_i p(x_i)\:log(p(x_i))\end{equation} $$

