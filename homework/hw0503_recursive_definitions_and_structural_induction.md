### Section 5.3 Recursive Definitions and Structural Induction
pg379: 12, 13, 15, 48, 49, 50

In Exercises 12–19 fn is the nth Fibonacci number.
12\. Prove that $f_1^2 + f_2^2 + \cdots + f_n^2 = f_nf_{n+1}$ when $n$ is a positive integer.
>Solution
Proof:
Let $P(n)$ be the statement $f_1^2 + f_2^2 + \cdots + f_n^2 = f_nf_{n+1}$ for all positive integer $n$.
**Basic step**. $P(1)$ is true, because $f_1^2 = 1^2 = 1 \cdot 1 = f_1f_2$.
**Hypothesis**. Assume $P(n)$ is true for $n=k$
$$
f_1^2 + f_2^2 + \cdots + f_k^2 = f_kf_{k+1}
$$
**Inductive step** We need to prove $P(k+1)$, namely, $f_1^2 + f_2^2 + \cdots + f_{k+1}^2 = f_{k+1}f_{k+2}$, is true.
$$
\begin{aligned}
&f_1^2 + f_2^2 + \cdots + f_{k+1}^2\\
&= f_1^2 + f_2^2 + \cdots + f_k^2 + f_{k+1}^2\\
&= f_kf_{k+1} + f_{k+1}^2 &\text{By Hypothesis}\\
&= f_{k+1}(f_k + f_{k+1}) &\text{Common factor } f_{k+1}\\
&= f_{k+1}f_{k+2} &\text{Definition of Fabonacci Function}
\end{aligned}
$$
By induction, $P(n)$ is true.

13\. Prove that $f_1 + f_3 + \cdots + f_{2n-1} = f_{2n}$ when $n$ is a positive integer.
>Solution
Proof:
Let $P(n)$ be the statement $f_1 + f_3 + \cdots + f_{2n-1} = f_{2n}$ for all positive integer $n$.
**Basic step**. $P(1)$ is true, because $f_1^2 = 1^2 = 1 = f_2$.
**Hypothesis**. Assume $P(n)$ is true for $n=k$
$$
f_1 + f_3 + \cdots + f_{2k-1} = f_{2k}
$$
**Inductive step** We need to prove $P(k+1)$, namely, $f_1 + f_3 + \cdots + f_{2k+1} = f_{2k+2}$, is true.
$$
\begin{aligned}
&f_1 + f_3 + \cdots + f_{2k+1}\\
&= f_1 + f_3 + \cdots + f_{2k-1} + f_{2k+1}\\
&= f_{2k} + f_{2k+1} &\text{By Hypothesis}\\
&= f_{2k+2} &\text{Definition of Fabonacci Function}
\end{aligned}
$$
By induction, $P(n)$ is true.

15\. Show that $f_0f_1 + f_1f_2 + \cdots + f_{2n-1}f_{2n} = f_{2n}^2$ when $n$ is a positive integer.
>Solution
Proof:
Let $P(n)$ be the statement $f_0f_1 + f_1f_2 + \cdots + f_{2n-1}f_{2n} = f_{2n}^2$ for all positive integer $n$.
**Basic step**. $P(1)$ is true, because $f_0f_1 + f_1f_2 = 0 \cdot 1 + 1 \cdot 1 = 1 = f_2^2$.
**Hypothesis**. Assume $P(n)$ is true for $n=k$
$$
f_0f_1 + f_1f_2 + \cdots + f_{2k-1}f_{2k} = f_{2k}^2
$$
**Inductive step** We need to prove $P(k+1)$, namely, $f_0f_1 + f_1f_2 + \cdots + f_{2k+1}f_{2k+2} = f_{2k+2}^2$, is true.
$$
\begin{aligned}
&f_0f_1 + f_1f_2 + \cdots + f_{2k+1}f_{2k+2}\\
&= f_0f_1 + f_1f_2 + \cdots + f_{2k-1}f_{2k} + f_{2k}f_{2k+1} + f_{2k+1}f_{2k+2}\\
&= f_{2k}^2 + f_{2k}f_{2k+1} + f_{2k+1}f_{2k+2} &\text{By Hypothesis}\\
&= f_{2k}(f_{2k} + f_{2k+1}) + f_{2k+1}f_{2k+2} &\text{Common factor }f){2k} \\
&= f_{2k}f_{2k+2} + f_{2k+1}f_{2k+2} &\text{Definition of Fabonacci Function}\\
&= f_{2k+2}(f_{2k} + f_{2k+1}) &\text{Common factor}\\
&= f_{2k+2}^2 &\text{Definition of Fabonacci Function}
\end{aligned}
$$
By induction, $P(n)$ is true.

Consider an inductive definition of a version of Ackermann's function. This function was named after Wilhelm Ackermann, a German mathematician who was a student of the great mathematician David Hilbert. Ackermann's function plays an important role in the theory of recursive functions and in the study of the complexity of certain algorithms involving set unions. (There are several different variants of this function. All are called Ackermann's function and have similar properties even though their values do not always agree.)
$$
\begin{aligned}
&A(m,n) = \begin{cases}
2n &\text{if } m=0\\
0 &\text{if } m\ges 1 \text{ and } n = 0\\
2 &\text{if } m\ges 1 \text{ and } n = 1
\end{cases}\\
&A(m-1, A(m, n-1)), \quad\text{if } m\ges 1 \text{ and } n \ges 2
\end{aligned}
$$

Exercises 48–55 involve this version of Ackermann's function.
48\. Find these values of Ackermann's function.
a. $A(1, 0)$ &emsp; b. $A(0, 1)$ &emsp; c. $A(1, 1)$ &emsp; d. $A(2, 2)$
>Solution
a. $A(1, 0) = 0$ &emsp; b. $A(0, 1) = 2\cdot 1= 2$ &emsp; c. $A(1, 1) = 2$
d.
$$
\begin{aligned}
A(2, 2) &= A(2-1, A(2, 2-1)) \\
&= A(1, A(2, 1)) \\
&= A(1, 2)\\
&= A(0, A(1, 1)) \\
&= A(0, 2) \\
&= 2 \cdot 2 = 4
\end{aligned}
$$


49\. Show that $A(m, 2) = 4$ whenever $m \ges 1$.
>Solution
Proof:
Let $P(m)$ be the statement $A(m, 2) = 4$ for every $m$ greater than or equal to 1.
**Basic step**. $P(1)$ is true, because $A(1, 2) = A(0, A(1, 1)) = A(0, 2) = 4$.
**Hypothesis**. Assume $P(k)$ is true for $m=k$
$$
A(k, 2) = 4
$$
**Inductive step** We need to prove $P(k+1)$, namely, $A(k+1, 2) = 4$, is true.
$$
\begin{aligned}
A(k+1, 2) &= A(k, A(k+1, 1)) \\
&= A(k, 2) &\text{Definition of Ackermann’s function}\\
&= 4 &\text{By hypothesis}
\end{aligned}
$$
By induction, $P(m)$ is true.

50\. Show that $A(1, n) = 2^n$ whenever $n \ges 1$.
>Solution
Proof:
Let $P(n)$ be the statement $A(1, n) = 2^n$ for every $n$ greater than or equal to 1.
**Basic step**. $P(1)$ is true, because $A(1, 1) = 2 = 2^1$.
**Hypothesis**. Assume $P(k)$ is true for $n=k$
$$
A(1, k) = 2^k
$$
**Inductive step** We need to prove $P(k+1)$, namely, $A(1, k+1) = 2^{k+1}$, is true.
$$
\begin{aligned}
A(1, k+1) &= A(0, A(1, k)) \\
&= A(0, 2^k) &\text{By hypothesis}\\
&= 2 \cdot 2^k &\text{Definition of Ackermann’s function}\\
&= 2^{k+1}
\end{aligned}
$$
By induction, $P(n)$ is true.
