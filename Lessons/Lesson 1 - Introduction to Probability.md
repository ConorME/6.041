
--- 
lesson: 01 
topic: Probability 
date: 2024-11-19 
tags: [lecture, introduction, probability] 

---
## Overview:
An introduction to probability and the axioms of probability. This lesson establishes the basic framework for solving probability problems, defines what probability means, and introduces the fundamental axioms of probability theory.  

## Probability:
Probability is a mathematical model for reasoning about uncertainty. One way we can think of probabilities is as frequencies. If we a repeat an experiment with uncertain results the probability can be said to be the frequency of that specific outcome.

## Sample Space:
A sample space is a set of all possible outcomes of some experiment. The sample space can take on different forms, but we will typically be seeing Discrete sample spaces, like flipping a coin, or continuous sample spaces like the probability of landing on a specific point in space.

## Event:
An event is simply a subset of the sample space. These subsets are what probabilities are applied to. This can be almost anything. We can pick balls from bin and then ask what is the probability of a ball being yellow. In this case the event is 'the ball is yellow' and we have essentially infinite flexibility in what an event is. As long as we can define it well.


## Axioms: 

1. Non-negativity. $$ P(A) \geq 0$$
2. Normalization. $$P(\Omega) = 1 $$
3. Additivity. $$ \text{if } A \cup B \ne \emptyset \text{ then }P(A \cup B) = P(A) + P(B)$$

## Probability Laws:
The probability law of a specific probabilistic model is the rule that maps subsets of the sample space onto specific probabilities. There are several common patterns in probability laws and correctly modeling our situation is largely going to be a matter of determining out sample space and our probability laws and then answering any questions we may want to ask.

## Discrete Uniform Law:
One common probability law is the Discrete Uniform Law. This law lets every outcome of a sample space be equally likely then: $$ P(A) = \frac{|A|}{|\Omega|}$$

## Continuous Uniform Law:
In the case of continuous sample spaces, the **uniform law** assigns equal probability density across a specified interval. We can determine probability by calculating the area of the event. 