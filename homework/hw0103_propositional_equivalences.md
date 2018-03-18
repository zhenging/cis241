### Section 1.3 Propositional Equivalences
pg55: 15, **16, 31, 34**

15\. Determine whether $(\neg q \land (p \to  q)) \to \neg p$ is a tautology.
>Solution
| $p$ | $q$ | $p \to q$ | $\neg q \land (p \to  q)$ | $(\neg q \land (p \to  q)) \to \neg p$ |
|:-:|:-:|:-:|:-:|:-:|
| T | T | T | F | T |
| T | F | F | F | T |
| F | T | T | F | T |
| F | F | T | T | T |
Therefore, $(\neg q \land (p \to  q)) \to \neg p$ is a tautology.

16\. Show that $p \bi q$ and $(p \land q) \lor (\neg p \land \neg q)$ are logically equivalent.
>Solution
| $p$ | $q$ | $p \bi q$ | $p \land q$ | $\neg p \land \neg q$ | $(p \land q) \lor (\neg p \land \neg q)$ |
|:-:|:-:|:-:|:-:|:-:|:-:|
| T | T | T | T | F | T |
| T | F | F | F | F | F |
| F | T | F | F | F | F |
| F | F | T | F | T | T |
Therefore, $p \bi q$ and $(p \land q) \lor (\neg p \land \neg q)$ are logically equivalent.

31\. Show that $(p \to q) \to r$ and $p \to (q \to r)$ are not logically equivalent.
>Solution
| $p$ | $q$ | $r$ | $p \to q$ | $(p \to q) \to r$ | $q \to r$ | $p \to (q \to r)$ |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| T | T | T | T | T | T | T |
| T | T | F | T | F | F | F |
| T | F | T | F | T | T | T |
| T | F | F | F | T | T | T |
| F | T | T | T | T | T | T |
| F | T | F | T | F | F | T |
| F | F | T | T | T | T | T |
| F | F | F | T | F | T | T |
Therefore $(p \to q) \to r$ and $p \to (q \to r)$ are not logically equivalent.

The **dual** of a compound proposition that contains only the logical operators $\lor, \land$ and $\lnot$ is the compound proposition obtained by replacing each $\lor$ by $\land$, each $\land$ by $\lor$, each $T$ by $F$, and each $F$ by $T$. The dual of $s$ is denoted by $s^{*}$.
34\. Find the dual of each of these compound propositions.
a) $p \lor \lnot q$
b) $p \land (q \lor (r \land T))$
c) $(p \land \lnot q) \lor (q \land F)$
>Solution
a. $(p \lor \lnot q)^* = p \land \lnot q$
b) ${\lb p \land (q \lor (r \land T)) \rb}^* = p \lor (q \land (r \lor F))$
c) ${\lb (p \land \lnot q) \lor (q \land F) \rb}^* = (p \lor \lnot q) \land (q \lor T)$
