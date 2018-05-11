### 9.1 Relations and Their Properties

p594
Ex: 1-16, 20

>Definition 1
Let $A$ and $B$ be sets. A binary relation $R$ from $A$ to $B$ is a subset of $A \times B$.
$$
\begin{aligned}
A \times B &= \{(a, b) \mid a\in A \land b \in B\}\\
R &\subseteq A \times B
\end{aligned}
$$

Example 1
Let $A$ be the set of students in your school, and let $B$ be the set of courses. Let $R$ be the relation that consists of those pairs $(a, b)$, where $a$ is a student enrolled in course $b$. For instance, if Jason Goodfriend and Deborah Sherman are enrolled in CS518, the pairs _(Jason Goodfriend, CS518)_ and _(Deborah Sherman, CS518)_ belong to $R$. If Jason Goodfriend is also enrolled in CS510, then the pair _(Jason Goodfriend, CS510)_ is also in $R$. However, if Deborah Sherman is not enrolled in CS510, then the pair _(Deborah Sherman, CS510)_ is not in $R$.
Note that if a student is not currently enrolled in any courses there will be no pairs in $R$ that have this student as the first element. Similarly, if a course is not currently being offered there
will be no pairs in $R$ that have this course as their second element.

Example 2
Let $A$ be the set of cities in the U.S.A., and let $B$ be the set of the 50 states in the U.S.A. Define the relation $R$ by specifying that $(a, b)$ belongs to $R$ if a city with name $a$ is in the state $b$. For instance, _(Boulder, Colorado)_, _(Bangor, Maine)_, _(Ann Arbor, Michigan)_, _(Middletown, New Jersey)_, _(Middletown, New York)_, _(Cupertino, California)_, and _(Red Bank, New Jersey)_ are in $R$.

>Definition 2
A relation on a set $A$ is a relation from $A$ to $A$.
$$
\begin{aligned}
R &\subseteq A \times A = A^2
\end{aligned}
$$

#### Properties of Relations
+ Reflexive
+ Symmetric
+ Antisymmetric
+ Transitive

>Definition
A relation $R$ on a set $A$ is called _reflexive_ if $(a, a) \in R$ for every element $a \in A$.
$$
\begin{aligned}
\forall a((a, a) \in R)
\end{aligned}
$$

EXAMPLE 7
Consider the following relations on $\{1, 2, 3, 4\}$:
$R_1 = \{(1, 1), (1, 2), (2, 1), (2, 2), (3, 4), (4, 1), (4, 4)\}$,
$R_2 = \{(1, 1), (1, 2), (2, 1)\}$,
$R_3 = \{(1, 1), (1, 2), (1, 4), (2, 1), (2, 2), (3, 3), (4, 1), (4, 4)\}$,
$R_4 = \{(2, 1), (3, 1), (3, 2), (4, 1), (4, 2), (4, 3)\}$,
$R_5 = \{(1, 1), (1, 2), (1, 3), (1, 4), (2, 2), (2, 3), (2, 4), (3, 3), (3, 4), (4, 4)\}$,
$R_6 = \{(3, 4)\}$.
Which of these relations are reflexive?
>Solution
The relations $R_3$ and $R_5$ are reflexive because they both contain all pairs of the form $(a, a)$, namely, $(1, 1)$, $(2, 2)$, $(3, 3)$, and $(4, 4)$. The other relations are not reflexive because they do not contain all of these ordered pairs. In particular, $R_1, R_2, R_4$, and $R_6$ are not reflexive because $(3, 3)$ is not in any of these relations.

>Definition
A relation $R$ on a set $A$ is called _symmetric_ if $(b, a) \in R$ whenever (a, b) \in R, for all $a, b \in A$. A relation $R$ on a set $A$ such that for all $a, b \in A$, if $(a, b) \in R$ and $(b, a) \in R$, then $a = b$ is called _antisymmetric_.
$$
\begin{aligned}
\forall a \forall b ((a, b) \in R &\to (b, a) \in R) &\text{Symmetric}\\
\forall a \forall b ((a, b) \in R \land (b, a) \in R) &\to (a=b)) &\text{Antisymmetric}\\
\end{aligned}
$$

EXAMPLE 12
Is the “divides” relation on the set of positive integers symmetric? Is it antisymmetric?
_Solution_: This relation is not symmetric because $1 \mid 2$, but $2 \nmid 1$. It is antisymmetric, for if a and b are positive integers with $a \mid b$ and $b \mid a$, then a = b (the verification of this is left as an exercise for the reader).

> Definition
A relation $R$ on a set $A$ is called _transitive_ if whenever $(a, b) \in R$ and $(b, c) \in R$, then $(a, c) \in R$, for all $a, b, c \in A$.
$$
\begin{aligned}
\forall a \forall b \forall c (((a, b) \in R \land (b, c) \in R) \to (a, c) \in R)
\end{aligned}
$$

EXAMPLE 15
Is the “divides” relation on the set of positive integers transitive?
_Solution_: Suppose that $a$ divides $b$ and $b divides c$. Then there are positive integers $k$ and $l$ such that $b = ak$ and $c = bl$. Hence, $c = a(kl)$, so $a$ divides $c$. It follows that this relation is transitive.

EXAMPLE 16
How many reflexive relations are there on a set with $\mathsf{n}$ elements?
_Solution_: A relation $R$ on a set $A$ is a subset of $A\times A$. Consequently, a relation is determined by specifying whether each of the $n^2$ ordered pairs in $A \times A$ is in $R$. However, if $R$ is reflexive, each of the $n$ ordered paries $(a, a)$ for $a \in A$ must be in $R$. Each of the other $n(n-1)$ ordered pairs of the form $(a, b)$, where $a\ne b$, may or may not be in $R$. Hence, by the product rule form counting, there are $2^{n(n-1)}$ reflexive relations [this is the number of ways to choose whether each element (a, b), with $a \ne b$, belongs to $R$].

#### Combining relations
> Definition
Let $R$ be a relation from a set $A$ to a set $B$ and $S$ a relation from $B$ to a set $C$. The _composite_ of $R$ and $S$ is the relation consisting of ordered pairs $(a, c)$, where $a \in A, c \in C$, and for which there exists an element $b \in B$ such that $(a, b) \in R$ and $(b, c) \in S$. We denote the composite of R and S by $S \circ R$.

EXAMPLE 20
What is the composite of the relations R and S, where R is the relation from $\{1, 2, 3\}$ to $\{1, 2, 3, 4\}$ with $R = \{(1, 1), (1, 4), (2, 3), (3, 1), (3, 4)\}$ and $S$ is the relation from $\{1, 2, 3, 4\}$ to $\{0, 1, 2\}$ with $S = \{(1, 0), (2, 0), (3, 1), (3, 2), (4, 1)\}$?
_Solution_: $S \circ R$ is constructed using all ordered pairs in $R$ and ordered pairs in $S$, where the second element of the ordered pair in $R$ agrees with the first element of the ordered pair in $S$. For example, the ordered pairs $(2, 3)$ in $R$ and $(3, 1)$ in $S$ produce the ordered pair $(2, 1)$ in $S \circ R$. Computing all the ordered pairs in the composite, we find
$$
\begin{aligned}
S \circ R = \{(1,0), (1, 1), (2, 1), (2, 2), (3, 0), (3, 1)\}
\end{aligned}
$$

#### Homework
p602: 3c-f, 9, 25, 32

3\. For each of these relations on the set $\{1, 2, 3, 4\}$, decide whether it is *reflexive*, whether it is *symmetric*, whether it is *antisymmetric*, and whether it is *transitive*.
c) $\{(2, 4), (4, 2)\}$
>Solution
Let $R$ be the relation.
*Reflective* - No.  $(1, 1) \notin R$.
*Symmetric* - Yes. $(2, 4) \in R \land (4, 2) \in R$.
*Antisymmetric* - No. $(2, 4) \in R \land (4, 2) \in R \land 2\ne 4$.
*Transitive* - No. $(2, 4) \in R \land (4, 2) \in R \land (2, 2) \notin R$.

d) $\{(1, 2), (2, 3), (3, 4)\}$
>Solution
Let $R$ be the relation.
*Reflective* - No. $(1, 1) \notin R$.
*Symmetric* - No. $(1, 2) \in R \land (2, 1) \notin R$.
*Antisymmetric* - Yes. $(2, 1) \notin R \land (3, 2) \notin R \land (4, 3) \notin R$.
*Transitive* - No. $(1, 2) \in R \land (2, 3) \in R \land (1, 3) \notin R$.

e) $\{(1, 1), (2, 2), (3, 3), (4, 4)\}$
>Solution
Let $R$ be the relation.
*Reflective* - Yes. $(1, 1) \in R \land (2, 2) \in R \land (3, 3) \in R \land (4, 4) \in R$.
*Symmetric* - Yes. $(1, 1) \in R \land (2, 2) \in R \land (3, 3) \in R \land (4, 4) \in R$.
*Antisymmetric* - Yes. $\forall a \forall b((a, b) \in R \land (b, a) \in R \to (a=b))$.
*Transitive* - Yes. $(1, 2) \in R \land (2, 3) \in R \land (1, 3) \notin R$

f) $\{(1, 3), (1, 4), (2, 3), (2, 4), (3, 1), (3, 4)\}$
Let $R$ be the relation.
>Solution
*Reflective* - No. $(1, 1) \notin R$.
*Symmetric* - No. $(1, 4) \in R \land (4, 1) \notin R$.
*Antisymmetric* - No. $(1, 3) \in R \land (3,1) \in R \land 1 \ne 3$.
*Transitive* - No. $(1, 3) \in R \land (3, 1) \in R \land (1, 1) \notin R$

9\. Show that the relation $R = \emptyset$ on the empty set $S = \emptyset$ is reflexive, symmetric, and transitive.
>Solution
Because the assumption that there are elements in $S\times S = \emptyset$ is false, the conclusion that $R$ is reflexive, symmetric and transitive is always true.

25\. How many different relations are there from a set with $m$ elements to a set with $n$ elements?
>Solution
Let the set with $m$ elements be $A$, and the set with $n$ elements be $B$.
1\. A relation from $A$ to $B$ is a subset of $A \times B$.
2\. By product rule, $A\times B$ has $mn$ elements, so it has $2^{mn}$ subsets.
3\. Thus there are $2^{mn}$ relations from $A$ to $B$.

32\. Let $R$ be the relation $\{(1, 2), (1, 3), (2, 3), (2, 4), (3, 1)\}$, and let $S$ be the relation $\{(2, 1), (3, 1), (3, 2), (4, 2)\}$. Find $S \circ R$.
 $R$   |  $S$   | $S \circ R$
 ------|--------|------------
(1, 2) | (2, 1) | (1, 1)
(1, 3) | (3, 1) | (1, 1)
(1, 3) | (3, 2) | (1, 2)
(2, 3) | (3, 1) | (2, 1)
(2, 3) | (3, 2) | (2, 2)
(2, 4) | (4, 2) | (1, 1)
(3, 1) | (2, 1) | (1, 1)
>Solution
See Table Above.
$S \circ R = \{(1, 1), (1, 2), (2, 1), (2, 2)\}$
