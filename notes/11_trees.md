## Chapter 11 Trees

### 11.1 Introduction to Trees

>Definition
A tree is a connected undirected graph with no simple circuits.

Theorem 1
An undirected graph is a tree if and only if there is a unique simple path between any two of its vertices.

Suppose that $T$ is a rooted tree. If $v$ is a vertex in $T$ other than the root, the **parent** of $v$ is the unique vertiex $u$ such that there is a direct edge from $u$ to $v$. When $u$ is the parent of $v$, $v$ is called a **child** of $u$. Vertices with the same parent are called **siblings**. The **ancestors** of a vertex other that the root are the vertices in the path from the root to this vertex, excluding the vertex itself and including the root (that is, its parent, its parent's parent, and so on, until the root is reached). The **descendants** of a vertex $v$ are those vertices that have $v$ as an ancestors. A vertex of a rooted tree is called a **leaf** if it has no children. Vertices that have children are called **internal vertices**. The root is an internal vertex unless it is the only vertex in the graph, in which case it is a leaf.
If $a$ is a vertex in a tree, the **subtree** with $a$ as its root is the subgraph of the tree consisting of $a$ and its descendants and all edges incident to these descendants.


Theorem 2
A tree with n vertices has n-1 edges. (Proof by induction. The extra vertex must have a degree of 1, otherwise the graph would contain a cycle and would not be a valid tree.)

Theorem 3
A full m-ary tree with $i$ internal vertices contains $n = mi + 1$ vertices.


### 11.2 Applications of Trees
Ex:
**HW**

### 11.3 Tree Traverse
Ex:
**HW** 8, 9
