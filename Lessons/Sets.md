Probability makes extensive use of sets operations. This review introduces notation and terminology. 

A set is a collection of unique elements. If $S$ is a set and $x$ is an element of $S$ we write $x \in S$. If $x$ is not in $S$ we write $x \notin S$. A set can have no elements, in which case we refer to it as a special case called the **empty set**, denoted by $\varnothing$.   

## Specifying Sets
Sets can be specified in a number of ways. If S contains a finite number of elements $x_1, x_2, \dots , x_n$, we write $S$ as a list of elements, in braces: $$S = \{x_1, x_2, \dots , x_n\} $$
The sample space of a all possible outcomes of a die roll is given by $S = \{1, 2, 3, 4, 5, 6\}$, and sample space of a coin toss is given by $\{H,T\}$. 

If $S$ contains infinitely many elements then it can be enumerated as a list: $$S = \{x_1, x_2, ...\}$$
Then we say the $S$ is countably infinite. We can also specifiy the elements of a set based on certain conditions. For example: $$S = \{x | x \text{ is even}\}$$ denotes the set of all numbers $x$ such that $x$ satisfies the property. 
## Subsets
If every element of $S$ is also an element of another set $T$ we say that $S$ is a subset of $T$, denoted $S \subset T$. If $S \subset T$ and $T \subset S$ then we say that $S = T$. We also introduce the universal set $\Omega$, which denotes the collection of elements that could conceivably of interest to us in a particular context. Having specified the context in terms of a universal set $\Omega$, we only consider the sets $S$ that are subsets of $\Omega$. 

## Set Complement
The complement of a set, with respect to the universe $\Omega$, is the set $\{x \in \Omega | x \notin S\}$ of all elements of the universal set that do not belong to $S$, and is denoted $S^C$. Notably $\Omega^C = \varnothing$. 

## Union and Intersection
The union of two sets $S, T$ is the set of all elements which belong to either $S$ or $T$, denoted $S \cup T$. The intersection of two sets is the set of all elements which belong to $S$ and $T$, denoted $S \cap T$. Thus: $$S \cup T = \{x|x \in S \text{ or } x \in T\}$$and $$S \cap T = \{x|x \in S \text{ and } x \in T\}$$
## Repeated and Infinite Unions
In same cases we may want to consider the union or intersection of several, or infinitely many sets, defined in some obvious way. If we consider the the set of positive integer we are given a set $S_n$: $$\bigcup_{n=1}^{\infty} S_n = S_1 \cup S_2 \cup \dots = \{ x \mid x \in S_n \text{ for some } n \}.
$$
and $$\bigcap_{n=1}^{\infty} S_n = S_1 \cap S_2 \cap \dots = \{ x \mid x \in S_n \text{ for all } n \}.
$$
## Disjoint Sets
Two sets are said to be disjoint if their intersection is empty. More generally several sets are said to be disjoint if no two of them contain a common element. 

## Partitions
A collection of sets is said to be a partition of a set $S$ if the sets in the collection are disjoint and their union is $S$. 

## Ordered Pairs
If $x,y$ are two elements. We use $(x,y)$  to denote the ordered pair of $x$ and $y$. The set of scalars is denoted by $\mathbb{R}$; the set of pairs (or triplets) of scalars, i.e., the two-dimensional plane (or three dimensional space, respectively) is denoted by $\mathbb{R}^2$ (or $\mathbb{R}^3$, respectively). 

## The Algebra of Sets
Set operations have several consequences, which are elementary consequences of the definitions. 
$$\begin{align*}
\text{Commutativity:} & \quad A \cup B = B \cup A, \quad A \cap B = B \cap A \\[8pt]
\text{Associativity:} & \quad (A \cup B) \cup C = A \cup (B \cup C), \quad (A \cap B) \cap C = A \cap (B \cap C) \\[8pt]
\text{Distributivity:} & \quad A \cap (B \cup C) = (A \cap B) \cup (A \cap C), \quad A \cup (B \cap C) = (A \cup B) \cap (A \cup C) \\[8pt]
\text{Identity:} & \quad A \cup \varnothing = A, \quad A \cap \Omega = A \\[8pt]
\text{Domination:} & \quad A \cup \Omega = \Omega, \quad A \cap \varnothing = \varnothing \\[8pt]
\text{Idempotence:} & \quad A \cup A = A, \quad A \cap A = A \\[8pt]
\text{Complementation:} & \quad A \cup A^C = \Omega, \quad A \cap A^C = \varnothing \\[8pt]
\text{De Morgan's Laws:} & \quad (A \cup B)^C = A^C \cap B^C, \quad (A \cap B)^C = A^C \cup B^C
\end{align*}
$$

Generally De Morgan's laws can be given as follows:
$$\begin{align*}
\left(\bigcup_{n=1}^{\infty} S_n\right)^C &= \bigcap_{n=1}^{\infty} S_n^C, \\[8pt]
\left(\bigcap_{n=1}^{\infty} S_n\right)^C &= \bigcup_{n=1}^{\infty} S_n^C.
\end{align*}
$$
which is a particularly useful property. 