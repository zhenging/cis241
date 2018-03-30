## Chapter 08 Advanced Counting Techniques

### 8.1 Applications of Recurrence Relations
p522
Ex: 1, 2

EXAMPLE 1
**Rabbits and the Fibonacci Numbers** Consider this problem, which was originally posed by Leonardo Pisano, also known as Fibonacci, in the thirteenth century in his book Liber abaci. A young pair of rabbits (one of each sex) is placed on an island. A pair of rabbits does not breed until they are 2 months old. After they are 2 months old, each pair of rabbits produces another pair each month, as shown in Figure 1. Find a recurrence relation for the number of pairs of rabbits on the island after n months, assuming that no rabbits ever die.

EXAMPLE 2
**The Tower of Hanoi** A popular puzzle of the late nineteenth century invented by the French mathematician Édouard Lucas, called the Tower of Hanoi, consists of three pegs mounted on a board together with disks of different sizes. Initially these disks are placed on the first peg in order of size, with the largest on the bottom (as shown in Figure 2). The rules of the puzzle allow disks to be moved one at a time from one peg to another as long as a disk is never placed on top of a smaller disk. The goal of the puzzle is to have all the disks on the second peg in order of size, with the largest on the bottom.
Let ${H_n}$ denote the number of moves needed to solve the Tower of Hanoi problem with $n$ disks. Set up a recurrence relation for the sequence ${H_n}$.

### 8.2 Solving Linear Recurrence Relations
p535
Ex: 1-6

> Definition
A _linear homogeneous recurrence relation of degree $k$ with constant coefficients_ is a recurrence relation of the form
$$
\begin{aligned}
a_n = c_1a_{n-1} + c_2a_{n-2} + \cdots + c_ka_{n-k},
\end{aligned}
$$
where $c_1, c_2, \cdots c_k$ are real numbers, and $c_k \ne 0$.

+ **Linear** - the right-hand side is a sum of previous terms of the sequence each multiplied by a function of $n$.
+ **Homogeneous** - no terms occur that are not multiplies of $a_j$s.
+ **Constants** - the coefficients of the terms are constants
+ **Degree** - $a_n$ is expressed in terms of the previous $k$ terms of the sequence.

Example 1
The recurrence relation $P_n = (1.11)P_{n-1}$ is a linear homogeneous recurrence relation of degree _one_. The recurrence relation $f_n = f_{n-1} + f_{n-2}$ is a linear homogeneous recurrence relation of degree _two_. The recurrence relation $a n = a_{n-5}$ is a linear homogeneous recurrence relation of degree _five_.

Example 2
The recurrence relation $a_n = a_{n-1} + a_{n-2}$ is not linear. The recurrence relation $H_n = 2H_{n-1} + 1$ is not homogeneous. The recurrence relation $B_n = nB_{n-1}$ does not have constant
coefficients.

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
