### Section 1.1 Propositional Logic
pg34: 31d, 32de, **38, 39**

31\. Construct a truth table for each of these compound propositions.
d). $(p \lor q) \to (p \land q)$
>Solution
| $p$ | $q$ | $p \lor q$ | $p \land q$ | $(p \lor q) \to (p \land q)$ |
|:-:|:-:|:-:|:-:|:-:|
| T | T | T | T | T |
| T | F | T | F | F |
| F | T | T | F | F |
| F | F | F | F | T |

32\. Construct a truth table for each of these compound propositions.
d. $(p \land q) \to (p \lor q)$
>Solution
| $p$ | $q$ | $p \land q$ | $p \lor q$ | $(p \land q) \to (p \lor q)$ |
|:-:|:-:|:-:|:-:|:-:|
| T | T | T | T | T |
| T | F | F | T | T |
| F | T | F | T | T |
| F | F | F | F | T |

e. $(q \to \neg p) \bi (p \bi q)$
>Solution
| $p$ | $q$ | $q \to \neg p$ | $p \bi q$ | $(q \to \neg p) \bi (p \bi q)$ |
|:-:|:-:|:-:|:-:|:-:|
| T | T | F | T | F |
| T | F | T | F | F |
| F | T | T | F | F |
| F | F | T | T | T |


38\. Construct a truth table for $((p \to q) \to r) \to s$.
>Solution
| $p$ | $q$ | $r$ | $s$ | $p \to q$ | $(p \to q) \to r$ | $((p \to q) \to r) \to s$ |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| T | T | T | T | T | T | T |
| T | T | T | F | T | T | F |
| T | T | F | T | T | F | T |
| T | T | F | F | T | F | T |
| T | F | T | T | F | T | T |
| T | F | T | F | F | T | F |
| T | F | F | T | F | T | T |
| T | F | F | F | F | T | F |
| F | T | T | T | T | T | T |
| F | T | T | F | T | T | F |
| F | T | F | T | T | F | T |
| F | T | F | F | T | F | T |
| F | F | T | T | T | T | T |
| F | F | T | F | T | T | F |
| F | F | F | T | F | T | T |
| F | F | F | F | F | T | F |


39\. Construct a truth table for $(p \bi q) \bi (r \bi s)$.
>Solution
| $p$ | $q$ | $r$ | $s$ | $p \bi q$ | $r \bi s$ | $(p \bi q) \bi (r \bi s)$ |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| T | T | T | T | T | T | T |
| T | T | T | F | T | F | F |
| T | T | F | T | T | F | F |
| T | T | F | F | T | T | T |
| T | F | T | T | F | T | F |
| T | F | T | F | F | F | T |
| T | F | F | T | F | F | T |
| T | F | F | F | F | T | F |
| F | T | T | T | F | T | F |
| F | T | T | F | F | F | T |
| F | T | F | T | F | F | T |
| F | T | F | F | F | T | F |
| F | F | T | T | T | T | T |
| F | F | T | F | T | F | F |
| F | F | F | T | T | F | F |
| F | F | F | F | T | T | T |
