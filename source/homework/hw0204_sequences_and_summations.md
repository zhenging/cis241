### Section 2.4 Sequences and Summations
pg189: 16cef, 19, 22

16\. Find the solution to each of these recurrence relations with the given initial conditions. Use an iterative approach such as that used in Example 10.
c. $a_n = a_{n-1} - n, a_0 = 4$
>Solution
$$
\begin{aligned}
a_n &= [a_{n-2}-(n-1)] - n\\
&= a_{n-2}-2n+1\\
&= [a_{n-3}-(n-2)]-2n+1\\
&= a_{n-3}-3n + 1+ 2\\
&= \cdots\\
&= a_0- n\cdot n + 1 + 2 + \cdots + n-1\\
&= a_0-n^2 + \frac{(1+n-1)(n-1)}{2}\\
&= 4-\frac{n^2+n}{2}
\end{aligned}
$$

e. $a_n = (n+1)a_{n-1}, a_0 = 2$
>Solution
$$
\begin{aligned}
a_n &= (n+1)n\cdot a_{n-2}\\
&= (n+1)n(n-1) \cdot a_{n-3}\\
&= \cdots\\
&= (n+1)n(n-1)\cdots 2 \times a_0\\
&= 2(n+1)!
\end{aligned}
$$

f. $a_n = 2n(n+1)a_{n-1}, a_0 = 3$
>Solution
$$
\begin{aligned}
a_n &= 2n(n+1) \cdot 2(n-1)n \cdot a_{n-2}\\
&= 2^2 \cdot (n+1)n \cdot n(n-1) \cdot a_{n-2}\\
&= 2^2 \cdot (n+1)n \cdot n(n-1) \cdot 2(n-2)(n-1) \cdot a_{n-3}\\
&= 2^3 \cdot (n+1)n(n-1) \cdot n(n-1)(n-2) \cdot a_{n-3}\\
&= \cdots\\
&= 2^n \cdot [(n+1)n(n-1)\cdots 2] \cdot [n(n-1)(n-2)\cdots 1] \cdots a_0\\
&= 2^n \cdot (n+1)! \cdot n! \cdot 3
\end{aligned}
$$

19\. Suppose that the number of bacteria in a colony triples every hour.
a) Set up a recurrence relation for the number of bacteria after n hours have elapsed.
b) If 100 bacteria are used to begin a new colony, how many bacteria will be in the colony in 10 hours?
>Solution
Let the initial number of bacteria be $a_0$, and the number of bacteria after $n$ hours be $a_n$
$$
\begin{aligned}
a_n &= 3a_{n-1}\\
&= 3^2 \cdot a_{n-2}\\
&= 3^3 \cdot a_{n-3}\\
&=\cdots\\
&= 3^n \cdot a_0\\
a_0&=100 \To a_{10} = 3^{10} \cdot 100
\end{aligned}
$$

22\. An employee joined a company in 2009 with a starting salary of $\$50,000$. Every year this employee receives a raise of $\$1000$ plus $5\%$ of the salary of the previous year.
a) Set up a recurrence relation for the salary of this employee n years after 2009.
b) What will the salary of this employee be in 2017?
c) Find an explicit formula for the salary of this employee $n$ years after 2009.
>Solution
Let the salary in 2009 be $a_0=50000$, and the salary after $n$ years be $a_n$.
$$
\begin{aligned}
a_n &= a_{n-1} \cdot 1.05 + 1000\\
&= [a_{n-2} \cdot 1.05 + 1000] \cdot 1.05 + 1000\\
&= a_{n-2} \cdot 1.05^2 + 1000 \cdot 1.05^1 + 1000\\
&= [a_{n-3} \cdot 1.05 + 1000] \cdot 1.05^2 + 1000 \cdot 1.05^1 + 1000\\
&= a_{n-3} \cdot 1.05^3 + 1000 \cdot 1.05^2 + 1000 \cdot 1.05^1 + 1000\\
&= \cdots \\
&= a_0 \cdot 1.05^n + 1000 \cdot 1.05^{n-1} + \cdots + 1000 \cdot 1.05^2 + 1000 \cdot 1.05^1 + 1000\\
&= a_0 \cdot 1.05^n + 1000(1.05^{n-1} + \cdots + 1.05^0)\\
&= a_0 \cdot 1.05^n + 1000 \cdot \frac{1.05^n-1}{1.05-1}\\
&= 50000 \cdot 1.05^n + 20000 \cdot 1.05^n - 200000\\
&= 70000 \cdot 1.05^n-20000\\
\end{aligned}
$$
When the year is 2017, $n=8$, $a_8= 70000 \cdot 1.05^n-20000 \approx 83421.88$.
