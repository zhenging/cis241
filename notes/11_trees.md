## Chapter 11 Trees

### 11.1 Introduction to Trees

A **tree** is a connected undirected graph with no simple circuits.

>Theorem 1
An undirected graph is a tree if and only if there is a unique simple path between any two of its vertices.

Suppose that $T$ is a rooted tree. If $v$ is a vertex in $T$ other than the root, the **parent** of $v$ is the unique vertiex $u$ such that there is a direct edge from $u$ to $v$. When $u$ is the parent of $v$, $v$ is called a **child** of $u$. Vertices with the same parent are called **siblings**. The **ancestors** of a vertex other that the root are the vertices in the path from the root to this vertex, excluding the vertex itself and including the root (that is, its parent, its parent's parent, and so on, until the root is reached). The **descendants** of a vertex $v$ are those vertices that have $v$ as an ancestors. A vertex of a rooted tree is called a **leaf** if it has no children. Vertices that have children are called **internal vertices**. The root is an internal vertex unless it is the only vertex in the graph, in which case it is a leaf.
If $a$ is a vertex in a tree, the **subtree** with $a$ as its root is the subgraph of the tree consisting of $a$ and its descendants and all edges incident to these descendants.

>Theorem 2
A tree with $n$ vertices has $n-1$ edges. (Proof by induction. The extra vertex must have a degree of 1, otherwise the graph would contain a cycle and would not be a valid tree.)

>Theorem 3
A full m-ary tree with $i$ internal vertices contains $n = mi + 1$ vertices.

### 11.2 Applications of Trees
Ex:-
HW:-

### 11.3 Tree Traverse

#### Preorder
Let $T$ be an ordered rooted tree with root $r$. It $T$ consists only of $r$, then $r$ is the _preorder trasversal_ of $T$. Otherwise, suppose that $T_1, T_2, \cdots T_n$ are the subtrees at $r$ from left to right in $T$. The _preorder trasveral_ begins by visiting $T_1$. It continues by traversing $T_1$ in preorder, then $T_2$ in preorder, and so on, until $T_n$ is traversed in preorder.
> Root => Left => Right

![Graph](../assets/1103_preorder_traversal.png)

##### Algorithem 1 Preorder traversal
```
procedure preorder(T: ordered rooted tree)
r := root of T
list r
for each child c of r from left to right
  T(c) := subtree with c as its root
  procedure(T(c))
```

#### Inorder
Let $T$ be an ordered rooted tree with root $r$. It $T$ consists only of $r$, then $r$ is the _inorder trasversal_ of $T$. Otherwise, suppose that $T_1, T_2, \cdots T_n$ are the subtrees at $r$ from left to right in $T$. The _inorder trasveral_ begins by traversing $T_1$ in inorder, then visiting $r$. It continues by traversing $T_2$ in inorder, then $T_3$ in inorder, ..., and finally $T_n$ in order.
> Left => Root => Right

![Graph](../assets/1103_inorder_traversal.png)

>Example
![Graph](../assets/1103_inorder_ex_03.png)
>Solution
```
b,                        a, c,    d
e,                b, f,   a, c,    g,       d, h, i
j, e, k,          b, f,   a, c,    l, g, m, d, h, i
j, e, n, k, o, p, b, f,   a, c,    l, g, m, d, h, i
```

##### Algorithem 2 Inorder traversal
```
procedure inorder(T: ordered rooted tree)
r := root of T
if r is a leaf then list r
else
  l := first child of r from left to right
  T(l) := subtree with l as its root
  inorder(T(l))
  list r
  for each child c of r except l from left to right
    T(c) := subtree with c as its root
    inorder(T(c))
```

#### Postorder
Let $T$ be an ordered rooted tree with root $r$. It $T$ consists only of $r$, then $r$ is the _postorder trasversal_ of $T$. Otherwise, suppose that $T_1, T_2, \cdots T_n$ are the subtrees at $r$ from left to right in $T$. The _postorder trasveral_ begins by traversing $T_1$ in postorder, then $T_2$ in postorder, ... then $T_n$ in postorder, and ends by visiting $r$.
> Left => Right => Root

![Graph](../assets/1103_postorder_traversal.png)

>Example
![Graph](../assets/1103_postorder_ex_04.png)
>Solution
```
b,       c, d,          a
e, f, b, c, g, h, i, d, a
j, k, e, f, b, c, l, m, g, h, i, d, a
j, n, o, p, k, e, f, b, c, l, m, g, h, i, d, a
```

##### Algorithem 3 Postorder traversal
```
procedure postorder(T: ordered rooted tree)
r := root of T
for each child c of r from left to right
  T(c) := subtree with c as its root
  postorder(T(c))
list r
```
