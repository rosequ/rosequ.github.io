---
layout: post
title: On Hallucination and Predictive Uncertainty in Conditional Language Generation
categories: [NLP, NLG, Papers]
---

### What is Hallucination in NLG?

In Natural Language Generation, hallucination refers to the phenomenon where the model
generates false information not supported by input. 


For example, in the image caption task, if captions have descriptions not present in the image 
would indicate hallucination.


### Task: Image caption

The objective of the image caption task is to generate caption tokens y_1, y_2, ... given the 
input image x.

### Hallucination probability

Supposing we know in advance the hallucination vocab, V_h given the context c_i, hallucination 
hallucination probability is given by the following expression:



### Predictive uncertainity

You might have seen entropy as the measure of information. An alaternative interpratation of entropy 
is a measure of uncertainity.


