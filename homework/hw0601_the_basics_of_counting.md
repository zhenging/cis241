### Section 6.1 The Basics of Counting
pg417: 1, 6, 10, 12, 17, 28, 32a-f, 34, 37a-b,48, 49, 55, 56

1\. There are 18 mathematics majors and 325 computer science majors at a college.
a) In how many ways can two representatives be picked so that one is a mathematics major and the other is a computer science major?
>Solution
By product rule, there are $18 \times 325 = 5850$ ways to pick up such two representatives.

b) In how many ways can one representative be picked who is either a mathematics major or a computer science major?
>Solution
By sum rule, there are $18 + 325 = 343$ ways to pick up such representative.

6\. There are four major auto routes from Boston to Detroit and six from Detroit to Los Angeles. How many major auto routes are there from Boston to Los Angeles via Detroit?
>Solution
By product rule, there are $4 \times 6 = 24$ routes from Boston to LA via Detroitt.

10\. How many bit strings are there of length eight?
>Solution
For each bit, there are 2 choices ($0$ or $1$). By product rule, there are $2^8$ of such bit strings.

12\. How many bit strings are there of length six or less, not counting the empty string?
>Solution
Let the length of such bit string be $n | 0 < n \leqslant 6$.
1\. For each bit, there are $2$ choices($0$ or $1$). By product rule, there are $2^n$ of such bit strings.
2\. when $n=6$, there are $2^6$ of such bit strings; $n=5$, there are $2^5$ of such bit strings, etcetera.
3\. By sum rule, there are total $2^6 + 2^5 + 2^4 + 2^3 + 2^2 + 2^1$ of such bit strings.

17\. How many strings of five ASCII characters contain the character @ ("at" sign) at least once? [Note: There are 128 different ASCII characters.
>Solution
1\. The number of strings of five ASCII characters is $128^5$.
2\. The number of strings of five ASCII characters that do not contain @ is $127^5$.
3\. By exclusion, the number of strings of five ASCII characters contain @ at least once is $128^5-127^5$.


28\. How many license plates can be made using either three digits followed by three uppercase English letters or three uppercase English letters followed by three digits?
>Solution
1\. When plates use three digits followd by three uppcase English letters, each of the first three characters has $10$ choices, and each of the last three characters has $26$ choices. By product rule, there are total $10^3 \cdot 26^3$ ways of combinations.
2\. When plates use three uppercase English letters followd by three digits, each of the first three characters has $26$ choices, and each of the last three characters has $10$ choices. By product rule, there are total $26^3 \cdot 10^3$ ways of combinations.
3\. By sum rule, there are total $10^3 \cdot 26^3 + 26^3 \cdot 10^3 = 2 \cdot 10^3 \cdot 26^3$ ways of combinations.

32\. How many strings of eight uppercase English letters are there?
a) if letters can be repeated?
>Solution
a. There are $26$ choices for each character. By product rule, there are total $26^8$ such strings.

b) if no letter can be repeated?
>Solution
There are $26$ choices for the first character; there are $26-1=25$ choices for the 2nd character; there are $26-2=24$ choices for the 3rd character, ..., and there are $26-7=19$ for the 8th character. By product rule, there are total $26 \times 25 \times 24 \times 23 \times 22 \times 21 \times 20 \times 19$ such strings.

c) that start with X, if letters can be repeated?
>Solution
There are only $1$ choice for the first character, and there are $26$ choices for each of the rest characters. By product rule, there are total $1 \times 26^7 = 26^7$ such strings.

d) that start with X, if no letter can be repeated?
>Solution
There are only $1$ choice for the 1st character; there are $26-1=25$ choices for the 2nd character; there are $26-2=24$ choices for the 3rd character,..., there are $26-7=19$ choices for the 8th character. By product rule, there are total $1 \times 25 \times 24 \times 23\times 22\times 21 \times 20\times 19$ such strings.

e) that start and end with X, if letters can be repeated?
>Solution
There are $1$ choice for both the lst and last characters, and there are $26$ choices for each of the rest 6 characters. By product rule, there are total $1 \times 26^6 \times 1$ such strings.

f) that start with the letters BO (in that order), if letters can be repeated?
>Solution
There are $1$ choice for both the 1st and 2nd characters, and there are $26$ choices for each of the rest 6 characters. By product rule, there are total $1 \times 1 \times 26^6$ such strings.


34\. How many different functions are there from a set with $10$ elements to sets with the following numbers of elements?
a) 2 &emsp; b) 3 &emsp; c) 4 &emsp; d) 5
>Solution
Let the length of set I be $m=10$, and the length of set II be $n$ ($n<m$ in this case), and the total number of different functions from set I to set II is $C$.
There are $n$ ways to map each element of set I to set II. By production rule, there are total $n^m$ ways of such mappings, namely $C=n^m=n^{10}$.
a. $C|_{n=2} = 2^{10}$ &emsp; b. $C|_{n=3} = 3^{10}$ &emsp;c. $C|_{n=4} = 4^{10}$ &emsp; d. $C|_{n=5} = 5^{10}$

37\. How many functions are there from the set $\{1, 2,...,n\}$, where $n$ is a positive integer, to the set $\{0, 1\}$
a) that are one-to-one?
>Solution
Let the 1-to-1 function be $f$
case 1: if $n>2$, there is no 1-to-1 functions.
case 2: if $n=2$, there are $2$ 1-to-1 functions. These functions are
$$
\begin{aligned}
f_1(1) &= 0, f_1(2) = 1 \\
f_2(1) &= 1, f_2(2) = 0
\end{aligned}
$$
case 3: if $n=1$, there are $2$ 1-to-1 functions. These functions are
$$
\begin{aligned}
f_1(1) &= 0\\
f_2(1) &= 1
\end{aligned}
$$

b) that assign 0 to both 1 and n?
>Solution
There are $2$ ways to map each element , that is not $1$ nor $n$, in set I,  to set II. There are only $1$ way to map element $1$ and $n$ to set II ($f(1) = 0, f(n)=0$). By production rule, there are total $1\times 2^{n-1} \times 1$ functions from set I to set II.


48\.How many bit strings of length seven either begin with two 0s or end with three 1s?
>Solution
1\. The number of bit strings that begin with two 0s is $1^2 \times 2^5 = 2^5$.
2\. The number of bit strings that end with three 1s is $2^4 \times 1^3 = 2^4$.
3\. The number of bit strings that begin with two 0s and end with three 1s is $1^2 \times 2^2 \times 1^3 = 2^2$.
4\. By inclusion and exclusion, the number of such string is $2^5+2^4-2^2=44$.

49\. How many bit strings of length 10 either begin with three 0s or end with two 0s?
>Solution
1\. The number of bit strings that begin with three 0s is $1^3 \times 2^7 = 2^7$.
2\. The number of bit strings that end with two 1s is $2^8 \times 1^2 = 2^8$.
3\. The number of bit strings that begin with three 0s and end with two 1s is $1^3 \times 2^5 \times 1^2 = 2^5$.
4\. By inclusion and exclusion, the number of such string is $2^7+2^8-2^5=352$.


55\. Suppose that a password for a computer system must have at least 8, but no more than 12, characters, where each character in the password is a lowercase English letter, an uppercase English letter, a digit, or one of the six special characters âˆ—, >, <, !, +, and =.
a) How many different passwords are available for this computer system?
>Solution
Let the length of the password be an integer $n \mid 8 \leqslant n \leqslant 12$
There are $26+26+10+6=68$ choices for each character. By product rule, the number of different passwords with length of $n$ is $68^n$. By sum rule, the total number of such passwords is $68^8 + 68^9 + 68^{10} + 68^{11} + 68^{12}$.

b) How many of these passwords contain at least one occurrence of at least one of the six special characters?
>Solution
Let the total number of passwords in part a) be $C_{total}$, the number of password that does not contain any of the six special characters be $C_{nospecial}$, and the number of passwords contain at least one occurence of at least one of the six special characters be $C_{special}$.
1\. By exclusion, $C_{special} = C_{total} - C_{nospecial}$.
2\. According to part a), $C_{total} = 68^8 + 68^9 + 68^{10} + 68^{11} + 68^{12}$. Similarly, $C_{nospecial} = 62^8 + 62^9 + 62^{10} + 62^{11} + 62^{12}$.
3\. $C_{special} = 68^8 + 68^9 + 68^{10} + 68^{11} + 68^{12} - (62^8 + 62^9 + 62^{10} + 62^{11} + 62^{12})$

c) Using your answer to part (a), determine how long it takes a hacker to try every possible password, assuming that it takes one nanosecond for a hacker to check each possible password.
>Solution
The time is $(68^8 + 68^9 + 68^{10} + 68^{11} + 68^{12}) \times 10^{-9}s \approx 314582 \: years$

56\. The name of a variable in the C programming language is a string that can contain uppercase letters, lowercase letters, digits, or underscores. Further, the first character in the string must be a letter, either uppercase or lowercase, or an underscore. If the name of a variable is determined by its first eight characters, how many different variables can be named in C? (Note that the name of a variable may contain fewer than eight characters.)
>Solution
Let the length of the variable name be an positive integer $n |0 < n\leqslant 8$.
1\. There are $26+26+1 = 53$ choices for the 1st character, and  there are $26+26+10+1 = 63$ choices for the rest of each character.
2\. By product rule, there are total $53 \times \overbrace{63 \times 63 \cdots \times 63}^{n-1 \: times} = 53 \times 63^{n-1}$ such different variables with length of $n$.
3\. By sum rule, there are total $53 \times 63^{8-1} + 53 \times 63^{7-1} + \cdots \times 53 \times 63^{1-1} = 53(63^7 +63^6+ \cdots + 63^0)$ different variables can be named in C.
