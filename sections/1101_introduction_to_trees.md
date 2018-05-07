### 11.1 Introduction To Trees

A **tree** is a connected undirected graph with no simple circuits.

>Theorem 1
An undirected graph is a tree if and only if there is a unique simple path between any two of its vertices.

Suppose that $T$ is a rooted tree. If $v$ is a vertex in $T$ other than the root, the **parent** of $v$ is the unique vertiex $u$ such that there is a direct edge from $u$ to $v$. When $u$ is the parent of $v$, $v$ is called a **child** of $u$. Vertices with the same parent are called **siblings**. The **ancestors** of a vertex other that the root are the vertices in the path from the root to this vertex, excluding the vertex itself and including the root (that is, its parent, its parent's parent, and so on, until the root is reached). The **descendants** of a vertex $v$ are those vertices that have $v$ as an ancestors. A vertex of a rooted tree is called a **leaf** if it has no children. Vertices that have children are called **internal vertices**. The root is an internal vertex unless it is the only vertex in the graph, in which case it is a leaf.
If $a$ is a vertex in a tree, the **subtree** with $a$ as its root is the subgraph of the tree consisting of $a$ and its descendants and all edges incident to these descendants.

>Theorem 2
A tree with $n$ vertices has $n-1$ edges. (Proof by induction. The extra vertex must have a degree of 1, otherwise the graph would contain a cycle and would not be a valid tree.)

>Theorem 3
A full m-ary tree with $i$ internal vertices contains $n = mi + 1$ vertices.

#### Homework
p777: 16, 17, 18, **28**

16\. Which complete bipartite graphs $K_{m,n}$, where $m$ and $n$ are positive integers, are trees?
>Solution
When $m=1$ and $n$ is any positive integer, graphs $K_{m,n}$ are trees.

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
