## Description

<div><p>An edge-weighted tree of $n$ nodes is given with each edge colored in some color. Each node of this tree can be blocked or unblocked, all nodes are unblocked initially.</p><p>A <span class="tex-font-style-it">simple path</span> is a path in a graph that does not have repeating nodes. The <span class="tex-font-style-it">length</span> of a path is defined as the sum of weights of all edges on the path.</p><p>A path is <span class="tex-font-style-it">good</span> when it is a <span class="tex-font-style-it">simple path</span> consisting of edges of the same color $c$, all edges of color $c$ are on this path, and every node on the path is unblocked.</p><p>You need to operate $2$ kinds of queries: </p><ol> <li> block a node, </li><li> unblock a node. </li></ol><p>After each query, print the maximum <span class="tex-font-style-it">length</span> among all <span class="tex-font-style-it">good</span> paths. If there are no <span class="tex-font-style-it">good</span> paths, print $0$.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $q$ ($1 \leq n,q \leq 2\cdot 10^5$) — the number of nodes and the number of queries.</p><p>Then $n-1$ lines follow, each containing four integers $u$, $v$, $w$ and $c$ ($1 \leq u,v,w,c \leq n$; $u \not = v$), denoting a weighted edge connecting node $u$ and node $v$ with weight $w$ and color $c$. It is guaranteed that these edges form a tree.</p><p>Then $q$ lines follow, each containing two integers $p$ and $x$ ($p = 0$ or $p = 1$, $1\leq x\leq n$), denoting a query: </p><ol> <li> if $p = 0$, block the node $x$. It's guaranteed that it's not blocked at this time; </li><li> if $p = 1$, unblock the node $x$. It's guaranteed that it's blocked at this time. </li></ol></div><div class="output-specification"><p>For each query, print the maximum length of a <span class="tex-font-style-it">good</span> path. If there are no <span class="tex-font-style-it">good</span> paths, print $0$.</p></div>

## Input

<p>The first line contains two integers $n$, $q$ ($1 \leq n,q \leq 2\cdot 10^5$) — the number of nodes and the number of queries.</p><p>Then $n-1$ lines follow, each containing four integers $u$, $v$, $w$ and $c$ ($1 \leq u,v,w,c \leq n$; $u \not = v$), denoting a weighted edge connecting node $u$ and node $v$ with weight $w$ and color $c$. It is guaranteed that these edges form a tree.</p><p>Then $q$ lines follow, each containing two integers $p$ and $x$ ($p = 0$ or $p = 1$, $1\leq x\leq n$), denoting a query: </p><ol> <li> if $p = 0$, block the node $x$. It's guaranteed that it's not blocked at this time; </li><li> if $p = 1$, unblock the node $x$. It's guaranteed that it's blocked at this time. </li></ol>

## Output

<p>For each query, print the maximum length of a <span class="tex-font-style-it">good</span> path. If there are no <span class="tex-font-style-it">good</span> paths, print $0$.</p>





```input1
5 4
4 1 3 4
5 2 4 4
3 1 3 2
1 2 5 1
0 4
0 3
0 2
1 3
```




```input2
5 5
4 1 4 4
4 5 2 2
3 1 2 4
3 2 3 1
0 3
0 4
1 3
1 4
0 1
```




```input3
6 9
3 2 2 3
2 4 4 2
3 1 5 5
6 4 3 2
5 3 1 3
0 2
0 4
0 5
0 6
1 2
1 4
1 5
0 3
1 6
```




```input4
1 2
0 1
1 1
```




```output1
5
5
0
3
```




```output2
2
0
3
6
3
```




```output3
5
5
5
5
5
5
5
0
7
```




```output4
0
0
```


