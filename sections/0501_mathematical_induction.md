### 5.1 Mathematical Induction
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

#### Homework
p350: 6, 14, 15, 20, 21, 31, 32, 34, 36, 43

6\. Prove that $1 \cdot 1! + 2 \cdot 2!+ \cdots + n \cdot n! = (n + 1)! - 1$ whenever $n$ is a positive integer.
>Solution
Proof:
Let $P(n)$ be the statement $1 \cdot 1! + 2 \cdot 2!+ \cdots + n \cdot n! = (n + 1)! - 1$ for all every integer $n$.
**Basic step**. $P(1)$ is true, because $1\cdot 1 = (1+1) \cdot 1 -1 = 1$
**Hypothesis**. Assume $P(n)$ is true for $n=k$
$$
1 \cdot 1! + 2 \cdot 2!+ \cdots + k \cdot k! = (k + 1)! - 1
$$
**Inductive step** We need to prove $P(k+1)$, namely, $1 \cdot 1! + 2 \cdot 2!+ \cdots + k \cdot k! + (k+1)\cdot (k+1) = (k + 2)! - 1$.
$$
\begin{aligned}
&1 \cdot 1! + 2 \cdot 2!+ \cdots + k \cdot k! + (k+1)\cdot (k+1)!\\
&= (k+1)! - 1 + (k+1)\cdot (k+1)! &\text{By Hypothesis}\\
&= (k+2)(k+1)! - 1\\
&= (k+2)! - 1
\end{aligned}
$$
By induction, $P(n)$ is true.

14\. Prove that for every positive integer $n$, $\sum_{k=1}^n{k2^k} = (n-1)2^{n+1} + 2$.
>Solution
Proof:
Let $P(n)$ be the statement $\sum_{k=1}^n{k2^k} = (n-1)2^{n+1} + 2$, for every positive integer $n$.
**Basic step**. $P(1)$ is true, because $\sum_{k=1}^1{k2^k} = 1 \cdot 2^1 = (1-1)\cdot 2^{1+1} + 2 = 2$.
**Hypothesis**. Assume $P(n)$ is true for $n=m$
$$
\sum_{k=1}^m{k2^k} = (m-1)2^{m+1} + 2
$$
**Inductive step** We need to prove $P(m+1)$, namely $\sum_{k=1}^{m+1}{k2^k} = (m)2^{m+2} + 2$, is true.
$$
\begin{aligned}
\sum_{k=1}^{m+1}{k2^k} &= \underline{\sum_{k=1}^{m}{k2^k}} + (m+1)2^{m+1} \\
&= \underline{(m-1)2^{m+1} + 2} + (m+1)2^{m+1} &\text{By Hypothesis}\\
&= (m-1 + m+1)2^{m+1} + 2\\
&= m \cdot 2 \cdot 2^{m+1} + 2\\
&= m2^{m+2} + 2
\end{aligned}
$$
By induction, $P(n)$ is true.

15\. Prove that for every positive integer $n$, $1\cdot 2 + 2\cdot 3 + \cdots + n(n + 1) = n(n + 1)(n + 2)/3$.
>Solution
Proof:
Let $P(n)$ be the statement $1\cdot 2 + 2\cdot 3 + \cdots + n(n + 1) = n(n + 1)(n + 2)/3$, for every positive integer $n$.
**Basic step**. $P(1)$ is true, because $1\cdot 2 = \dfrac{1\cdot (1+1)(1+2)}{3} = 2$.
**Hypothesis**. Assume $P(n)$ is true for $n=k$
$$
1\cdot 2 + 2\cdot 3 + \cdots + k(k + 1) = \frac{k(k + 1)(k + 2)}{3}
$$
**Inductive step** We need to prove $P(k+1)$, namely $1\cdot 2 + 2\cdot 3 + \cdots + k(k+1)+(k+1)(k+2)= \dfrac{(k+1)(k+2)(k+3)}{3}$, is true.
$$
\begin{aligned}
&1\cdot 2 + 2\cdot 3 + \cdots + k(k+1)+(k+1)(k+2)\\
&= \frac{k(k + 1)(k + 2)}{3} + (k+1)(k+2) &\text{By hypothesis}\\
&= \frac{k(k + 1)(k + 2)}{3} + \frac{3(k + 1)(k + 2)}{3}\\
&= \frac{(k + 1)(k + 2)(k+3)}{3}
\end{aligned}
$$
By induction, $P(n)$ is true.

20\. Prove that $3^n< n!$ if $n$ is an integer greater than 6.
>Solution
Let $P(n)$ be the statement $3^n< n!$ for integer $n$ greater than 6.
**Basic step** $P(7)$ is true, because $3^7=2187 < 7!=5040$.
**Hypothesis**. Assume $P(n)$ is true for $n=k$,
$$
3^k< k!
$$
**Inductive step**. We need to prove $P(k+1)$, namely $3^{k+1}< (k+1)!$, is true.
$$
\begin{aligned}
3^{k+1} = 3 \cdot 3^k < 3 \cdot k! \quad \text{By hypothesis}\\
\because k+1> n+1 > 6+1 =7 > 3\\
\therefore 3^{k+1} = 3 \cdot 3^k < (k+1) \cdot k! = (k+1)!
\end{aligned}
$$
By induction, $P(n)$ is true.

21\. Prove that $2^n > n^2$ if $n$ is an integer greater than 4.
>Solution
Let $P(n)$ be the statement $2^n > n^2$ for integer $n$ greater than 4.
**Basic step** $P(5)$ is true, because $2^5=32 > 5^2=25$.
**Hypothesis**. Assume $P(n)$ is true for $n=k$,
$$
2^n> n^2
$$
**Inductive step**. We need to prove $P(k+1)$, namely $2^{k+1}> (k+1)^2$, is true.
$$
\begin{aligned}
2^{k+1} =2 \cdot 2^k > 2k^2 \quad \text{By hypothesis}\\
2k^2 - (k+1)^2 = 2k^2-k^2-2k-1 = (k-1)^2 - 2\\
\because k>4\\
\therefore (k-1)^2 -2 > 0\\
\therefore 2k^2 - (k+1)^2 > 0\\
\therefore 2k^2 > (k+1)^2\\
\therefore 2^{k+1} > (k+1)^2
\end{aligned}
$$
By induction, $P(n)$ is true.

31\. Prove that $2$ divides $n^2 + n$ whenever $n$ is a positive integer.
>Solution
Let $P(n)$ be the statement $2 \lvert n^2 + n$ for positive integer $n$.
**Basic step** $P(1)$ is true, because $\dfrac{1^2+1}{2} = 1$.
**Hypothesis**. Assume $P(n)$ is true for $n=k$,
$$
2 \lvert k^2 + k
$$
**Inductive step**. We need to prove $P(k+1)$, namely $2 \lvert (k+1)^2 + k+1$, is true.
$$
\begin{aligned}
(k+1)^2 + k+1 &= k^2+2k+1+k+1\\
&= k^2+k + 2(k+1)\\
&\because 2 \lvert k^2+k \text{ and } 2 \lvert 2(k+1)\\
&\therefore 2 \lvert k^2+k + 2(k+1) \text { or } 2 \lvert (k+1)^2 + k+1
\end{aligned}
$$
By induction, $P(n)$ is true.

32\. Prove that $3$ divides $n^3 + 2n$ whenever $n$ is a positive integer.
>Solution
Let $P(n)$ be the statement $3 \lvert n^3 + 2n$ for positive integer $n$.
**Basic step** $P(1)$ is true, because $\dfrac{1^3+2 \cdot 1}{3} = 1$.
**Hypothesis**. Assume $P(n)$ is true for $n=k$,
$$
3 \lvert k^3 + 2k
$$
**Inductive step**. We need to prove $P(k+1)$, namely $3 \lvert (k+1)^3 + 2(k+1)$, is true.
$$
\begin{aligned}
(k+1)^3 + 2(k+1) &= k^3+3k^2+3k+1 + 2k+2\\
&= (k^3+2k) + (3k^2+3k+3)\\
&= (k^3+2k) + 3(k^2+k+1)\\
&\because 3 \lvert (k^3+2k) \text{ and } 3 \lvert 3(k^2+k+1)\\
&\therefore 3 \lvert (k^3+2k) + 3(k^2+k+1) \text{ or } 3\lvert (k+1)^3 + 2(k+1)
\end{aligned}
$$
By induction, $P(n)$ is true.

34\.Prove that $6$ divides $n^3 - n$ whenever $n$ is a nonnegative
integer.
>Solution
Let $P(n)$ be the statement $6 \lvert n^3 - n$ for positive integer $n$.
**Basic step** $P(1)$ is true, because $\dfrac{1^3-1}{6} = 0$.
**Hypothesis**. Assume $P(n)$ is true for $n=k$,
$$
6 \lvert k^3 - k
$$
**Inductive step**. We need to prove $P(k+1)$, namely $6 \lvert (k+1)^3 -(k+1)$, is true.
$$
\begin{aligned}
(k+1)^3 -(k+1)&= k^3+ 3k^2+3k+1-k-1\\
&= (k^3 -k) + 3k(k+1)
\end{aligned}
$$
As $6|(k^3 -k)$, we need to to prove $6|3k(k+1)$.
Because one in $k$ and $k+1$ is even, $k(k+1)$ is even. Thus $6|3k(k+1)$.
That is $6\lvert (k^3 -k) + 3k(k+1)$
By induction, $P(n)$ is true.

36\.Prove that 21 divides $4^{n+1} + 5^{2n-1}$ whenever $n$ is a positive integer.
>Solution
Let $P(n)$ be the statement $21 \lvert 4^{n+1} + 5^{2n-1}$ for positive integer $n$.
**Basic step** $P(1)$ is true, because $\dfrac{4^{1+1} + 5^{2-1}}{21} = \dfrac{21}{21} = 1$.
**Hypothesis**. Assume $P(n)$ is true for $n=k$,
$$
21 \lvert 4^{k+1} + 5^{2k-1}
$$
**Inductive step**. We need to prove $P(k+1)$, namely $21 \lvert 4^{(k+1)+1} + 5^{2(k+1)-1}$, is true.
$$
\begin{aligned}
4^{(k+1)+1} + 5^{2(k+1)-1} &= 4\cdot 4^{k+1} + 25 \cdot 5^{2k-1}\\
&= 25\cdot 4^{k+1} + 25 \cdot 5^{2k-1} - 21\cdot 4^{k+1}\\
&= 25\cdot(4^{k+1} + 5^{2k-1}) - 21\cdot 4^{k+1}\\
&\because 21 \lvert (4^{k+1} + 5^{2k-1}) \quad \text{Hypothesis}\\
&\therefore 21 \lvert 25\cdot(4^{k+1} + 5^{2k-1})\\
&\because 21 \lvert 21\cdot 4^{k+1}\\
&\therefore 21 \lvert 25\cdot(4^{k+1} + 5^{2k-1}) - 21\cdot 4^{k+1} \text{ or } 21 \lvert 4^{(k+1)+1} + 5^{2(k+1)-1}
\end{aligned}
$$
By induction, $P(n)$ is true.

43\. Prove that if $A1, A2,...,An$ are subsets of a universal set $U$, then $\overline{\bigcup_{k=1}^n A_k} = \bigcap_{k=1}^n \overline{A_k}$.
>Solution
Let $P(n)$ be the statement $\overline{\bigcup_{k=1}^n A_k} = \bigcap_{k=1}^n \overline{A_k}$.
**Basic step**. $P(1)$ is true, because $\overline{\bigcup_{k=1}^1 A_k} = \overline{A_1} = \bigcap_{k=1}^1 \overline A_1$.
**Hypothesis**. Assume $P(n)$ is true for $n=m$,
$$
\overline{\bigcup_{k=1}^m A_k} = \bigcap_{k=1}^m \overline{A_k}
$$
**Inductive step**. We need to prove $P(k+1)$, namely $\overline{\bigcup_{k=1}^{m+1} A_k} = \bigcap_{k=1}^{m+1} \overline{A_k}$, is true.
$$
\begin{aligned}
\overline{\bigcup_{k=1}^{m+1} A_k} &= \overline{\bigcup_{k=1}^{m} A_k \cup A_{m+1}} &\text{Defition of union of sets}\\
&= \overline{\bigcup_{k=1}^{m} A_k} \cap \overline{A_{m+1}} &\text{De Morgan's Law}\\
&= \bigcap_{k=1}^{m} \overline{A_k} \cap \overline{A_{m+1}} &\text{By Hypothesis}\\
&= \bigcap_{k=1}^{m+1} \overline{A_k} &\text{Defition of intersection of sets}\\
\end{aligned}
$$
By induction, $P(n)$ is true.
