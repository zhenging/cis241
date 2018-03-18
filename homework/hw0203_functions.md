### Section 2.3 Functions
pg175: 40, 42, 44

40\. Let $f$ be a function from the set $A$ to the set $B$. Let $S$ and $T$ be subsets of $A$. Show that
a. $f(S \cup T) = f(S) \cup f(T)$.
>Solution
we need to prove **(1) $f(S \cup T) \subseteq f(S) \cup f(T)$** and **(2) $f(S) \cup f(T) \subseteq f(S \cup T)$**.
**a1**. Prove $f(S \cup T) \subseteq f(S) \cup f(T)$
Let $b \in f(S \cup T)$, it follows that $\exists (a \in S \cup T)f(a) = b$
$$
\begin{gathered}
a \in S \cup T \To a \in S \lor a \in T\\
\To \text{(Or)} \begin{cases}
a \in S \To f(a) \in f(S) \\
a \in T \To f(a) \in f(T)
\end{cases}
\To f(a) \in f(S) \cup f(T) \To b \in f(S) \cup f(T)
\end{gathered}
$$
Therefore **a1** is proved.
**a2**. Prove $f(S) \cup f(T) \subseteq f(S \cup T)$
Let $b \in f(S) \cup f(T)$, it follows that $b \in f(S) \lor b \in f(T)$
$$
\begin{aligned}
\text{case 1: } & b \in f(S) \To \exists (a_1 \in S)f(a_1) = b \\
& a_1 \in S \To a_1 \in S \cup T \\
&\To f(a_1) \in f(S \cup T) \\
&\To b \in f(S \cup T)\\
\text{case 2: } & b \in f(T) \To \exists (a_2 \in T)f(a_2) = b \\
& a_2 \in T \To a_2 \in S \cup T \\
&\To f(a_2) \in f(S \cup T) \\
&\To b \in f(S \cup T)
\end{aligned}
$$
In both cases, $b \in f(S \cup T)$. Therefore **a2** is proved.
According to **(a1)** and **(a2)**, **a** is true.

b. $f(S \cap T) \subseteq f(S) \cap f(T)$.
>Solution
Let $b \in f(S \cap T)$, it follows that $\exists (a \in S \cap T)f(a) = b$
$$
\begin{gathered}
a \in S \cap T \To a \in S \land a \in T\\
\To \text{(And)}\begin{cases}
a \in S \To f(a) \in f(S)\\
a \in T \To f(a) \in f(T)
\end{cases}
\To f(a) \in f(S) \cap f(T) \To b \in f(S) \cap f(T)
\end{gathered}
$$
Therefore **b** is true.

Let $f$ be a function from the set $A$ to the set $B$. Let $S$ be a subset of $B$. We define the **inverse image** of $S$ to be the subset of $A$ whose elements are precisely all pre-images of all elements of $S$. We denote the inverse image of S by $f^{-1}(S)$, so $f^{-1}(S) = \{a \in A | f (a) \in S\}$. (Beware: The notation $f^{-1}$ is used in two different ways. Do not confuse the notation introduced here with the notation $f^{-1}(y)$ for the value at $y$ of the inverse of the invertible function $f$. Notice also that $f^{-1}(S)$, the inverse image of the set $S$, makes sense for all functions $f$, not just invertible functions.)

42\. Let $f$ be the function from $\mathbb {R}$ to $\mathbb {R}$ defined by $f(x) = x^2$. Find
a. $f^{-1}(\{1\})$
>Solution
$$
\begin{gathered}
f(x) = x^2 =1 \To x=\pm 1 \\
f^{-1}(\{1\}) = \{\pm 1\}
\end{gathered}
$$

b. $f^{-1}(\{x | 0 <x< 1\})$
>Solution
$$
\begin{gathered}
0 < f(x)=x^2 <1 \To 0<x<1 \text{ or } -1<x<0 \\
f^{-1}(\{x | 0 <x< 1\}) = \{a \in (0, 1) \lor a \in (-1, 0)\}
\end{gathered}
$$

c. $f^{-1}(\{x | x > 4\})$
>Solution
$$
\begin{gathered}
f(x)=x^2 >4 \To x<-2 \text{ or } x>2 \\
f^{-1}(\{x | x > 4\}) = \{a \in (2, \infty) \lor a \in (-\infty, 2)\}
\end{gathered}
$$

44\. Let $f$ be a function from $A$ to $B$. Let $S$ and $T$ be subsets of $B$. Show that
a) $f^{-1}(S \cup T) = f^{-1}(S) \cup f^{-1}(T)$.
>Solution
We need to prove **(a1) $f^{-1}(S \cup T) \subseteq f^{-1}(S) \cup f^{-1}(T)$** and **(a2) $f^{-1}(S) \cup f^{-1}(T) \subseteq f^{-1}(S \cup T)$**.
**a1**. Prove $f^{-1}(S \cup T) \subseteq f^{-1}(S) \cup f^{-1}(T)$
Let $a \in f^{-1}(S \cup T)$, it follows that $f(a) \in S \cup T$
$$
\begin{gathered}
\text{(Or)} \begin{cases}
f(a) \in S \To a \in f^{-1}(S) \\
f(a) \in T \To a \in f^{-1}(T) \\
\end{cases}
\To a \in f^{-1}(T) \cup f^{-1}(S)
\end{gathered}
$$
Therefore **a1** is proved.
**a2**. Prove $f^{-1}(S) \cup f^{-1}(T) \subseteq f^{-1}(S \cup T)$
Let $a \in f^{-1}(S) \cup f^{-1}(T)$, then $a \in f^{-1}(S) \lor a \in f^{-1}(T)$
$$
\begin{gathered}
\text{(Or)} \begin{cases}
a \in f^{-1}(S) \To f(a) \in S\\
a \in f^{-1}(T) \To f(a) \in T
\end{cases}\\
\To f(a) \in S \cup T \To a \in f^{-1}(S \cup T)
\end{gathered}
$$
Therefore **a2** is proved.
According to **(a1)** and **(a2)**, **a** is true.

b) $f^{-1}(S \cap T) = f^{-1}(S) \cap f^{-1}(T)$.
>Solution
We need to prove **(b1) $f^{-1}(S \cap T) \subseteq f^{-1}(S) \cap f^{-1}(T)$** and **(b2) $f^{-1}(S) \cap f^{-1}(T) \subseteq f^{-1}(S \cap T)$**.
**b1**. Prove $f^{-1}(S \cap T) \subseteq f^{-1}(S) \cap f^{-1}(T)$
Let $a \in f^{-1}(S \cap T)$, it follows that $f(a) \in S \cap T$
$$
\begin{gathered}
\text{(And)} \begin{cases}
f(a) \in S \To a \in f^{-1}(S)\\
f(a) \in T \To a \in f^{-1}(T)
\end{cases}\\
\To a \in f^{-1}(S) \cap f^{-1}(T)
\end{gathered}
$$
Therefore **b1** is proved.
**b2**. Prove $f^{-1}(S) \cap f^{-1}(T) \subseteq f^{-1}(S \cap T)$
Let $a \in f^{-1}(S) \cap f^{-1}(T)$, then $a \in f^{-1}(S) \land a \in f^{-1}(T)$
$$
\begin{gathered}
\text{(And)} \begin{cases}
a \in f^{-1}(S) \To f(a) \in S\\
a \in f^{-1}(T) \To f(a) \in T
\end{cases}\\
\To f(a) \in S \cap T \To a \in f^{-1}(S \cap T)
\end{gathered}
$$
Therefore **b2** is proved.
According to **(b1)** and **(b2)**, **b** is true.
