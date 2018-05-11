### 8.3 Divide-and-Conquer Algorithms and Recurrence Relations
p548
Ex: 1, 3, 5, 9

EXAMPLE 1
**Binary Search** We introduced a binary search algorithm in Section 3.1. This binary search algorithm reduces the search for an element in a search sequence of size $n$ to the binary search for this element in a search sequence of size $n/2$, when $n$ is even. (Hence, the problem of size $n$ has been reduced to one problem of size $n/2$.) Two comparisons are needed to implement this reduction (one to determine which half of the list to use and the other to determine whether any terms of the list remain). Hence, if $f (n)$ is the number of comparisons required to search for an element in a search sequence of size $n$, then
$$
\begin{aligned}
f(n) = f(n/2) + 2
\end{aligned}
$$

EXAMPLE 3
**Merge Sort** The merge sort algorithm (introduced in Section 5.4) splits a list to be sorted with n items, where n is even, into two lists with n/2 elements each, and uses fewer than n comparisons to merge the two sorted lists of n/2 items each into one sorted list. Consequently, the number of comparisons used by the merge sort to sort a list of n elements is less than M(n), where the function M(n) satisfies the divide-and-conquer recurrence relation
$$
\begin{aligned}
M(n) = 2M(n/2) + n
\end{aligned}
$$

**MASTER THEOREM** Let $f$ be an increasing function that satisfies the recurrence relation
$$
\begin{aligned}
f(n) = af(n/b) + cn^d
\end{aligned}
$$
whenever $n = b^k$ , where $k$ is a positive integer, $a \ges 1, b$ is an integer greater than 1, and $c$ and $d$ are real numbers with $c$ positive and $d$ nonnegative. Then
$$
\begin{aligned}
f(n) \text{ is } \begin{cases}
O(n^d) &\text{if } a < b^d\\
O(n^d \log n) &\text{if } a = b^d\\
O(n^{log_b a}) &\text{if } a > b^d
\end{cases}
\end{aligned}
$$

EXAMPLE 9
**Complexity of Merge Sort** In Example 3 we explained that the number of comparisons used by the merge sort to sort a list of n elements is less than $M(n)$, where $M(n) = 2M(n/2) + n$. By the master theorem (Theorem 2) we find that $M(n)$ is $O(n \log n)$, which agrees with the estimate found in Section 5.4.

#### Homework
p535: 34, 36 (**Deprecated**)

34\. Find $f(n)$ when $n = 4k$, where $f$ satisfies the recurrence relation $f(n) = 5f (n/4) + 6n$, with $f (1) = 1$.

36\. Find $f(n)$ when $n = 2k$, where $f$ satisfies the recurrence relation $f (n) = 8f (n/2) + n^2$ with $f (1) = 1$.
