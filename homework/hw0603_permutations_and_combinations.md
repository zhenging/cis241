### Section 6.3 Permutations and Combinations
pg434: 8, 10, 11, 12, 14, 16, 19, 22a,b,c, 27, 33, 34

8\. In how many different orders can five runners finish a race if no ties are allowed?
>Solution
Because the order matters, the number of different orders in this race is the number of 5-**permutations** of a set of 5 elements. Consequently, the answers is $P(5, 5) = 5! = 120$.

10\. There are six different candidates for governor of a state. In how many different orders can the names of the candidates be printed on a ballot?
>Solution
Because the order matters, the number of different orders of names is the number of 6-**permutations** of a set of 6 elements. Consequently, the answers is $P(6, 6) = 6! = 720$.

11\. How many bit strings of length 10 contain
a) exactly four 1s?
b) at most four 1s?
c) at least four 1s?
d) an equal number of 0s and 1s?
>Solution
Because the order of 1s doesn't matter, the number of bit strings of length $10$ contain exactly $n$ 1s can be given by the number of $n$-**combinations** of a set of $10$ elements, where  $n \mid 0 \leqslant n \leqslant 10$. That is
$$
C(10, n) = \frac{10!}{(10-n)!n!}
$$
a. The number of bit string of length 10 contain exactly $4$ 1s is $C(10, 4) = \dfrac{10!}{(10-4)!4!} = 210$
b. By sum rule, the number of bit string of lenght 10 contains at most four 1s is the sum of numbers of bit strings contain exactly $n$ 1s, where is this case $0 \leqslant n \leqslant 4$.
$$
C_b = C(10, 0) + C(10, 1) + C(10, 2) + C(10, 3) + C(10, 4)
$$
c. By sum rule, the number of bit string of lenght 10 contains at least four 1s is the sum of numbers of bit strings contain exactly $n$ 1s, where in this case $4 \leqslant n \leqslant 10$.
$$
C_c = C(10, 4) + C(10, 5) + \cdots + C(10, 10)
$$
d. The answer can be given by the number of bit strings of length of 10 contain exactly $5$ 1s, that is
$$
C_d = C(10, 5) = \frac{10!}{5!5!} = 252
$$


12\. How many bit strings of length 12 contain
a) exactly three 1s?
b) at most three 1s?
c) at least three 1s?
d) an equal number of 0s and 1s?
>Solution
Because the order of 1s doesn't matter, the number of bit strings of length $12$ contain exactly $n$ 1s can be given by the number of $n$-**combinations** of a set of $12$ elements, where  $n \mid 0 \leqslant n \leqslant 12$. That is
$$
C(12, n) = \frac{12!}{(12-n)!n!}
$$
a. The number of bit string of length 12 contain exactly $3$ 1s is $C(12, 3) = \dfrac{12!}{(12-3)!3!} = 220$
b. By sum rule, the number of bit string of lenght 12 contains at most three 1s is the sum of numbers of bit strings contain exactly $n$ 1s, where is this case $0 \leqslant n \leqslant 3$.
$$
C_b = C(12, 0) + C(12, 1) + C(12, 2) + C(12, 3)
$$
c. By sum rule, the number of bit string of lenght 12 contains at least three 1s is the sum of numbers of bit strings contain exactly $n$ 1s, where in this case $3 \leqslant n \leqslant 12$.
$$
C_c = C(12, 3) + C(12, 4) + \cdots + C(12, 12)
$$
d. The answer can be given by the number of bit strings of length of 12 contain exactly $6$ 1s, that is
$$
C_d = C(12, 6) = \frac{12!}{6!6!} = 924
$$

14\. In how many ways can a set of two positive integers less than 100 be chosen?
>Solution
Because the order of chosen integers doesn't matter, the number of ways to choose 2 positive integers less than 100 is the number of $2$-**combinations** of a set of 99 elements. Consequently, the answer is
$$
C(99, 2)= \frac{99!}{97!2!} = 4851
$$

16\. How many subsets with an odd number of elements does a set with 10 elements have?
>Solution
Let the number of elements of such one subset be $n$, where $n \in [1, 3, 5, 7, 9]$.
1\. Because the order doesn't matter, the number of subsets with $n$ elements is the number of $n$-**combinations** of a set with 10 element.
2\. By sum rule, the **number of subsets** with an odd number of elements of a set with 10 elements is **the sum** of the numbers of subsets with $n$ elements. That is
$$
C = C(10, 1) + C(10, 3) + C(10, 5) + C(10, 7)+ C(10, 9)
$$


19\. A coin is flipped 10 times where each flip comes up eitherheads or tails. How many possible outcomes
a) are there in total?
b) contain exactly two heads?
c) contain at most three tails?
d) contain the same number of heads and tails?
>Solution
a. By product rule, the total number is $2^{10}$.
b. Because the order of heads doesn't matter, the number of possible outcomes contain exactly two heads is the number of 2-**combinations** of a set of 10 elements. The answer is $C(10, 2) = \dfrac{10!}{8!2!} = 45$.
c. By sum rule, the number of possible outcomes contain at most three tails is the sum of numbers of possible outcomes contain exactly $n$ tails, where in this case $n\in [0, 1, 2, 3]$. That is
$$
C_c = C(10, 0) + C(10, 1) + C(10, 2) + C(10, 3)
$$
d. The answer can be given by the number of possible outcomes contain exactly $5$ heads, that is
$$
C_d = C(10, 5) = \frac{10!}{5!5!} = 252
$$

22\. How many permutations of the letters ABCDEFGH contain
a) the string ED?
b) the string CDE?
c) the strings BA and FGH?
>Solution
a. We can treat "ED" as one element, then the answer can be given by the number of 7-**permutations** of a set of 7 elements. That is $P(7, 7) = 7! = 5040$.
b. We can treat "CDE" as one element, then the answer can be given by the number of 6-**permutations** of a set of 6 elements. That is $P(6, 6) = 6! = 720$.
c. We can treat "BA" and "FGH" as two elements, then the answer can be given by the number of 5-**permutations** of a set of 5 elements. That is $P(5, 5) = 5! = 120$.

27\. A club has 25 members.
a) How many ways are there to choose four members of the club to serve on an executive committee?
b) How many ways are there to choose a president, vice president, secretary, and treasurer of the club, where no person can hold more than one office?
>Solution
a. Because the order of chosen members doesn't matter, the number of choosing 4 members from the club is the number of 4-**combinations** of a set of 25 elements. The answer is $C(25, 4) = \frac{25!}{21!4!}=12650$.
b. Because the order of chosen members matters, the number of choosing 4 members from the club is the number of 4-**permutions** of a set of 25 elements. The answer is $P(25, 4) = \frac{25!}{21!}=303600$.


33\. Suppose that a department contains 10 men and 15 women. How many ways are there to form a committee with six members if it must have the same number of men and women?
>Solution
1\. We need to choose 3 women from 15 women and 3 men from 10 men.
2\. Because the order doesn't matter, the number $C_{w}$ of ways to choose 3 women from 15 women is the number of 3-**combinations** of a set of 15 elements. The number $C_{m}$ of ways to choose 3 men from 10 women is the number of 3-**combinations** of a set of 10 elements. It follows that
$$
\begin{aligned}
C_{w} &= C(15, 3) = \frac{15!}{12!3!} = 455\\
C_{m} &= C(10, 3) = \frac{10!}{7!3!} = 120
\end{aligned}
$$
3\. By product rule, the number of ways to form such committee is $C_{w} \cdot C_{m} = 455 \cdot 120 = 54600$

34\. Suppose that a department contains 10 men and 15 women. How many ways are there to form a committee with six members if it must have more women than men?
>Solution
Let the numbers of women and men in the committee be $w$ and $m$ respectively, where $w+m=6$ and $w>m$. It follows that
$$
[w,m] \in \{[6, 0], [5, 1], [4, 2]\}
$$
1\. The number $C_w$ of ways to choose $w$ women from 15 women is the number of $w$-**combinations** of a set of 15 elements. The number $C_m$ of ways to choose $m$ men from 10 men is the number of $m$-**combinations** of a set of 10 elements.
2\. By product rule, the number of ways to form a commiitee with $w$ women and $m$ man is $C_{w} \cdot C_{m} = C(15, w) \cdot C(10, m))$.
3\. By sum rule, the total number of ways to form a committee if it must have more women than men is
$$
C = C(15, 6)\cdot C(10, 0) + C(15, 5)\cdot C(10, 1)+C(15, 4)\cdot C(10, 2)
$$
