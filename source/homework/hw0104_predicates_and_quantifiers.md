### Section 1.4 Predicates And Quantifiers
pg74: 11, 13, 30, 36, 52

11\. Let $P(x)$ be the statement $"x = x^2."$ If the domain consists of the integers, what are these truth values?
a) $P(0)$  &emsp; b) $P(1)$ &emsp; c) $P(2)$ &emsp; d) $P(-1)$ &emsp; e) $\forall xP(x)$ &emsp; f) $\exists xP(x)$
>Solution
a) $P(0)$ is the statement "$0 = 0^2$", and it's true.
b) $P(1)$ is the statement "$1 = 1^2$", and it's true.
c) $P(2)$ is the statement "$2 = 2^2$", and it's false.
d) $P(-1)$ is the statement "$-1 = (-1)^2$", and it's false.
e) $P(x)$ is not true for every integer, for instance, $P(-1)$ is false. That is, $x=-1$ is a counterexample for  $\forall xP(x)$. Thus $\forall xP(x)$ is false.
f) $P(x)$ is sometimes true, for instance, $P(0)$ is true. Thus $\exists xP(x)$ is true.

13\. Determine the truth value of each of these statements if the domain consists of all integers.
a) $\forall n(n + 1 > n)$ &emsp; b) $\exists n(2n = 3n)$ &emsp; c) $\exists n(n = -n)$ &emsp; d) $\forall n(3n \leqslant 4n)$
>Solution
a) $n + 1 > n$ is true for all integers. Thus $\forall n(n + 1 > n)$ is true.
b) $2n = 3n$ is sometimes true, for instance, $2\times 0 = 3 \times 0$. Thus $\exists n(2n = 3n)$ is true.
c) $n = -n$ is sometimes true, for instance, $0 = -(0)$. Thus $\exists n(n = -n)$ is true.
d) $3n \leqslant 4n$ is not true for every integer, for instance, $3 \times (-1) \leqslant 4 \times (-1)$ is false. That is $x=-1$ is a counterexample for $\forall n(3n \leqslant 4n)$. Thus $\forall n(3n \leqslant 4n)$ is false.

30\. Suppose the domain of the propositional function $P(x, y)$ consists of pairs $x$ and $y$, where $x$ is 1, 2, or 3 and $y$ is 1, 2, or 3. Write out these propositions using disjunctions and conjunctions.
a) $\exists x P (x, 3)$ &emsp; b) $\forall yP(1, y)$ &emsp; c) $\exists y \neg P (2, y)$ &emsp; d) $\forall x \neg P (x, 2)$
>Solution
a) $\exists x P (x, 3) \Bi P(1, 3) \lor P(2, 3) \lor P(3, 3)$
b) $\forall yP(1, y) \Bi P(1, 1) \land P(1, 2) \land P(1, 3)$
c) $\exists y \neg P (2, y) \Bi \neg P(2, 1) \lor \neg P(2, 2) \lor \neg P(2, 3)$
d) $\forall x \neg P (x, 2) \Bi \neg P(1, 2) \land \neg P(2, 2) \land P(3, 2)$

36\. Find a counterexample, if possible, to these universally quantified statements, where the domain for all variables consists of all real numbers.
a) $\forall x(x^2=x)$ &emsp; b) $\forall x(x^2 =2)$ &emsp; c) $\forall x(|x| > 0)$
>Solution
a) $x=2$ is a counterexample. When $x=2$, $x^2=x$ is false.
b) $x=2$ is a counterexample. When $x=2$, $x^2=2$ is false.
c) $x=0$ is a counterexample. When $x=0$, $|x|>0$ is false.

52\. As mentioned in the text, the notation $\exists !xP(x)$ denotes "There exists a unique $x$ such that $P(x)$ is true." If the domain consists of all integers, what are the truth values of these statements?
a) $\exists !x(x > 1)$ &emsp; b) $\exists !x(x^2 = 1)$ &emsp; c) $\exists !x(x + 3 = 2x)$ &emsp; d) $\exists !x(x = x + 1)$
>Solution
a) $\exists !x(x > 1)$ is false. Because there exists more than one $x$ such that $x>1$, for instance, $x=2$, $x=3$.
b) $\exists !x(x^2 = 1)$ is false. Because there exists more than one $x$ such that $x^2 = 1$, for instance, $x=1$, $x=-1$.
c) $\exists !x(x + 3 = 2x)$ is true. $x + 3 = 2x$ is true only if $x=3$.
d) $\exists !x(x = x + 1)$ is false. Because $x=x+1$ is always false for all integers.
