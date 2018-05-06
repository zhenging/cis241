### Section 1.8 Proof Methods and Strategy
pg129: 14, 19, 29, 30, 36

14\. Prove or disprove that if $a$ and $b$ are rational numbers, then $a^b$ is also rational.
>Solution
Disprove. When $a=2, b=\dfrac{1}{2}$, it follows that $a^b = \sqrt 2$. $a$ and $b$ are rational numbers, but $\sqrt 2$ is a irrational number.

19\. Show that if $n$ is an odd integer, then there is a unique integer $k$ such that $n$ is the sum of $k-2$ and $k + 3$.
>Solution
Let $n = 2a+1$, where $a$ is an integer. $n=2a+1 = (a-2) + (a+3)$. Therefore, there is a unique $k$, where $k=a$, such that $n=(k-2) + (k+3)$.

29\. Prove that there is no positive integer $n$ such that $n^2 + n^3 = 100$.
>Solution
By contradiction. The contradiction is "there is an positive integer $n$ such that $n^2 + n^3 = 100$".
$$
\begin{gathered}
n > 0 \To n^3 > 0\\
n^2 + n^3 = 100 \To n^3 =100 -n^2\\
0< n^3 < 100
\end{gathered}
$$
The possible values for $n$ are $1, 2, 3, 4$. None of these values satisfies $n^2 + n^3 = 100$.
Therefore the contradiction is false, and the original statement is true.

30\. Prove that there are no solutions in integers $x$ and $y$ to the equation $2x^2 + 5y^2 = 14$.
>Solution
1\. $2x^2 + 5y^2 = 14 \To  x^2 = 7-\dfrac{5y^2}{2} \To 0 \leqslant x^2 \leqslant 7$
2\. The possible integer values for $x$ are $\pm 2, \pm 1, 0$. Solve for $y$, $y = \pm \sqrt{\frac{6}{5}}, \pm \sqrt{\frac{12}{5}}, \pm \sqrt{\frac{14}{5}}$
3\. None of the possible values of $y$ is an integer.
Therefore, the original statement is true.

36\. Prove that between every rational number and every irrational number there is an irrational number.
>Solution
1\. Consider $x, y, z$, where $x$ is rational, $y$ is irrational, and $z = \dfrac{x+y}{2}$, it follows that $z = \dfrac{x+y}{2} \To y= 2z-x$
2\. Assume $z$ is rational, because $x$ is rational too, $2z-x$ is rational.
3\. $y$ is irrational and $y = 2z-x$, the assumption that $z$ is rational is false. $z$ is irrational.
Therefore, the original statement is true.
