## 01 The foundations: Logic and Proofs

### 1.1 Propositional Logic
**EX**
**HW** pg 34: 31d, 32d, e, 38, 39

* Proposition - A statement that has a truth value.
* Truth table and how to construct one.
* Logical operations - and ($\land$), or ($\lor$), negation ($\neg$).
* Implication (If **assumption** is false, the **conclusion** is always true).
  >$p\to q$, if $p$, then $q$.
  If $p$ (assumption) is false, $p\to q$ (conclusion) is always true.
* Bi-implication (Double implication, if and only if) $p \iff q \equiv (p \to q \land q \to p)$.
* Contrapositive - The contrapositive of $p\to q \text{ is } \lnot q \to \lnot p$.

### 1.3 Propositional Equivalencies
**EX**
**HW** pg 55: 15, 16, 24, 31

* Propositional 1 $\equiv$ propositional 2. These two are logically equivalent. (Use truth table to prove)
* DeMogan's Law:
  >1\. $\neg (p\land q) \equiv \neg p \lor \neg  q$
  2\. $\neg (p\lor q) \equiv \neg p \land \neg  q$
* Tautology - a statement that is always true for every possible case.

### 1.4 Predicates and Quantifiers
**EX** 1, 3, 6, 8, 9, 10, 14, 16
**HW** pg 74: 11, 13, 30, 36, 52

* Propositional function $P(x)$
* Convert a propositional function to a proposition, and evaluate it.
* Quantification
  1\. Universal quantification - $\forall x P(x) \equiv P(x_1) \land P(x_2) \land \cdots P(x_n)$
  2\. Existential quantification - $\exists x P(x) \equiv P(x_1) \lor P(x_2) \lor \cdots P(x_n)$
* Negation of quantified expressions
  1\. $\lnot \forall x P(x) \equiv \exists x \neg P(x)$
  2\. $\lnot \exists x P(x) \equiv \forall x \neg P(x)$

### 1.5 Nested Quantifiers
**EX** 1, 2, 3, 4, 5, table 1
**HW** pg 85: 26, 27 e g h, 31b d, 46

* How to evaluate quantification expressions? (example and counter-example)
* How to distribute negation in quantification expression ? **(hw31, 32)**

### 1.7 Introduction to Proofs
**EX** 3, 8, 10, 12, 13
**HW** pg 112: 13, 26, 27, 31, 32, 42

* Direct proof
  > If $n$ is odd, then $n^3$ is odd.
* Contrapositive
  > If $3n+2$ is even, then $n$ is even.
* Contradiction
  > $\sqrt 2$ is irrational.
* How to prove "if and only if" statement? ($p \iff q \equiv p \to q \land q \to p$).
* How to prove multiple statements are equivalent? ($p \to q, q \to r$, and $r \to p$).

### 1.8 Proof Methods and Strategy
**EX** 1, 2, 3, 6, 13
**HW** pg 129: 14, 19, 29, 30, 36
Can $(irrational)^{irrational}= rational?$
>Proof: Consider $(\sqrt 2)^{\sqrt 2} = x$,
case 1, $x$ is rational, done.
case 2, $x$ is irrational
$$
\begin{aligned}
((\sqrt 2)^{\sqrt 2})^{\sqrt 2} &= x^{\sqrt 2}\\
(\sqrt 2)^2 &= x^{\sqrt 2}\\
2 &= x^{\sqrt 2}
\end{aligned}
$$
2 is rational. Done.
