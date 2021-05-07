---
layout: post
title: On Hallucination and Predictive Uncertainty in Conditional Language Generation
categories: [NLP, NLG, Papers]
---

This blogpost explores the relationship between predictive uncertainity and language generation, 
and the correlation between uncertainity and hallucination in NLG. For more details, read the 
original [paper](https://arxiv.org/abs/2103.15025). 

### What is Hallucination in NLG?

In Natural Language Generation, hallucination refers to the phenomenon where the model
generates false information not supported by input. 


For example, in the image caption task, if captions have descriptions not present in the image 
would indicate hallucination.


### Task: Image caption

The objective of the image caption task is to generate caption tokens $y_1, y_2, ...$ given the 
input image $x$.

### Hallucination probability

Supposing we know in advance the hallucination vocab, $\mathcal{V}_h$ given the context $c_i$, hallucination 
hallucination probability is given by the following expression:




### Predictive uncertainity

You might have seen entropy as the measure of information. An alaternative interpratation of entropy 
is a measure of uncertainity. Entropy is expressed as follows:

$$ \begin{equation} H(x) = -\sum_i p(x_i) log(p(x_i))\end{equation} $$

To see the uncertainity interpretation of entropy, consider $p(.)$ as a uniform probability distribution. 
Uniform distribution has equality probability for all events, and therefore maximum randomness, implying 
maximum uncertainity. 


### Uncertainity decomposition

### Evaluation

### Correlation between different uncertainities

### Reducing hallucinations

