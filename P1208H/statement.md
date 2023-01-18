## Description

<div><p>You are given a tree of $n$ nodes. The tree is rooted at node $1$, which is not considered as a leaf regardless of its degree.</p><p>Each leaf of the tree has one of the two colors: <span class="tex-font-style-it">red</span> or <span class="tex-font-style-it">blue</span>. Leaf node $v$ initially has color $s_{v}$.</p><p>The color of each of the internal nodes (including the root) is determined as follows. </p><ul> <li> Let $b$ be the number of <span class="tex-font-style-it">blue</span> immediate children, and $r$ be the number of <span class="tex-font-style-it">red</span> immediate children of a given vertex. </li><li> Then the color of this vertex is <span class="tex-font-style-it">blue</span> if and only if $b - r \ge k$, otherwise <span class="tex-font-style-it">red</span>. </li></ul><p>Integer $k$ is a parameter that is same for all the nodes.</p><p>You need to handle the following types of queries: </p><ul> <li> <span class="tex-font-style-tt">1 v</span>: print the color of node $v$; </li><li> <span class="tex-font-style-tt">2 v c</span>: change the color of leaf $v$ to $c$ ($c = 0$ means red, $c = 1$ means blue); </li><li> <span class="tex-font-style-tt">3 h</span>: update the current value of $k$ to $h$. </li></ul></div><div class="input-specification"><p>The first line of the input consists of two integers $n$ and $k$ ($2 \le n \le 10^{5}$, $-n \le k \le n$)&nbsp;— the number of nodes and the initial parameter $k$.</p><p>Each of the next $n - 1$ lines contains two integers $u$ and $v$ ($1 \le u,v \le n$), denoting that there is an edge between vertices $u$ and $v$.</p><p>The next line consists of $n$ space separated integers&nbsp;— the initial array $s$ ($-1 \le s_i \le 1$). $s_{i} = 0$ means that the color of node $i$ is red. $s_{i} = 1$ means that the color of node $i$ is blue. $s_{i} = -1$ means that the node $i$ is not a leaf.</p><p>The next line contains an integer $q$ ($1 \le q \le 10^5$), the number of queries.</p><p>$q$ lines follow, each containing a query in one of the following queries: </p><ul> <li> <span class="tex-font-style-tt">1 v</span> ($1 \le v \le n$): print the color of node $v$; </li><li> <span class="tex-font-style-tt">2 v c</span> ($1 \le v \le n$, $c = 0$ or $c = 1$): change the color of leaf $v$ to $c$ ($c = 0$ means red, $c = 1$ means blue). It is guaranteed that $v$ is a leaf; </li><li> <span class="tex-font-style-tt">3 h</span> ($-n \le h \le n$): update the current value of $k$ to $h$. </li></ul></div><div class="output-specification"><p>For each query of the first type, print $0$ if the color of vertex $v$ is red, and $1$ otherwise.</p></div>

## Input

<p>The first line of the input consists of two integers $n$ and $k$ ($2 \le n \le 10^{5}$, $-n \le k \le n$)&nbsp;— the number of nodes and the initial parameter $k$.</p><p>Each of the next $n - 1$ lines contains two integers $u$ and $v$ ($1 \le u,v \le n$), denoting that there is an edge between vertices $u$ and $v$.</p><p>The next line consists of $n$ space separated integers&nbsp;— the initial array $s$ ($-1 \le s_i \le 1$). $s_{i} = 0$ means that the color of node $i$ is red. $s_{i} = 1$ means that the color of node $i$ is blue. $s_{i} = -1$ means that the node $i$ is not a leaf.</p><p>The next line contains an integer $q$ ($1 \le q \le 10^5$), the number of queries.</p><p>$q$ lines follow, each containing a query in one of the following queries: </p><ul> <li> <span class="tex-font-style-tt">1 v</span> ($1 \le v \le n$): print the color of node $v$; </li><li> <span class="tex-font-style-tt">2 v c</span> ($1 \le v \le n$, $c = 0$ or $c = 1$): change the color of leaf $v$ to $c$ ($c = 0$ means red, $c = 1$ means blue). It is guaranteed that $v$ is a leaf; </li><li> <span class="tex-font-style-tt">3 h</span> ($-n \le h \le n$): update the current value of $k$ to $h$. </li></ul>

## Output

<p>For each query of the first type, print $0$ if the color of vertex $v$ is red, and $1$ otherwise.</p>





```input1
5 2
1 2
1 3
2 4
2 5
-1 -1 0 1 0
9
1 1
1 2
3 -2
1 1
1 2
3 1
2 5 1
1 1
1 2
```




```output1
0
0
1
1
0
1
```



## Note

<center> <span class="tex-font-size-small"><span class="tex-font-style-bf">Figures:</span><p>(i) The initial tree </p><p>(ii) The tree after the 3rd query </p><p>(iii) The tree after the 7th query </p><p>  </p></span> <img class="tex-graphics" src="file://i2i8qgol.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
