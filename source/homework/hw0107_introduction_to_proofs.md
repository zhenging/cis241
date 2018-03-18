### Section 1.7 Introduction to Proofs
pg112: 13, 26, 27, 31, 32, 42

13\. Prove that if $x$ is irrational, then $1/x$ is irrational.
>Solution
Proof By Contraposition
If $1/x$ is rational, then $x$ is rational.
Let $\dfrac{1}{x} = \dfrac{a}{b}$, where $a \ne 0$, $b \ne 0$ and $a,b$ have no common factors. It follows that
$$
\frac{1}{x} = \frac{a}{b} \To x = \frac{b}{a}
$$
As $a \ne 0$, $b \ne 0$ and $a,b$ have no common factors, $x$ is rational.
Therefore, the original statement is true.

26\. Prove that if $n$ is a positive integer, then $n$ is even if and only if $7n + 4$ is even.
>Solution
Let $p$ be the statement "$n$ is even", and $q$ be the statement "$7n + 4$ is even." To prove the original statement, we need to show $p \to q$ and $q \to p$.
1\. $p \to q$. Let $n=2k$, where $k$ is a positive integer. It follows that
$$
7n + 4 = 7 \times 2k + 4 = 2(7k+2)
$$
Therefore, $7n+4$ is even. $p \to q$ is proved.
2\. $q \to p$. By contraposition, the contrapositive is "If $n$ is odd, then $7n + 4$ is odd". Let $n=2m+1$, where $m$ is a non-negative integer.
$$
7n + 4 = 7 \times (2m+1) + 4 = 2(7m+5) + 1
$$
Therefore, $7n+4$ is odd. The contrapositive is proved, and $q \to p$ is true.
Becuase both $p \to q$ and $q \to p$ are true, the original statement is true.

27\. Prove that if $n$ is a positive integer, then $n$ is odd if and only if $5n + 6$ is odd.
>Solution
Let $p$ be the statement "$n$ is odd", and $q$ be the statement "$5n + 6$ is odd." To prove the original statement, we need to show $p \to q$ and $q \to p$.
1\. $p \to q$. Let $n=2k+1$, where $k$ is a non-negative integer. It follows that
$$
5n + 6 = 5 \times (2k+1) + 6 = 2(5k+5) + 1
$$
Therefore, $5n+6$ is odd. $p \to q$ is proved.
2\. $q \to p$. By contraposition, If $n$ is even, then $5n + 6$ is even. Let $n=2m$, where $m$ is a non-negative integer.
$$
5n + 6 = 5 \times 2m + 6 = 2(5m+3)
$$
Therefore, $5n+6$ is even. $q \to p$ is proved.
Becuase both $p \to q$ and $q \to p$ are true, the original statement is true.

31\. Show that these statements about the integer $x$ are equivalent: (i) $3x + 2$ is even, (ii) $x + 5$ is odd, (iii) $x^2$ is even.
>Solution
Let $p$ be the statement (i) $3x + 2$ is even, $q$ be the statement (ii) $x + 5$ is odd, and $r$ be the statement (iii) $x^2$ is even. In order to show that these statement are equivalent about the integer $x$, we need to show  (1)$p \to q$, (2)$q \to r$, and (3) $r \to p$.
(1) $p \to q$. If (i) $3x + 2$ is even, then (ii) $x + 5$ is odd.
By contraposition, the contrapositive is "if $x + 5$ is even, then $3x + 2$ is odd". Let $x + 5 = 2k$, where $k$ is an integer.
$$
\begin{aligned}
x + 5 &= 2k  \\
x &= 2k-5 \\
3x+2 &= 3(2k-5) + 2 = 2(3k-7) + 1
\end{aligned}
$$
Therefore, $3x+2$ is odd. $p \to q$ is proved.
(2) $q \to r$. If (ii) $x + 5$ is odd, then (iii) $x^2$ is even.
Let $x + 5 = 2k + 1$, where $k$ is an integer.
$$
\begin{aligned}
x+5 &= 2k+1\\
x &= 2k-4\\
x^2 &= (2k-4)^2 = 2(2k^2 - 8k + 8)
\end{aligned}
$$
Therefore, $x^2$ is even. $q \to r$ is proved.
(3) $r \to p$.  If (iii) $x^2$ is even, then (i) $3x + 2$ is even.
We first need to proof that if $x^2$ is even, then $x$ is even. By contraposition, the contrapositive is "if $x$ is odd, then $x^2$ is odd". Let $x = 2k + 1$, where $k$ is an integer.
$$
x^2 = (2k+1)^2 = 2(2k^2 + 2k) + 1
$$
Therefore $x^2$ is odd. We proved that if $x^2$ is even, then $x$ is even.
Let $x = 2m$, where $m$ is an integer.
$$
3x + 2 = 3 \times 2m + 2 = 2(3m+1)
$$
Therefore $3x + 2$ is even. $r \to p$ is proved.
Because (1)$p \to q$, (2)$q \to r$, and (3) $r \to p$ are all true, the statements $p$, $q$, and $r$ are equivalent.

32\. Show that these statements about the real number $x$ are equivalent: (i) $x$ is rational, (ii) $x/2$ is rational, (iii) $3x - 1$ is rational.
>Solution
Let $p$ be the statement (i) $x$ is rational, $q$ be the statement (ii) $x/2$ is rational, and $r$ be the statement (iii) $3x - 1$ is rational. In order to show that these statement are equivalent about the real number $x$, we need to show  (1)$p \to q$, (2)$q \to r$, and (3) $r \to p$.
(1) $p \to q$. If (i) $x$ is rational, then (ii) $x/2$ is rational.
Let $x =\dfrac{a}{b}$, where $a$ and $b$ have no common factors and $b \ne 0$.
$$
\frac{x}{2} = \frac{a}{2b}
$$
Therefore $\dfrac{x}{2}$ is rational. $p \to q$ is proved.
(2) $q \to r$.  If (ii) $x/2$ is rational, then (iii) $3x - 1$ is rational.
Let $\dfrac{x}{2} = \dfrac{m}{n}$, where $m$ and $n$ have no common factors and $n \ne 0$.
$$
x = \frac{2m}{n} \To 3x - 1 = \frac{6m-n}{n}
$$
Therefore $3x-1$ is rational. $q \to r$ is proved.
(3) $r \to p$. If (iii) $3x - 1$ is rational, then (i) $x$ is rational.
Let $3x-1 = \dfrac{c}{d}$, where $c$ and $d$ have no common factors and $d \ne 0$.
$$
x = \frac{c+d}{3d}
$$
Therefore $x$ is rational. $r \to p$ is proved.
Because (1)$p \to q$, (2)$q \to r$, and (3) $r \to p$ are all true, the statements $p$, $q$, and $r$ are equivalent.

42\. Prove that these four statements about the integer $n$ are equivalent: (i) $n^2$ is odd, (ii) $1 - n$ is even, (iii) $n^3$ is odd, (iv) $n^2 + 1$ is even.
>Solution
Let $p$ be the statement (i) $n^2$ is odd, $q$ be the statement (ii) $1 - n$ is even, $r$ be the statement (iii) $n^3$ is odd, and $s$ be the statement (iv) $n^2 + 1$. In order to show that these statement are equivalent about the real number $x$, we need to show  (1)$p \to q$, (2)$q \to r$, (3) $r \to s$, and (4) $s \to p$.
(1) $p \to q$. If (i) $n^2$ is odd, then (ii) $1 - n$ is even.
We first need to prove that if $n^2$ is odd, then $n$ is odd. By contraposition, the contrapositive is "if $n$ is even, then $n^2$ is even." Let $n = 2k$, where $k$ is an integer.
$$
n^2 = (2k)^2 = 2(2k^2)
$$
Therefore, $n^2$ is even. The contrapositive is proved, and the original statement "if $n^2$ is odd, then $n$ is odd" is true. Let $n = 2a + 1$, where $a$ is an integer.
$$
1-n = 1-2a-1 = 2(-a)
$$
Therefore $1-n$ is even. $p \to q$ is proved.
(2) $q \to r$.  If (ii) $1 - n$ is even, then (iii) $n^3$ is odd.
Let $1-n = 2b$, where $b$ is an integer.
$$
\begin{aligned}
1-n &= 2b \To n = 1-2b\\
n^3 &= (1-2b)^3 \\
&= 1-6b+12b^2-8b^3 \\
&= 2(-4b^3+6b^2-3b) +1
\end{aligned}
$$
Therefore $n^3$ is odd. $q \to r$ is proved.
(3) $r \to s$.  If (iii) $n^3$ is odd, then (iv) $n^2 + 1$ is even.
We first need to prove that if $n^3$ is odd, then $n$ is odd.
By contraposition, the contrapositive is "if $n$ is even, then $n^3$ is even". Let $n = 2c$, where $c$ is an integer.
$$
n^3 = (2c)^3 = 2(4c^3)
$$
Therefore $n^3$ is even. The statement "if $n^3$ is odd, then $n$ is odd" is true.
Let $n = 2d+1$, where $d$ is an integer.
$$
n^2 + 1 = (2d+1)^2 +1 = 2(2d^2+2d+1)
$$
Therefore $n^2 + 1$ is even. $r \to s$ is proved.
(4) $s \to p$. If (iv) $n^2 + 1$ is even, then (i) $n^2$ is odd.
We first need to prove that if $n^2 + 1$ is even, $n$ is odd. By contraposition, the contrapositive is "if $n$ is even, then $n^2 + 1$ is odd." Let $n = 2h$, where $h$ is an integer.
$$
n^2 + 1 = (2h)^2 + 1 = 2(2h^2) + 1
$$
Therefore $n^2 + 1$ is odd. The statement "if $n^2 + 1$ is even, $n$ is odd" is true.
Let $n = 2f+1$, where $f$ is an integer.
$$
n^2 = (2f+1)^2 = 2(2f^2+2f) + 1
$$
Therefore $n^2$ is odd. $s \to p$ is proved.
Because (1)$p \to q$, (2)$q \to r$, (3) $r \to s$, and (4) $s \to p$ are all true, the statements $p$, $q$, $r$, and $s$ are equivalent.
