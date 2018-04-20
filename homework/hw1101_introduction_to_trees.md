### Section 11.1 Introduction To Trees
p777: 16, 17, 18, **28**

16\. Which complete bipartite graphs $K_{m,n}$, where $m$ and $n$ are positive integers, are trees?
>Solution
Todo

17\. How many edges does a tree with 10,000 vertices have?
>Solution
A tree with n vertices has (n-1) edged. The tree with 10,000 vertices has 9,999 edges.

18\. How many vertices does a full 5-ary tree with 100 internal vertices have?
>Solution
The number of vertices is $100 \cdot 5 + 1 = 501$.

28\. **A complete m-ary tree** is a full m-ary tree in which every leaf is at the same level. How many vertices and how many leaves does a complete m-ary tree of height h have?
>Solution
A complete m-ary tree of height h has $m^0 + m^1 + \cdot +m^h$ vertices and  $m^h$ leaves.
Proof by induction.
**Basic step** When h = 0, the tree has $m^0 = 1$ vertex and $m^0 = 1$ leaves.
**Hypothesis** Assume that the number of leaves for a complete m-ary tree with height k is $m^k$ and the number of vertices is $m^0 + m^1 + \cdots +m^k$.
**Inductive Step** We need to prove that the number of leaves for a complete m-ary tree with height $k+1$ is $m^{k+1}$ and the number of vertices is $m^0 + m^1 + \cdots +m^k + m^{k+1}$.
Let $T$ be a complete m-ary tree of height $k+1$ and consider a subgraph $T'$ that results from removing all leaves from $T$. $T'$ is a complete m-ary tree of height $k$, so $T'$ has $m^k$ leaves and $m^0 + m^1 + \cdots +m^k$ vertices (_By hypothesis_).
Each leaf of $T'$ has $m$ children in $T$ and each leaves of $T$ is the child of some leaf of $T'$. Therefore, $T$ has $m \cdot m^k = m^{k+1}$ leaves and $m^0 + m^1 + \cdots +m^k + m^{k+1}$ vertices.
