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

To calculate hallucination probability, we simply have to find the probability of generating _undesired_ words. 
Let's assume that for each image we have this set of _undesired_ words and we call them hallucination vocabulary.
Given the hallucination vocab, $\mathcal{V}_h$ given the context $c_i$, hallucination 
hallucination probability is given by the following expression:




### Predictive uncertainity

You might have seen entropy as the measure of information. An alaternative interpratation of entropy 
is a measure of uncertainity. Entropy is expressed as follows:

$$ \begin{equation} H(x) = -\sum_i p(x_i)\:log(p(x_i))\end{equation} $$

To see the uncertainity interpretation of entropy, consider $p(.)$ as a uniform probability distribution. 
Uniform distribution has equality probability for all events, and therefore maximum randomness, implying 
maximum uncertainity. 

The total predictive uncertainity $H(x)$ can be broken down into two parts. Given the entire vocabulary, $\mathcal{V}$, 
let $\mathcal{V_h}$ be the hallucination vocabulary and $\mathcal{V}\ \mathcal{V_h}$ be the normal non-hallucination 
vocabulary. Then predictive uncertainity can be broken down into two pars as follows:
- Model's uncertainity matching the right token
- Uncertainity matching unsuitable tokens. This is directly proportional to hallucination probability

### Uncertainity decomposition
Historically, uncertainities have been decomposed into two parts:
- Epistemic uncertainity:
    Epistemic uncertainity corresponds to uncertainity associated with the model weights. For the rest of the article, 
    you can consider this as `model uncertainity`.
- Aleotoric uncertainity:
    This uncertainity is corresponds to the uncertainity associated with randomness in data or measure. You can think of 
    this as `random uncertainity`. 

### Evaluation

### Correlation between different uncertainities

### Reducing hallucinations

