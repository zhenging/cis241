## 02 Basic Structures: Sets, Functions, Sequences, Sums, and Matrices.
### 2.1 Set
* Element, Empty set ($\emptyset = \{\}$)
  >**Prove** $\emptyset \subseteq A$.
  Proof:
  We need prove $\forall x(x\in \emptyset \to x\in A)$.   Since the assumption $x\in \emptyset$ is false, the conculsiont $x \in A$ is always true. Thus $\forall x(x\in \emptyset \to x\in A)$ is ture.
* Subset ($\subset$ and $\subseteq$) - $A \subseteq B \quad \forall x (x \in A \to x \in B$)
* Powerset - the set of all subsets of a set. The number of subsets of a set with $n$ elements is $2^n$.
* Cartesian Products - $A\times B = \{ (a, b) \mid a\in A \land b\in B\}$

### 2.2 Set Operations
**EX** 1-9, 13, 16, 17
**HW** pg 157: 13, 15, 24, 30, 31, 47, 48

* Union - $A \cup B = \{x\mid x \in A \lor x \in B \}$
* Intersection - $A \cap B = \{x\mid x \in A \land x \in B \}$
* Difference - $A - B = \{x\mid x \in A \land x \notin B \}$
* Complement - $\overline A = \{x\mid x \notin A\}$
* Membership table and how to construct one
* $\bigcup^{n}_{i=1} A_i= A_1 \cup A_2 \cup \cdots A_n$
* $\bigcap^{n}_{i=1} A_i= A_1 \cap A_2 \cap \cdots A_n$

### 2.3 Functions
**EX** 1-23
**HW** pg 175: 40, 42, 44

* Function $f: A\to B$ - an assiagnment of exactly one element of $B$ to each element of $A$.
* Domain and codomain, image and preimage, range
* One-to-one function
	>$\forall a \forall b (f(a)=f(b) \to a=b)$ or equivalently $\forall a \forall b (a\ne b \to f(a) \ne f(b))$
* Image of set $f(s) = \{t \mid \exists s \in S, f(s) = t\}$
* Inverse function
	>1\. If $f$ is a function $f: A\to B$ and is one to one, then $f^{-1}$ exists.
	2\. $f^{-1}(b) = a$ when $f(a) = b$
* Inverse image **(hw 42, 44)**
* Composite Function

### 2.4 Sequences and Summations
**EX** 10, 11
**HW** pg 189: 16cef, 19, 22

* Sequence - $a_1, a_2 \cdots a_n$
* Summation - $\sum^{n}_{i=1} a_i = a_1 + a_2 + \cdots + a_n$

### 2.5 Infinite Sets
**Definition** We call a set $X$ countably infinite if there exists an 1-1 function $f: N\to x$, where $N$ is positive integers.
> $X=\{2, 4, 6, 8 \cdots\}, f(n) = 2n$,
