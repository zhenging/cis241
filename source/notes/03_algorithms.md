#### 3. Algorithms
##### 3.1 Algorithms

##### 3.2 The growth of Functions
**EX** 1, 2, 3, 4, 8, 12, 13, Fig 3
**HW** pg 237: 10, 13, 15, 16, 25, 26

1\. **Definion of Big-O Notation**
Let $f$ and $g$ function from the set of integers or the set of real numbers to the set of real numbers, we say that $f(x)$ is $O(g(x))$ of there are constant $C$ and $k$ such that
$$
|f(x)| \leqslant C|g(x)|
$$
whenever $x>k$. [This is read as $f(x)$ is big oh of $g(x)$].
2\. Suppose that $f_1(x)$ is $O(g_1(x))$, and  $f_2(x)$ is $O(g_2(x))$, then $(f_1+f_2)(x)$ is $O(max(|g_1(x)|, |g_2(x)|))$.
3\. Suppose that $f_1(x)$ is $O(g_1(x))$, and  $f_2(x)$ is $O(g_2(x))$, then $(f_1f_2)(x)$ is $O(g_1(x)g_2(x)))$.
4\. BigOmega and Big-Theta Notation.

##### 3.3 Complexity of Algorithm
