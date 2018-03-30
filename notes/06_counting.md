## Chapter 06 Counting

### 6.1 The Basics of Counting
Ex: 1-23, except 17
**HW** pg 417: 1, 6, 10, 12, 17, 28, 32a-f, 34, 37a-b,48, 49, 55, 56

* How to count one-to-one functions (**hw37**)
* Product rule (**and**)
* Sum rule (**or**)

### 6.2 The Pigeonhole Principle
Ex: 1-3, 5-7
**HW** 2, 6, 9

>Theorem 1 - The pigeonhole principle
If **k** is a positive integer and **k+1** or more objects are placed into $k$ boxes, then there is at least one box containing two or more of the objects.

>Theorem 2 - Generalized pigeonhole principle
If $N$ object are placed into $k$ boxes, then there is at least one box containing $\lceil N/k \rceil$ objects.

### 6.3 Permutations and Combinations
p428
Ex: 1-15, except 11

* Permutation (order matters)
> If $n$ is positive integer and $r$ is an integer with $0 \leqslant r \leqslant n$, then there are $P(n, r) = n(n-1) \cdots (n-r+1) = \frac{n!}{(n-r)!}$

* Combination (order does not matter)
> The number is $r$-combinations of a set with $n$ elements, where $n$ is a nonnegative integer and $r$ i an integer with $0 \leqslant r \leqslant n$, equals $C(n, r) = \frac{n!}{(n-r)!r!}$

### 6.4 Binomial Coefficients and Identities
p436
Ex: 1-4

**THE BINOMIAL THEOREM** Let $x$ and $y$ be variables, and let n be a nonnegative integer. Then
$$
\begin{aligned}
(x+y)^n &= \binom{n}{0}x^ny^0 + \binom{n}{1}x^{n-1}y^1 + \cdots + \binom{n}{n}x^0y^n\\
&=\sum^n_{k=0}x^{n-k}y^k
\end{aligned}
$$
