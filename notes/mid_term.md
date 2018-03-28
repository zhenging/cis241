Determine the truth value of the statement: $\exists a \forall b (b^2 \ges a)$ if the domain of the variable consists of the positive (non-zero) real numbers.
>Solution
The statement is false. There are three cases:
case #1: $a>1$, when $b=1$, $b^2 \ges a$ is false.
case #2: $a=1$, when $b=0.5$, $b^2 \ges a$ is false.
case #3: $0<a<1$, when $b=a$, $b^2 \ges a$ is false.
No matter what value we choose for $a$ in its domain, there is alwasy some value for $b$, that $b^2 \ges a$ is false.

Prove that: $\sqrt[3]{2}$ is irrational.
>Solution
Todo

Let k be interger. Prove: If $k^3$ is odd, then $k^2 + 1$ is even.
>Solution
To prove the statment, we first need to prove that if $k^3$ is odd, then $k$ is odd.
(1) By contrapositive, the contraposition is: if $k$ is even, then $k^3$ is even.
Let $k=$, where $n$ is an integer. We have
$$
\begin{aligned}
k^3 &=(2n)^3
\\ &=8n^3 = 2 \cdot (4n^3) &\text {Even}
\end{aligned}
$$
Thus the statement that if $k^3$ is odd, then $k$ is odd, is proved.
(2) From (1), we know that $k$ is odd. Let $k=2m+1$,
$$
\begin{aligned}
k^2 + 1 &= (2m+1)^2 + 1\\
&= 2(2m^2+2m+1) &\text{Even}
\end{aligned}
$$
Thus the original statment is proved.

Prove that: $16^n$ is not $O(15^n)$.
>Solution
By contradiction, the contradiction is: $16^n$ is $O(15^n)$.
(1) By definition of $O$, $\exists c,k (16^n \les C\cdot 15^n) \forall n>k$, then we have
$$
\begin{aligned}
16^n \les C\cdot 15^n\\
C \ges (\frac{16}{15})^n
\end{aligned}
$$
(2) Because $\dfrac{16}{15} \ges 1$ and $n$ can be arbitraily large, $\dlim_{n \to \infty}(\frac{16}{15})^n = \infty$.
(3) There is no such constant $C$, which statisfies $C \ges (\frac{16}{15})^n$.
(4) Thus the contradiction is false.
The original statment is **true**.

3a. Let $h$ be a function from a set $X$ to a set $Y$. Let A and B be subsets of set $X$. Prove: $h(A) \cup h(B) \subseteq h(A\cup B)$
>Solution
Let $y \in h(A) \cup h(B)$,
case #1: $y \in h(A)$, by defintion, $\exists (a_1\in A) h(a_1) = y$
$$
\begin{aligned}
y \in h(A) &\To a_1 \in A\\
&\To a_1 \in A \cup B\\
&\To h(a_1) \in h(A \cup B)\\
&\To y \in h(A \cup B)
\end{aligned}
$$
case #2: $y \in h(B)$, by defintion, $\exists (a_2\in B) h(a_2) = y$
$$
\begin{aligned}
y \in h(A) &\To a_2 \in B\\
&\To a_2 \in A \cup B\\
&\To h(a_2) \in h(A \cup B)\\
&\To y \in h(A \cup B)
\end{aligned}
$$
In both cases, we proved if $y \in h(A) \cup h(B)$, then $y \in h(A\cup B)$. Thus. the original statement is proved.

4b. How many _one-to-one_ functions are there from a set of $p$ elements to a set of $s$ elements?
>Solution
Let the set of $p$ elements be $P$, and the set of $s$ elements be $S$
case #1: when $p>s$, there is no _one-to-one_ function.
case #2: when $p \les s$, there are $s$ ways to map $p_1$ to $S$, there are $(s-1)$ ways to map $p_2$ to $S$, so on so forth, there are $(s-p+1)$ ways to map $p_p$ to $S$. By product rule, the total of _one-to-one_ functions is $s(s-1)(s-2) \cdots (s-p+1)$.
