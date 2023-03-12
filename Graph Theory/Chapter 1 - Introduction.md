## 1.1 Graphs and Graph Models

### Definitions:
  - **Graph**: $G(V,E)$ An ordered pair of two sets vertices $(V)$ and edges $(E)$
  - $V$: Finite non empty set of objects
  - $E$: Two element subsets of $V$
  - **Order**: Number of vertices in $G$
  - **Size**: Number of edges in $G$
  - **Trivial graph**: A graph with exactly one vertex
  - **Non-Trivial graph**: A graph with at least 2 vertex
  - **Labeled graph**: A graph with vertices labeled
  - **Unlabeled graph**: A graph without vertex labels

### Observations:
 - Two graphs G and H are **equal** if V(G) = V(H) and E(G) = E(H)

## 1.2 Connected Graphs

### **Definitions**:
 - **Neighbors**: Two vertices connected by an edge.
 - **Adjacent edge**: Two edges incident to a common vertex.
 - **Subgraph**: Denoted as $H\subseteq G$, if 
 - **Proper subgraph**: $H \subset G$ 
 - **Spanning subgraph**:
 - **Induced subgraph**:
 - **Edge induced subgraph**: $X \subset E(G)$ and $V$ contains all vertives of $G$ that are incident to at least one edge in $X$.
 - **Walk**: Sequence of vertices that are neighbour in $G$.
 - **Trail**: A walk with no edge traversed more than once.
 - **Path**: A walk in which no vertices are repeated.
 - **Circuit**: A trial where the starting and ending vertices are same.
 - **Cycle**: A circuit without no vertices repeated.
 - $k$-**cycle**: A cycle of length $k$.
 - **Triangle**: A 3-cycle graph.
 - **Odd cycle**: A cycle of odd length.
 - **Even cycle**: A cycle of even lenght.
 - **Component**: A connected subgraph of $G$ that is not proper subgraph of any other connected subgraph of $G$.
 - **Distance**: The smallest length of any $u-v$ path in $G$.
 

### Observations:
 - Any proper subgraph of a graph $G$ can be obtaibed by removing vertices and edges from $G$
 - If X is a set of edges of $G$, then $G-X$ is the spanning subgraph of $G$ with $E(G-X)=E(G)-X$
 - If $G$ contains $u-v$ path, then $u$ and $v$ are said to be **connected** and $u$ **is connected to** $v$.
 - Every graph is the union of its components

### Theorems:
 1. *If a graph $G$ contains a $u-v$ walk of length $l$, then $G$ contains a $u-l$ path of length at most $l$.
 2. *Let $R$ be the relation defined on the vertex set of a graph $G$ by $u\ R\ v$, where $u, v ∈ V(G)$, if $u$ is connected to $v$, that is, if G contains a $u − v$ path. Then $R$ is an equivalence relation.*
 3. *Let $G$ be a graph of order 3 or more. If $G$ contains two distinct vertices $u$ and $v$ such that $G − u$ and $G − v$ are connected, then $G$ itself is connected.*
 4. *If $G$ is a connected graph of order 3 or more, then $G$ contains two distinct vertices $u$ and $v$ such that $G-u$ and $G-v$ are connected.*
 5. Let $G$ be a graph of order 3 or more. Then $G$ is connected iff $G$ contains two distinct vertices $u$ and $v$ such that $G-u$ and $G-v$ are connected.

## 1.4 Multigraphs and Digraphs

### Definitions:
 - **Multigraph**: A finite nonempty set $V$ of vertices and a set $E$ of edges, where every two vertices are joined by a finite number of edges(possibily zero).
 - **Parallel edges**: Two or more edges join same pair of (distinct) edges.
 - **Loop**: Edge joining a vertex to itself.
 - **Pseudograph**: A graph with parallel edges and loops.
 - **Digraph** (directed graph): A finite nonempty set of $V$ of objects  
