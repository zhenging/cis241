### Mid Term
(1a) Are the following expressiongs $\neg p \to (q\to r)$ and $q \to (p \lor r)$ logically equivalent? Prove or Disprove.
>Solution
Todo

(1b) Determine the truth value of the statement: $\exists a \forall b (b^2 \ges a)$ if the domain of the variable consists of the positive (non-zero) real numbers.
>Solution
The statement is false. There are three cases:
case #1: $a>1$, when $b=1$, $b^2 \ges a$ is false.
case #2: $a=1$, when $b=0.5$, $b^2 \ges a$ is false.
case #3: $0<a<1$, when $b=a$, $b^2 \ges a$ is false.
No matter what value we choose for $a$ in its domain, there is alwasy some value for $b$, that $b^2 \ges a$ is false.

>Solution
Let $p$ be the statement $\exists a \forall b (b^2 \ges a)$ and $s$ be the statement $\neg p$.
$$
\begin{aligned}
s &\equiv \neg(\exists a \forall b (b^2 \ges a))\\
&\equiv \forall a \exists b (b^2 < a)\\
\end{aligned}
$$
For every $a$, let $b=\frac{\sqrt a}{2}$, we have
$$
\begin{aligned}
b^2 &= (\frac{\sqrt a}{2})^2\\
b^2 &= \frac{a}{4} < a
\end{aligned}
$$
Thus the statement $s$ is true, and the original statement $p$ is false.

(2a) Prove that: $\sqrt[3]{2}$ is irrational.
>Solution
Todo

(2b) Let k be interger. Prove: If $k^3$ is odd, then $k^2 + 1$ is even.
>Solution
To prove the statment, we first need to prove that if $k^3$ is odd, then $k$ is odd.
(1) By contrapositive, the contraposition is: if $k$ is even, then $k^3$ is even.
Let $k=$, where $n$ is an integer. We have
$$
\begin{aligned}
k^3 &=(2n)^3
\\ &=8n^3 = 2 \cdot (4n^3)
\end{aligned}
$$
The contraposition is true. Thus the statement that if $k^3$ is odd, then $k$ is odd, is proved.
(2) From (1), we know that $k$ is odd. Let $k=2m+1$,
$$
\begin{aligned}
k^2 + 1 &= (2m+1)^2 + 1\\
&= 2(2m^2+2m+1)
\end{aligned}
$$
$k^2 + 1$ is even.Thus the original statment is proved.

(3a) Let $h$ be a function from a set $X$ to a set $Y$. Let A and B be subsets of set $X$. Prove: $h(A) \cup h(B) \subseteq h(A\cup B)$
>Solution
Let $y \in h(A) \cup h(B)$,
case #1: $y \in h(A)$, by defintion, $\exists (a_1\in A) h(a_1) = y$
$$
\begin{aligned}
y \in h(A) &\To a_1 \in A\\
&\To a_1 \in A \cup B\\
&\To h(a_1) \in h(A \cup B)\\
&\To y \in h(A \cup B)
\end{aligned}
$$
case #2: $y \in h(B)$, by defintion, $\exists (a_2\in B) h(a_2) = y$
$$
\begin{aligned}
y \in h(A) &\To a_2 \in B\\
&\To a_2 \in A \cup B\\
&\To h(a_2) \in h(A \cup B)\\
&\To y \in h(A \cup B)
\end{aligned}
$$
In both cases, we proved if $y \in h(A) \cup h(B)$, then $y \in h(A\cup B)$. Thus. the original statement is proved.

(4a) How many bit strings of length 12 either start with _00_ or end with _1111_?
>Solution
Strings start with _00_: $2^{10}$.
Strings end with _1111_: $2^{8}$.
Strings start with _00_ and end with _1111_: $2^{6}$
Because of double counting, by inclusion/exclusion principle, the number of strings either start with _00_ or end with _1111_ is $2^{10} + 2^8 - 2^6$.

(4b) How many _one-to-one_ functions are there from a set of $p$ elements to a set of $s$ elements?
>Solution
Let the set of $p$ elements be $P$, and the set of $s$ elements be $S$
case #1: when $p>s$, there is no _one-to-one_ function.
case #2: when $p \les s$, there are $s$ ways to map $p_1$ to $S$, there are $(s-1)$ ways to map $p_2$ to $S$, so on so forth, there are $(s-p+1)$ ways to map $p_p$ to $S$. By product rule, the total of _one-to-one_ functions is $s(s-1)(s-2) \cdots (s-p+1)$.

(5a) Prove that 133 divides $11^{k+2} + 12^{2k-1}$ whenever $k$ is positive integer.
>Solution
Todo

(5b) Prove that: $16^n$ is not $O(15^n)$.
>Solution
By contradiction, the contradiction is: $16^n$ is $O(15^n)$.
(1) By definition of $O$, $\exists c,k (16^n \les C\cdot 15^n) \forall n>k$, then we have
$$
\begin{aligned}
16^n \les C\cdot 15^n\\
C \ges (\frac{16}{15})^n
\end{aligned}
$$
(2) Because $\dfrac{16}{15} \ges 1$ and $n$ can be arbitraily large, $\dlim_{n \to \infty}(\frac{16}{15})^n = \infty$.
(3) There is no such constant $C$, which statisfies $C \ges (\frac{16}{15})^n$.
(4) Thus the contradiction is false.
The original statment is _true_.

(6a) Let $K$ be a positive integer. Let $n$ be a positive integer. Let $x$ be integer. _Prove_ that among any group of $nx+1$ (not necessarily consecutive) integers, there are _at least_ $(n+1)$ with exactly the same reminder when they are divided by $x$.
>Solution
The possible reminders of a number divided by $x$ are $0, 1, 2, \cdots, x-1$. The total of the reminders is $x$.
_Objects_: $nx+1$ integers
_Boxes_: $x$ reminders
By the Piegeon Hole Principle, the number of integers with same reminders is at least
$$
\lceil \frac{nx+1}{x} \rceil = \lceil n+ \frac{1}{x} \rceil = n+1
$$

(6b) Let $X$ be a set with $m$ elements. Prove that the number of subsets is: $2^m$
>Solution
1\. The number of subsets with $n$ elements is $C(m, n)$ (combination), where $ 0 \les n \les m$.
2\. The number of all subsets is
$$
C(m, 0) + C(m, 1) + \cdots + C(m, m) = \sum_{n=0}^m C(m, n)
$$
3\. Let $x=1, y=1$
$$
\begin{aligned}
2^m = (x+y)^m &= \sum_{n=0}^m C(m, n) x^{n-k} y^k\\
& = \sum_{n=0}^m C(m, n) 1^{n-k} 1^k\\
&= \sum_{n=0}^m C(m, n)
\end{aligned}
$$
According to (2) and (3), the statement is proved.

(7a) Suppose a password for a computer system must have at least 7, but no more than 11 characters where each character in the password is a lower case English letter, an upper case English letter, a binary digit, or one of the seven special characters (*, >, <, !, +, =, $). How many of these password contain at least one occurence of at least one of the seven special characters?
>Solution
$$
\begin{aligned}
C_{total} &= 61^{11}+ 61^{10} + 61^{9} + 61^{8} + 61^{7}\\
C_{nospecial} &= 54^{11}+ 54^{10} + 54^{9} + 54^{8} + 54^{7}\\
C_{special} &= C_{total} - C_{special}
\end{aligned}
$$

(7b) Assume strings of length 8 are formed with letters: _ABCDEFGH_. Calculate the numbers of strings that contain the substrings: _AB_ and _FGH_
>Solution
We can treat _AB_ and _FGH_ as two individual elements, then the answer can be given by the number of 5-**permutations** of a set of 5 elements. That is $P(5, 5)$.

(8a) Give an example of a relation that both symmetric and anti-symmetric. Define the set and the relation.
>Solution
1\. Let the set be $A$ and $A=\emptyset$.
2\. Let the relation be $R$ and $R \subseteq A \times A = \emptyset$.
Because the assumption that there are elements in $A$ is false, the conclusion $R$ is symmetric and anti-symmetric is true.

(8b) Assume string of length 10 formed by letters _M_ and/or _W_. Calculate the number of strings that contain at most four _M_ s.
>Solution
