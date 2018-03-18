### Section 9.1 Relations and Their Properties
pg602: 3c-f, 9, 25, 32

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

9\. Show that the relation $R = \emptyset $ on the empty set $S = \emptyset$ is reflexive, symmetric, and transitive.
>Solution
Because the assumption that there are elements in $S\times S = \emptyset$ is false, the conclusion that $R$ is reflexive, symmetric and transitive is always true.


25\. How many different relations are there from a set with $m$ elements to a set with $n$ elements?
>Solution
Let the set with $m$ elements be $A$, and the set with $n$ elements be $B$.
1\. A relation from $A$ to $B$ is a subset of $A \times B$.
2\. By product rule, $A\times B$ has $mn$ elements, so it has $2^{mn}$ subsets.
3\. Thus there are $2^{mn}$ relations from $A$ to $B$.

32\. Let $R$ be the relation $\{(1, 2), (1, 3), (2, 3), (2, 4), (3, 1)\}$, and let $S$ be the relation $\{(2, 1), (3, 1), (3, 2), (4, 2)\}$. Find $S \circ R$.
>Solution
$$
\begin{gathered}
(1, 2) \in R \land (2, 1) \in S \to (1, 1) \in S \circ R\\
(1, 3) \in R \land (3, 1) \in S \to (1, 1) \in S \circ R\\
(1, 3) \in R \land (3, 2) \in S \to (1, 2) \in S \circ R\\
(2, 3) \in R \land (3, 1) \in S \to (2, 1) \in S \circ R\\
(2, 3) \in R \land (3, 2) \in S \to (2, 2) \in S \circ R\\
(2, 4) \in R \land (4, 2) \in S \to (2, 2) \in S \circ R\\
S \circ R = \{(1, 1), (1, 2), (2, 1), (2, 2)\}
\end{gathered}
$$
