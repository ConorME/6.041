lesson: 03
topic: Probability 
date: 2024-11-21 
tags: [lecture, probability] 

## Review:
Give the definitions for the three equations related to conditional probality from the last lesson.

1. The multiplication rule. When we are dealing with conditional probabilities and we are interested in the probability of a single leaf in our conditional probability tree. We can apply the multiplication rule. As follows: $$ P(A \cap B) = P(A)P(B | A)$$
2. The Total Probability Law is applied when we want to know the probability of an event that occurs across multiple branches of our conditional probability tree: $$P(A) = \sum_i P(B_i)P(A|B_i)$$
3. Bayesian Inference is a systematic way for us to update our initial beliefs when new information has been presented to us. This is a simple equation found by using the two above formulas. : $$P(A_i | B) = \frac{P(A_i \cap B)}{P(B)} = \frac{P(A_i)P(B|A_i)}{\sum_jP(A_j)P(B|A_j)}$$
## Models based on Conditional Probabilities:
A tree based structure is a good way of modeling conditional probabilities. It allows us to work sequentially where every edge is a conditional probability and every node represents the outcome of those edges, also known as the intersection. If we consider a series of fair coin flips we can model this system using our tree based model. We can represent an arbitrary number of coin flips as a tree of potential outcomes where every leaf represents a different sequence and every edge represents the conditional probability of heads or tails given the previous result. This gives us a very simple model for solving problems of conditional probabilities, but gives us our first introduction to the idea of independence.

## Independence of Two Events:
Two events are said to be independent if the conditional probability if the condition of one event does not change the probability of the other event.

Definition: $$P(B|A) = P(B) $$
Recall that the probability of the intersection is given by the following: $$P(A \cap B)= P(A)P(B|A)$$
We will tend to use the following definition instead: $$ P(A \cap B) = P(A)P(B)$$
## Conditioning May Effect Independence:
The introduction of a condition may result in two independent events becoming tightly coupled. For example if a condition occurs in which either one or the other event occur exclusively then the occurrence of one event causes the other event to become impossible, which implies that either condition changes the probability  of the other.


## Independence of Collections of events:
Definitions: Events $A_1, A_2, ... , A_n$ are called independent if: $$ P(A_i\cap A_j \cap \dots \cap A_q) = P(A_i)P(A_j)\dots P(A_q)$$
For distinct indices, $i, j, \dots , q \in \{1,  \dots , n\}$

## Pairwise Independence: 
Suppose we have a set of events and those events are pairwise independent. That is that any two events do not impact the probability of the other. It can be shown that this does not imply independence across the entire set.


