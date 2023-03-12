___

## 2.1 Degree of a vertex
 - **Degree of a vertex** v in a graph G is the number of edges incident with v. Denoted  by $deg_G  \ v$ or $deg \ v$
 - $deg \ v$ is the number of vertices adjacent to v.
 - Two adjacent vertices are called **neighbous** of each other.
 - **Neighborhood** of $v$: Set $N(v)$ neighbors of a vertex. Thus $deg \ v$ = $|N(v)|$.
 - **Isolated vertex**:  A vertex with 0 degree.
 - **End vertex** (or a **leaf**): A vertex with 1 degree.
 - **Minimum degree** of G is the minimum degree among the vertices of G and is denoted $\delta(G)$.
 - **Maximum degree** of G is denoted by $\Delta(G)$
 - If G is a graph of order $n$ and $v$ is any vertex of $G$, then
$$0\leq \delta(G) \leq deg \ v\leq \Delta(G)\leq n-1$$

### Theorems
 - **Theorem 2.1**: *if $G$ is a graph of size $m$, then*
$$\sum_{v\in V(G)}deg\ v = 2m$$
	- Corollary: Every graph has an even number of odd vertices

 - **Theorem 2.4**: *Let $G$ be a graph of order $n$, If*
$$deg \ u + deg\ v \ge n-1$$
	*for every two non adjacent vertices $u$ and $v$ of $G$, then $G$ is connected and diam($G$) $\le$ 2*
	 - **Corollary**: *If $G$ is graph of order $n$ with $\delta(G) \ge (n-1)/2$, then $G$ is connected.*

___

## 2.2 Regular Graphs
 - **Regular graph**: If all vertices of $G$ have asme degree
 - r-**regular** graph: If $deg\ v = r$ for every vertex $v$ of $G$, where $0\le r\le n-1$.

### Theorems:
 - **Theorem 2.6**: *Let $r$ and $n$ be integers with  $0\le r\le n-1$. There exists an r-regular graph of order $n$ iff at least one of $r$ and $n$ is even*.

 - **Theorem 2.7**: *For every graph $G$ and every integer $r\ge\Delta(G)$, then there exists an r-regu;ar graph $H$ containing $G$ as an induced subgraph*.

___

## 2.3 Degree Sequences
 - **Degree sequence**: If the degrees of the vertices of a graph $G$ are listed in a sequence $s$.
 - A finite set of non-negative integers is called **graphical** if it is a degree sequence of some graph.

### Theorem
 - **Theorem 2.10**: *A non-increasing sequence $s$ : $d_1 ,d_2 , ..., d_n\ (n\ge2)$ of non-negative integers, where $d_1\ge1$, is graphical iff the sequence*
$$
s_1 : d_2 -1,d_3 - 1,...,d_{d_1 +1} - 1,d_{d_1 +2},...,d_n
$$
	*is graphical.*

___

