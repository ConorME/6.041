---

---

lesson: 02
topic: Probability 
date: 2024-11-19 
tags: [lecture, probability] 

## Conditional Probability:
Conditional probability is a definition. Not a theorem. When given some new information we want to update our model with this new information. Conditional probability allows us to calculate the probability of an event given that another event has occurred. Mathematically we can write this: $$ P(A|B) = \frac{P(A \cap B)}{P(B)} $$ This definition makes sense. If B has occurred then we can calculate the probability of A occurring by finding the fraction of B that is occupied by its intersection with A. 

## Examples of Conditional Probability:
Consider the example with two die rolls, x and y. Let B be the event: min(x, y) = 2. And let M = max(x,y). Then what is the probability of M = 1 if B has occurred? We know that if B has occurred then the possible outcomes for our event take the form (2, y) or (x, 2) where x,y > 2. Thus P(M = 1 | B ) = 0 since, the intersection contains no elements. What about P(M = 2 | B)? In this example we can analyze a diagram. Again the form must be (2, y) or (x, 2), thus the probability P(M = 2 | B ) is simply the number of outcomes in the intersection divided by the number of outcomes in event B. In this case, this is only the single value (2, 2). 

## Models on Conditional Probability:
There are three very common questions we encounter when discussing conditional probability. We likely want to know the probability that an event A occurs and an event B occurs (the intersection), the probability that the event B occurs, or the conditional probability that A will occur given that B has already occurred. We can determine these values by looking at tree structures where each node is an event and each edge is weighted by the probability of that event occurring. We can find the probability of the intersection by re-arranging the formula for conditional probability: $$P(A \cap B) = P(B)P(A | B) = P(A)P(B|A)$$
Similarly we can find P(B): $$ P(B) = \frac{P(A \cap B)}{P(A|B)}$$
Lastly we can calculate P(A | B) from the above two formulas using our formula for conditional probability: $$P(A | B) = \frac{P(A \cap B)}{P(B)}$$

## Multiplication Rule:
The multiplication rule is a rule for calculating repeated conditional probabilities. We may notice that we can calculate the probability of intersections by simply multiplying the probability of event B with the probability of A given that B has occurred. We can expand this idea to three intersection. $$P(A \cap B \cap C) = P(A)(P(B|A)P(C | A \cap B)$$
This pattern repeats allowing us to generalize this notion of repeated events into a simple multiplication rule for the probabilities of intersections.

## Total Probability Theorem:
The total probability theorem governs finding the probability of an event where the sample space is partitioned. We can compute the probability of an event B by finding the sum of the probabilities of B given that $A_i$ has occurred:
$$ P(B) = \sum_i P(A_i)P(B | A_i) $$
This makes sense. If there is a chance that B occurs given that $A_i$ has occurred then each portion of B lies within one of the $A_i$ events. By summing them together we are able to add up the total probability of the event B. 

## Bayesian Inference:
Bayesian inference offers us a systematic way of updating our beliefs about a system. We begin with a set of initial beliefs $P(A_i)$. We know $P(B|A_i)$ for each i. But we suddenly discover that B has occurred. How can we revise our initial beliefs $A_i$? Essentially we now wish to computer $P(A_i| B)$:
$$ P(A_i|B)= \frac{P(A_i \cap B)}{P(B)} = \frac{P(A_i)P(B|A_i)}{P(B)} = \frac{P(A_i)P(B|A_i)}{\sum_j P(A_j)P(B|A_j)}$$
