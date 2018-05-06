### Section 1.5 Nested Quantifiers
pg85: 26, 27 e g h, 31b d, **46**

26\. Let $Q(x, y)$ be the statement “$x + y = x - y$” If the domain for both variables consists of all integers, what are the truth values?
a) $Q(1, 1)$ &emsp; b) $Q(2, 0)$ &emsp; c) $\forall y Q(1, y)$
d) $\exists x Q(x, 2)$ &emsp; e) $\exists x \exists yQ(x, y)$ &emsp; f) $\forall x\exists yQ(x, y)$
g) $\exists y \forall x Q(x, y)$ &emsp; h) $\forall y\exists xQ(x, y)$
>Solution
a) $Q(1, 1) \Bi 1+1=1-1$. **$Q(1, 1)$ is false**.
b) $Q(2, 0) \Bi 2+0=2-0$. **$Q(2, 0)$ is true**.
c) $\forall y Q(1, y)$ denotes the proposition "For every integer y, $1+y=1-y$ holds". When $y=1$, $1+y=1-y$ is false, therefore **$\forall y Q(1, y)$ is false**.
d) $\exists x Q(x, 2)$ denotes the proposition "There is an integer x, such that $x+2=x-2$". Such $x$ can not be found, **$\exists x Q(x, 2)$ is false**.
e) $\exists x \exists yQ(x, y)$ denotes the proposition "There is a pair $x, y$ such that $Q(x, y)$".  The pair $x=1, y=0$ satisfies $Q(x, y)$,  **$\exists x \exists yQ(x, y)$ is true.**
f) $\forall x\exists yQ(x, y)$ denotes the proposition "For every integer $x$ there is an integer $y$ such that $Q(x, y)$". When $y=0$, $Q(x, y)$ is true for every integer $x$, **$\forall x\exists yQ(x, y)$ is true**.
g) $\exists y \forall x Q(x, y)$ denots the proposition "There is an integer $y$, such that for every integer $x$, $x+y=x-y$ holds". When $y=0$,  $x+y=x-y$ holds for every $x$, **$\exists y \forall x Q(x, y)$ is true.**
h) $\forall y\exists xQ(x, y)$ denotes the proposition "For every integer $y$ there is an integer $x$ such that $Q(x, y)$". When $y=1$, we could not find any $x$ to satisfy  $Q(x, y)$, **$\forall y\exists xQ(x, y)$ is false.**

27\. Determine the truth value of each of these statements if the domain for all variables consists of all integers.
e) $\exists n\exists m(n^2 + m^2 = 5)$
g) $\exists n\exists m(n + m = 4 \land n - m = 1)$
h) $\exists n\exists m(n + m = 4 \land n - m = 2)$
>Solution
e) The quantification $\exists n\exists m(n^2 + m^2 = 5)$ denotes the proposition "There is a pair $m, n$ such that $n^2 + m^2 = 5$". The pair $m=1, n=2$ satisfies $n^2 + m^2 = 5$. Hence the statement is true.
g) The quantification $\exists n\exists m(n + m = 4 \land n - m = 1)$ denotes the proposition "There is a pair $m, n$ such that $n + m = 4 \land n - m = 1$". We could not find any integer pair $m,n$ to satisfy $n + m = 4 \land n - m = 1$, so the statement is false.
h) The quantification $\exists n\exists m(n + m = 4 \land n - m = 2)$ denotes the proposition "There is a pair $m, n$ such that $n + m = 4 \land n - m = 2$". The pair $m=1,n=3$ satisfies $n + m = 4 \land n - m = 2$. Hence, the statement is true.

31\. Express the negations of each of these statements so that all negation symbols immediately precede predicates.
b) $\forall  x\exists yP (x, y) \lor \forall  x\exists yQ(x, y)$
>Solution
$$
\begin{aligned}
\neg (\forall  x\exists yP (x, y) \lor \forall  x\exists yQ(x, y)) &\equiv \neg \forall  x\exists yP (x, y) \land \neg \forall  x\exists yQ(x, y) \\
&\equiv \exists x \neg \exists yP (x, y) \land  \exists x \neg \exists yQ(x, y) \\
&\equiv \exists x \forall y \neg P (x, y) \land  \exists x \forall y \neg Q(x, y) \\
\end{aligned}
$$

d) $\forall  x\exists y(P (x, y) \to Q(x, y))$
>Solution
$$
\begin{aligned}
\neg \forall  x\exists y(P (x, y) \to Q(x, y)) &\equiv \exists x  \neg \exists y(P (x, y) \to Q(x, y)) \\
&\equiv \exists x  \forall y  \neg(P (x, y) \to Q(x, y)) \\
&\equiv \exists x  \forall y  (P (x, y)  \land \neg Q(x, y))
\end{aligned}
$$

46\. Determine the truth value of the statement $\exists x\forall  y(x \leqslant y^2)$ if the domain for the variables consists of
a) the positive real numbers.
b) the integers.
c) the nonzero real numbers.
>Solution
The quantification $\exists x\forall  y(x \leqslant y^2)$ denotes the proposition "There is a $x$ such that for every $y$, $x \leqslant y^2$".
a) The statement is false when $x,y$ are positive numbers. Because $y^2 \geqslant 0$, we could not find any positive number $x$ that $x \leqslant y^2$.
b) The statement is true when $x,y$ are integers. When $x=0$, the $x \leqslant y^2$ is true for every $y$.
c) The statement is true when $x,y$ are nonzero real numbers. When $x=-1$, the $x \leqslant y^2$ is true for every $y$.
