### Section 2.2 Set Operations
pg157: 13, 15, 24, 30, 31, 47, 48

13\.  Prove the second absorption law from Table 1 by showing that if $A$ and $B$ are sets, then $A \cap (A \cup B) = A$.
>Solution
| $A$ | $B$ | $A \cup B$ | $A \cap (A \cup B)$ |
|:-:|:-:|:-:|:-:|
| 1 | 1 | 1 | 1 |
| 1 | 0 | 1 | 1 |
| 0 | 1 | 1 | 0 |
| 0 | 0 | 0 | 0 |

15\. Prove the second De Morgan law in Table 1 by showing that if $A$ and $B$ are sets, then $\overline{A \cup B} = \overline A \cap \overline B$
a) by showing each side is a subset of the other side.
>Solution
$$
\begin{aligned}
\overline{A \cup B} &= \{x \mid x \notin {A \cup B} \} \\
&= \{x \mid \neg (x \in A \cup B) \} \\
&= \{x \mid \neg(x \in A) \land \neg(x \in B) \} \\
&= \{x \mid x \notin A \land x \notin B \} \\
&= \{x \mid x \in \overline A \land x \in \overline B \} \\
&= \{x \mid x \in \overline A \cap \overline B \} \\
&= \overline A \cap \overline B
\end{aligned}
$$

b) using a membership table.
>Solution
| $A$ | $B$ | $A \cup B$ | $\overline {A \cup B}$ | $\overline A$ | $\overline B$ | $\overline A \cap \overline B$ |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| 1 | 1 | 1 | 0 | 0 | 0 | 0 |
| 1 | 0 | 1 | 0 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 | 0 | 0 |
| 0 | 0 | 0 | 1 | 1 | 1 | 1 |

24\. Let A, B, and C be sets. Show that $(A - B) - C = (A - C) - (B - C)$.
>Solution
$$
\begin{aligned}
(A - C) - (B - C)&= (A \cap \overline C) - (B \cap \overline C)\\
&= (A \cap \overline C) \cap (\overline {B \cap \overline C})\\
&= (A \cap \overline C) \cap (\overline B \cup C)\\
&= [(A \cap \overline C) \cap \overline B] \cup [(A \cap \overline C) \cap C]\\
&= [(A \cap \overline B) \cap \overline C) \cup [A \cap (\overline C \cap C)]\\
&= [(A \cap \overline B) \cap \overline C) \cup (A \cap \emptyset)\\
&= [(A \cap \overline B) \cap \overline C) \cup \emptyset\\
&= (A \cap \overline B) \cap \overline C \\
&= (A - B) - C
\end{aligned}
$$

30\. Can you conclude that $A = B$ if $A$, $B$, and $C$ are sets such that
a) $A \cup C = B \cup C$?
b) $A \cap C = B \cap C$?
c) $A \cup C = B \cup C$ and $A \cap C = B \cap C$?
>Solution
a. No. Consider $A = \{1\}, B = \{2\}, C = \{1, 2, 3\}$, $A \cup C = B \cup C$, but $A \ne B$.
b. No. Consider $A = \{1\}, B = \{2\}, C = \emptyset$.
c. True. To prove two sets $A, B$ are equal, we need to prove $A \subseteq B$, and $B \subseteq A$.
1\. Show $A \subseteq B$. Let $x \in A$,
$$
\begin{aligned}
& \text{case 1: } \\
& (1) \quad x \in A \land x \in C \To x \in A \cap C\\
& (2) \quad A \cap C = B \cap C \To x \in B \cap C\\
& (3) \quad \To x \in B\\
& \text{case 2: } \\
& (1) \quad x \notin C \To x \in A\cup C\\
& (2) \quad A \cup C = B \cup C \To x \in B \cup C\\
& (3) \quad x \notin C \To x \in B
\end{aligned}
$$
2\. Show $B \subseteq A$. Let $y \in B$,
$$
\begin{aligned}
&\text{case 1: } \\
&(1) \quad y \in C \To y \in B \cap C\\
&(2) \quad B \cap C = A \cap C \To y \in A \cap C\\
&(3) \quad y \in C \To y \in A\\
&\text{case 2: } \\
&(1) \quad y \notin C \To y \in B\cup C\\
&(2) \quad B \cup C = A \cup C \To y \in A \cup C\\
&(3) \quad y \notin C \To y \in A
\end{aligned}
$$

31\. Let $A$ and $B$ be subsets of a universal set $U$. Show that $A \subseteq B$ if and only if $\overline B \subseteq \overline A$.
>Solution
$$
\begin{aligned}
A \subseteq B &\equiv \{x \mid x \in A \to x \in B\}\\
&\equiv \{x \mid x \notin B \to x \notin A\}\\
&\equiv \{x \mid x \in {\overline B} \to x \in {\overline A}\}\\
&\equiv \overline B \subseteq \overline A
\end{aligned}
$$

47\. Let $A_i = \{1, 2, 3, \cdots,i\}$ for $i = 1, 2, 3, \cdots$ Find
a) $\bigcup\limits_{i=1}^n A_i$ &emsp; b) $\bigcap\limits_{i=1}^n A_i$
>Solution
a. $\bigcup\limits_{i=1}^n A_i = \{1, 2, 3, \cdots, n\}$
b. $\bigcap\limits_{i=1}^n A_i = \{1\}$

48\.  Let $A_i = {\cdots, -2, -1, 0, 1, \cdots ,i}$. Find
a) $\bigcup\limits_{i=1}^n A_i$ &emsp; b) $\bigcap\limits_{i=1}^n A_i$
>Solution
a. $\bigcup\limits_{i=1}^n A_i = \{\cdots, -2, -1, 0, 1, \cdots ,n\}$
b. $\bigcap\limits_{i=1}^n A_i = \{\cdots, -2, -1, 0, 1\}$
