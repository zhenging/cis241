### Chapter 05 Induction and Recursion

#### 5.1 Mathematical Induction
p334
Ex: 1, 2, 3, 5, 6, 8, 9, 10, 11

To prove a statement $P(n)$ is true for every $n \mid n > n_{threshold}$ (positive integer)
1\. **Basic step** Show $P(n_{threshold})$ is true.
2\. **Hypothesis** Assume the statement for a value of $n=k, P(k)$ is true .
3\. **Induction step** Prove for $n=k+1, P(k+1)$ is true.

EXAMPLE 1
Show that if $n$ is a positive integer, then $1 + 2 + \cdots + n = \frac{n(n+1)}{2}$

EXAMPLE 2
Conjecture a formula for the sum of the first n positive odd integers. Then prove your conjecture using mathematical induction.

EXAMPLE 3
Use mathematical induction to show that $1 + 2 + 2^2 + \cdots + 2^n = 2^{n+1} - 1$

EXAMPLE 5
Use mathematical induction to prove the inequality $n <2^n$ for all positive integers.

EXAMPLE 6
Use mathematical induction to prove that $2^n < n!$ for every integer $n$ with $n \ges 4$. (Note that this inequality is false for $n = 1, 2$, and $3$.)

EXAMPLE 8
Use mathematical induction to prove that $n^3 - n$ is divisible by $3$ whenever $n$ is a positive integer. (Note that this is the statement with $p = 3$ of Fermat’s little theorem, which is Theorem 3 of Section 4.4.)

EXAMPLE 9
Use mathematical induction to prove that $7^{n+2} + 8^{2n+1}$ is divisible by $57$ for every nonnegative integer $n$.

EXAMPLE 10
**The Number of Subsets of a Finite Set** Use mathematical induction to show that if $S$ is a finite set with $n$ elements, where $n$ is a nonnegative integer, then $S$ has $2^n$ subsets. (We will prove this result directly in several ways in Chapter 6.)

EXAMPLE 11
Use mathematical induction to prove the following generalization of one of De Morgan's laws:
$$
\begin{aligned}
\overline{\bigcap_{j=1}^n A_j} = \bigcup_{j=1}^n \overline{A_j}
\end{aligned}
$$
whenever $A_1, A_2, \cdots, A_n$ are subsets of a universal set $U$ and $n\ges 2$

#### 5.3 Recursive Definitions and Structural Induction
p365
Ex: 1, 2, 3, 5

EXAMPLE 1
Suppose that $f$ is defined recursively by
$$
\begin{aligned}
f(0)&=3\\
f(n+1) &= 2f(n) + 3
\end{aligned}
$$
Find $f(1), f(2), f(3)$ and $f(4)$.

EXAMPLE 2
Give a recursive definition of $a^n$, where $a$ is a nonzero real number and $n$ is a nonnegative integer.
**Solution**: The recursive definition contains two parts. First $a_0$ is specified, namely, $a^0 = 1$. Then the rule for finding a n+1 from $a^n$, namely, $a^{n+1} = a \cdot a^n$, for $n = 0, 1, 2, 3, \cdots$, is given. These
two equations uniquely define $a^n$ for all nonnegative integers $n$.

EXAMPLE 3
Give a recursive definition of $\sum\limits_{k=0}^n a_k$.
**Solution**: The first part of the recursive definition is $\sum\limits_{k=0}^0 = a_0$.
The second part is $\sum\limits_{k=0}^{n+1} a_k = \left(\sum\limits_{k=0}^n a_k \right)+ a_{n+1}$

EXAMPLE 5
Consider the subset $S$ of the set of integers recursively defined by
Basic Step: $3 \in S$.
Recursive Step: If $x \in S$ and $y \in S$, then $x+y \in S$.
The new elements found to be in S are $3$ by the basis step, $3 + 3 = 6$ at the first application of the recursive step, $3 + 6 = 6 + 3 = 9$ and $6 + 6 = 12$ at the second application of the recursive step, and so on. We will show in Example 10 that S is the set of all positive multiples of $3$.
