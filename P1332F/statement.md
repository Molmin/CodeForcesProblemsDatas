## Description

<div><p>Eric is the teacher of graph theory class. Today, Eric teaches independent set and edge-induced subgraph.</p><p>Given a graph $G=(V,E)$, an <span class="tex-font-style-it">independent set</span> is a subset of vertices $V' \subset V$ such that for every pair $u,v \in V'$, $(u,v) \not \in E$ (i.e. no edge in $E$ connects two vertices from $V'$).</p><p>An <span class="tex-font-style-it">edge-induced subgraph</span> consists of a subset of edges $E' \subset E$ and all the vertices in the original graph that are incident on at least one edge in the subgraph.</p><p>Given $E' \subset E$, denote $G[E']$ the edge-induced subgraph such that $E'$ is the edge set of the subgraph. Here is an illustration of those definitions:</p><center> <img class="tex-graphics" src="file://mTWjz8tf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In order to help his students get familiar with those definitions, he leaves the following problem as an exercise:</p><p>Given a tree $G=(V,E)$, calculate the sum of $w(H)$ over all except null edge-induced subgraph $H$ of $G$, where $w(H)$ is the number of independent sets in $H$. Formally, calculate $\sum \limits_{\emptyset \not= E' \subset E} w(G[E'])$.</p><p>Show Eric that you are smarter than his students by providing the correct answer as quickly as possible. Note that the answer might be large, you should output the answer modulo $998,244,353$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 3 \cdot 10^5$), representing the number of vertices of the graph $G$.</p><p>Each of the following $n-1$ lines contains two integers $u$ and $v$ ($1 \le u,v \le n$, $u \not= v$), describing edges of the given tree.</p><p>It is guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>Output one integer, representing the desired value modulo $998,244,353$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 3 \cdot 10^5$), representing the number of vertices of the graph $G$.</p><p>Each of the following $n-1$ lines contains two integers $u$ and $v$ ($1 \le u,v \le n$, $u \not= v$), describing edges of the given tree.</p><p>It is guaranteed that the given edges form a tree.</p>

## Output

<p>Output one integer, representing the desired value modulo $998,244,353$.</p>





```input1
2
2 1
```




```input2
3
1 2
3 2
```




```output1
3
```




```output2
11
```



## Note

<p>For the second example, all independent sets are listed below.</p><center> <img class="tex-graphics" src="file://qrHWWxjl.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
