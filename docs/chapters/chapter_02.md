# Basic Graph Terminologies

## Exercises

### 1.
Show that every regular graph with an odd degree has an even number of vertices.

**Answer:** $k$-regular graph of vertices $n$, where $k$ is odd.  
Degree sum $= 2m$, where $m$ is number of edges.  
$2m = k \times n$  
$k$ is odd, $2m$ is even.  
$\therefore n$ must be even.  

### 2.
Construct the complement of $K_{3,3}, W_{5}$, and $C_{5}$.

**Answer:** Complement of $K_{3,3}$ Figure [2.2.1]

<figure>
<embed src="../../figures/2_2_k33.svg" id="fig:2_2_k33" style="width:100.0%" />
<figcaption aria-hidden="true"><span
class="arithmatex">\(K_{3,3}\)</span></figcaption>
</figure>

<figure>
<embed src="../../figures/2_2_k33_c.svg" id="fig:2_2_k33_c" style="width:100.0%" />
<figcaption aria-hidden="true"><span
class="arithmatex">\(\overline{K}_{3,3}\)</span></figcaption>
</figure>

[2.2.1]: #fig:2_2_k33

Complement of $W_{5}$ Figure [2.2.2]

<figure>
<embed src="../../figures/2_2_w5.svg" id="fig:2_2_w5" style="width:100.0%" />
<figcaption aria-hidden="true"><span
class="arithmatex">\(W_{5}\)</span></figcaption>
</figure>

<figure>
<embed src="../../figures/2_2_w5_c.svg" id="fig:2_2_w5_c" style="width:100.0%" />
<figcaption aria-hidden="true"><span
class="arithmatex">\(\overline{W}_{5}\)</span></figcaption>
</figure>

[2.2.2]: #fig:2_2_w

Complement of $C_{5}$ Figure [2.2.3]

<figure>
<embed src="../../figures/2_2_c5.svg" id="fig:2_2_c5" style="width:100.0%" />
<figcaption aria-hidden="true"><span
class="arithmatex">\(C_{5}\)</span></figcaption>
</figure>

<figure>
<embed src="../../figures/2_2_c5_c.svg" id="fig:2_2_c5_c" style="width:100.0%" />
<figcaption aria-hidden="true"><span
class="arithmatex">\(\overline{C}_{5}\)</span></figcaption>
</figure>

[2.2.3]: #fig:2_2_c

### 3.
Can you construct a disconnected graph $G$ of two or more vertices such that $\overline{G}$ is also disconnected. Give a proof supporting your answer.

**Answer:** No.  
Let us prove given a graph $G$ of two or more vertices, either $G$ or $\overline{G}$ is connected.  
$G$ is disconnected. We want to show that $\overline{G}$ is connected.  
Suppose $v$ and $w$ are vertices. If $(v, w)$ is not an edge in $G$, then it is an edge in $\overline{G}$, and so we have a path from $v$ to $w$ in $\overline{G}$. On the other hand, if $(v, w)$ is an edge in $G$, then this means $v$ and $w$ are in the same component of $G$. Since $G$ is disconnected, we can find a vertex $u$ in a different component, so that neither $(v, u)$ nor $(u, w)$ are edges of $G$. Then $(v, u, w)$ is a path from $v$ to $w$ in $\overline{G}$.  
This shows that any two vertices in $\overline{G}$ have a path (in fact a path of length one or two) between them in $\overline{G}$, so $\overline{G}$ is connected. \[[5]\]  
Example Figure [2.3.1]:

<figure>
<embed src="../../figures/2_3_disc_g.svg" id="fig:2_3_disc_g" style="width:100.0%" />
<figcaption aria-hidden="true">Complement of disconnected graph is
connected example</figcaption>
</figure>

[2.3.1]: #fig:2_3_disc_g
[5]: ../../references/#ref5

### 4.
Give two examples of self-complementary graphs.

**Answer:** Self complementary graphs example: $C_5$, $P_4$ Figure [2.4.1]

<figure>
<embed src="../../figures/2_4_self_compl.svg" id="fig:2_4_self_compl" style="width:100.0%" />
<figcaption aria-hidden="true">Self complementary graphs <span
class="arithmatex">\(C_5, P_4\)</span></figcaption>
</figure>

[2.4.1]: #fig:2_4_self_compl

### 5.
What is the necessary and sufficient condition for $K_{m,n}$ to be a regular graph?

**Answer:** In the complete bipartite graph $K_{m,n}$, the vertices have degree $m$ or degree $n$ (and both of these degrees are reached). Thus, to be regular, a sufficient and necessary condition is $n=m$. \[[6]\]

[6]: ../../references/#ref6

### 6.
Is there a simple graph of $n$ vertices such that the vertices all have distinct degrees? Give a proof supporting your answer.

**Answer:** If $n=1$, yes, trivial.  
For $n>1$. Suppose such a graph exists. Each vertex in the graph can have a degree from $0$ to $n-1$ (simple graphs do not forbid a degree-$0$ vertex, \emph{connected} graphs do). Since this range spans $n$ values in total and each vertex degree is different, the degrees are distributed one-per-vertex. In particular, there must exist a vertex with degree $n-1$ and one with degree $0$.  
Now the degree-$n-1$ vertex is connected to all other vertices because the graph is simple, \emph{including} the degree-$0$ vertex. But the latter is not connected to any vertex, which is a contradiction. Therefore two vertices in the graph must have the same degree.
\[[3]\] \[[7]\]

[3]: ../../references/#ref3
[7]: ../../references/#ref7

### 7.
Draw the graph $G = (V, E)$ with vertex set $V = \{a, b, c, d, e, f, g, h\}$ and edge set $\{(a, b), (a, e), (b, c), (b, d), (c, d), (c, g), (d, e)(e, f ), ( f, g), ( f, h), (g, h)\}$. Draw $G - (d, e)$. Draw the subgraph of $G$ induced by $\{c, d, e, f\}$. Contract the edge $(d, e)$ from $G$.

**Answer:** Graph drawings Figure [2.7.1]

<figure>
<embed src="../../figures/2_7_G.svg" id="fig:2_7_G" style="width:100.0%" />
<figcaption aria-hidden="true"><span class="arithmatex">\(G\)</span></figcaption>
</figure>

<figure>
<embed src="../../figures/2_7_G-d_e.svg" id="fig:2_7_G-d_e" style="width:100.0%" />
<figcaption aria-hidden="true"><span class="arithmatex">\(G-(d,e)\)</span></figcaption>
</figure>

<figure>
<embed src="../../figures/2_7_c_d_e_f.svg" id="fig:2_7_c_d_e_f" style="width:100.0%" />
<figcaption aria-hidden="true"><span class="arithmatex">\(G\)</span> induced by <span class="arithmatex">\(\{c, d, e, f\}\)</span></figcaption>
</figure>

<figure>
<embed src="../../figures/2_7_G-d_e_contr.svg" id="fig:2_7_G-d_e_contr" style="width:100.0%" />
<figcaption aria-hidden="true"><span class="arithmatex">\((d, e)\)</span> edge contracted from <span class="arithmatex">\(G\)</span></figcaption>
</figure>

  [2.7.1]: #fig:2_7_G

### 8.
Show that two graphs are isomorphic if and only if their complements are isomorphic.

**Answer:** Let graph $G$ be isomorphic to $H$, and let $\overline G$, $\overline H$ denote their complements.  
Since $G$ is isomorphic to $H$, then there exists a bijection $f: V(G) \to V(H)$, such that $(u, v) \in E(G)$ if and only if $(f(u), f(v)) \in E(H)$.  
Equivalently, there exists a bijection $f: V(G) \to V(H)$, such that $(u, v) \notin E(G)$ if and only if $(f(u), f(v)) \notin E(H)$.  
Since the vertex set of $G$ and $\overline G$ are the same, therefore $f$ is a bijection from $V(\overline G)$ to $V(\overline H)$. Then suppose $(u, v) \notin E(G)$, by definition of a complement, $(u, v) \in E(\overline G)$. Likewise, if $(f(u), f(v)) \notin E(H)$, then $(f(u), f(v)) \in E(\overline H)$.  
Hence $\overline G$ and $\overline H$ are isomorphic. \[[4]\]

[4]: ../../references/#ref4
