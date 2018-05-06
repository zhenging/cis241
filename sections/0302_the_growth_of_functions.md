### Section 3.2 The Growth of Functions
pg237: 10, 13, 15, 16, 25, 26

10\. Show that $x^3$ is $O(x^4)$ but that $x^4$ is not $O(x^3)$.
>Solution
1\. $x^3$ is $O(x^4)$. When $x>1$, $x^3 < x^4$. With witnesses $C=1, k=1$ , $x^3$ is $O(x^4)$.
2\. $x^4$ is not $O(x^3)$. Proof by contradiction. The contradiction is "$x^4$ is $O(x^3)$".
a. There exists some $C$, where $|x^4| \leqslant C\cdot |x^3|$. It follows that $C \geqslant |x|$.
b. $C$ is constant and $x$ can be arbitriarily large in magnitue. So there is no such $C$ such that $C \geqslant |x|$.
c. The contradiction is false. Thus $x^4$ is not $O(x^3)$.

13\. Show that $2^n$ is $O(3^n)$ but that $3^n$ is not $O(2^n)$. (Note that this is a special case of Exercise 60.)
>Solution
1\. $2^n$ is $O(3^n)$. When $n>0$, $2^n < 3^n$. With witnesses $C=1, k=0$, $2^n$ is $O(3^n)$.
2\. $3^n$ is not $O(2^n)$. Proof by contradiction. The contradiction is "$3^n$ is $O(2^n)$".
a. There exists some $C$, where $3^n \leqslant C\cdot 2^n$. It follows that $C \geqslant (\frac{3}{2})^n$.
b. $C$ is constant and $n$ can be arbitriarily large in magnitue. So there is no such $C$ such that $C \geqslant (\frac{3}{2})^n$.
c. The contradiction is false. Thus $3^n$ is not $O(2^n)$.

15\. Explain what it means for a function to be $O(1)$.
>Solution
There are real numbers $C$ and $K$ such that $|f(x)| \leqslant C$ and $x>k$. $f(x)$ is bounded by $C$ for all sufficiently large $x$. In other word, the excution time of an algorithm whoes complexity is $O(1)$  does not depent on the size of input.

16\. Show that if $f(x)$ is $O(x)$, then $f(x)$ is $O(x^2)$.
>Solution
There are constants $C$ and $k$, such that $|f(x)| \leqslant C|x|$ and $x>k$.
$$
|f(x)| \leqslant C|x| \To |f(x)| \leqslant C|x^2| \text{ when } x>max(1, k)
$$
There are constant $C$ and $k_{max}=(1, k)$ such that $|f(x)| \leqslant C|x^2|$ and $x>k_{max}$. Thus $f(x)$ is $O(x^2)$.

25\. Give as good a big-$O$ estimate as possible for each of these functions.
a) $(n^2 + 8)(n + 1)$
>Solution
1\. $(n^2 + 8)$ is $O(n^2)$ and $n + 1$ is $O(n)$.
2\. $(n^2 + 8)(n + 1)$ is $O(n^2 \cdot n) = O(n^3)$.

b) $(n\log n + n^2)(n^3 + 2)$
>Solution
1\. $(n\log n + n^2)$ is $O(n^2)$ and $(n^3 + 2)$ is $O(n^3)$.
2\. $(n\log n + n^2)(n^3 + 2)$ is $O(n^2 \cdot n^3) = O(n^5)$.


c) $(n! + 2^n)(n^3 + \log(n^2 + 1))$
>Solution
1\. $n! + 2^n$ is $O(n!)$.
2\. $n^3 + \log(n^2 + 1)$. When $n>2$
$$
n^3 + \log(n^2 + 1) \leqslant n^3 + \log(2n^2) \leqslant n^3 + \log 2 + 2\log(n) \leqslant 3n^3
$$
Thus $n^3 + \log(n^2 + 1)$ is $O(n^3)$.
3\. $(n! + 2^n)(n^3 + \log(n^2 + 1))$ is $O(n! \cdot n^3)$.

26\. Give a big-$O$ estimate for each of these functions. For the function g in your estimate $f(x)$ is $O(g(x))$, use a simple function $g$ of smallest order.
a) $(n^3+n^2\log n)(\log n+1) + (17 \log n+19)(n^3+2)$
>Solution
1\. $(n^3+n^2\log n)$ is **$O(n^3)$**.
2\. $(\log n+1)$ is **$O(\log n)$**.
3\. $(n^3+n^2\log n)(\log n+1)$ is **$O(n^3 \log n)$**
4\. $(17 \log n+19)$ is **$O(\log n)$**.
5\. $(n^3+2)$ is **$O(n^3)$**.
6\. $(17 \log n+19)(n^3+2)$ is **$O(n^3 \log n)$**.
7\. $(n^3+n^2\log n)(\log n+1) + (17 \log n+19)(n^3+2)$ is **$O(n^3 \log n)$**.

b) $(2^n + n^2)(n^3 + 3^n)$
>Solution
1\. $(2^n + n^2)$ is $O(2^n)$.
2\. $(n^3 + 3^n)$ is $O(3^n)$.
3\. $(2^n + n^2)(n^3 + 3^n)$ is $O(3^n \cdot 2^n) = O(6^n)$

c) $(n^n + n2^n + 5^n)(n! + 5^n)$
>Solution
1\. $(n^n + n2^n + 5^n)$. When $n \geqslant 5$
$$
\begin{aligned}
n2^n &< n^n \text{ and } 5^n < n^n \To n^n + n2^n + 5^n < 3n^n\\
&\To (n^n + n2^n + 5^n) \text{ is } O(n^n)
\end{aligned}
$$
2\. $(n! + 5^n)$. When $n \geqslant 12$
$$
\begin{aligned}
n! &> 5^n \To n! + 5^n < 2n!\\
&\To (n! + 5^n) \text{ is } O(n!)
\end{aligned}
$$
3\. $(n^n + n2^n + 5^n)(n! + 5^n)$ is $O(n^n \cdot 2n!)$.
