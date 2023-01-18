## Description

<div><p>A forestation is an act of planting a bunch of trees to grow a forest, usually to replace a forest that had been cut down. Strangely enough, graph theorists have another idea on how to make a forest, i.e. by cutting down a tree!</p><p>A tree is a graph of $N$ nodes connected by $N - 1$ edges. Let $u$ be a node in a tree $U$ which degree is at least $2$ (i.e. directly connected to at least $2$ other nodes in $U$). If we remove $u$ from $U$, then we will get two or more disconnected (smaller) trees, or also known as forest by graph theorists. In this problem, we are going to investigate a special forestation of a tree done by graph theorists.</p><p>Let $V(S)$ be the set of nodes in a tree $S$ and $V(T)$ be the set of nodes in a tree $T$. Tree $S$ and tree $T$ are <span class="tex-font-style-bf">identical</span> if there exists a bijection $f : V(S) \rightarrow V(T)$ such that for all pairs of nodes $(s_i, s_j)$ in $V(S)$, $s_i$ and $s_j$ is connected by an edge in $S$ if and only if node $f(s_i)$ and $f(s_j)$ is connected by an edge in $T$. Note that $f(s) = t$ implies node $s$ in $S$ corresponds to node $t$ in $T$.</p><p>We call a node $u$ in a tree $U$ as a good cutting point if and only if the removal of $u$ from $U$ causes two or more disconnected trees, and all those disconnected trees are pairwise identical.</p><p>Given a tree $U$, your task is to determine whether there exists a good cutting point in $U$. If there is such a node, then you should output the maximum number of disconnected trees that can be obtained by removing exactly one good cutting point.</p><p>For example, consider the following tree of $13$ nodes.</p><p><img class="tex-graphics" src="file://EvYXHdIO.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There is exactly one good cutting point in this tree, i.e. node $4$. Observe that by removing node $4$, we will get three identical trees (in this case, line graphs), i.e. $\{5, 1, 7, 13\}$, $\{8, 2, 11, 6\}$, and $\{3, 12, 9, 10\}$, which are denoted by $A$, $B$, and $C$ respectively in the figure. </p><ul> <li> The bijection function between $A$ and $B$: $f(5) = 8$, $f(1) = 2$, $f(7) = 11$, and $f(13) = 6$. </li><li> The bijection function between $A$ and $C$: $f(5) = 3$, $f(1) = 12$, $f(7) = 9$, and $f(13) = 10$. </li><li> The bijection function between $B$ and $C$: $f(8) = 3$, $f(2) = 12$, $f(11) = 9$, and $f(6) = 10$. </li></ul> Of course, there exists other bijection functions for those trees.</div><div class="input-specification"><p>Input begins with a line containting an integer: $N$ ($3 \le N \le 4000$) representing the number of nodes in the given tree. The next $N - 1$ lines each contains two integers: $a_i$ $b_i$ ($1 \le a_i &lt; b_i \le N$) representing an edge $(a_i,b_i)$ in the given tree. It is guaranteed that any two nodes in the given tree are connected to each other by a sequence of edges.</p></div><div class="output-specification"><p>Output in a line an integer representing the maximum number of disconnected trees that can be obtained by removing exactly one good cutting point, or output <span class="tex-font-style-tt">-1</span> if there is no such good cutting point.</p></div>

## Input

<p>Input begins with a line containting an integer: $N$ ($3 \le N \le 4000$) representing the number of nodes in the given tree. The next $N - 1$ lines each contains two integers: $a_i$ $b_i$ ($1 \le a_i &lt; b_i \le N$) representing an edge $(a_i,b_i)$ in the given tree. It is guaranteed that any two nodes in the given tree are connected to each other by a sequence of edges.</p>

## Output

<p>Output in a line an integer representing the maximum number of disconnected trees that can be obtained by removing exactly one good cutting point, or output <span class="tex-font-style-tt">-1</span> if there is no such good cutting point.</p>





```input1
13
1 5
1 7
2 4
2 8
2 11
3 12
4 7
4 12
6 11
7 13
9 10
9 12
```




```input2
6
1 2
1 3
2 4
3 5
3 6
```




```output1
3
```




```output2
-1
```



## Note

<p><span class="tex-font-style-it">Explanation for the sample input/output #1</span></p><p>This is the example from the problem description.</p>
