## Description

<div><p>You are given a tree of $n$ vertices numbered from $1$ to $n$. A tree is a connected undirected graph without cycles. </p><p>For each $i=1,2, \ldots, n$, let $w_i$ be the weight of the $i$-th vertex. A vertex is called <span class="tex-font-style-it">good</span> if its weight is equal to the sum of the weights of all its neighbors.</p><p>Initially, the weights of all nodes are unassigned. Assign positive integer weights to each vertex of the tree, such that the number of good vertices in the tree is maximized. If there are multiple ways to do it, you have to find one that minimizes the sum of weights of all vertices in the tree.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2\le n\le 2\cdot 10^5$) — the number of vertices in the tree.</p><p>Then, $n−1$ lines follow. Each of them contains two integers $u$ and $v$ ($1\le u,v\le n$) denoting an edge between vertices $u$ and $v$. It is guaranteed that the edges form a tree.</p></div><div class="output-specification"><p>In the first line print two integers &nbsp;— the maximum number of good vertices and the minimum possible sum of weights for that maximum.</p><p>In the second line print $n$ integers $w_1, w_2, \ldots, w_n$ ($1\le w_i\le 10^9$) &nbsp;— the corresponding weight assigned to each vertex. It can be proven that there exists an optimal solution satisfying these constraints.</p><p>If there are multiple optimal solutions, you may print any.</p></div>

## Input

<p>The first line contains one integer $n$ ($2\le n\le 2\cdot 10^5$) — the number of vertices in the tree.</p><p>Then, $n−1$ lines follow. Each of them contains two integers $u$ and $v$ ($1\le u,v\le n$) denoting an edge between vertices $u$ and $v$. It is guaranteed that the edges form a tree.</p>

## Output

<p>In the first line print two integers &nbsp;— the maximum number of good vertices and the minimum possible sum of weights for that maximum.</p><p>In the second line print $n$ integers $w_1, w_2, \ldots, w_n$ ($1\le w_i\le 10^9$) &nbsp;— the corresponding weight assigned to each vertex. It can be proven that there exists an optimal solution satisfying these constraints.</p><p>If there are multiple optimal solutions, you may print any.</p>





```input1
4
1 2
2 3
2 4
```




```input2
3
1 2
1 3
```




```input3
2
1 2
```




```input4
9
3 4
7 6
2 1
8 3
5 6
1 8
8 6
9 6
```




```output1
3 4
1 1 1 1
```




```output2
2 3
1 1 1
```




```output3
2 2
1 1
```




```output4
6 11
1 1 1 1 1 1 1 3 1
```



## Note

<p>This is the tree for the first test case: </p><center> <img class="tex-graphics" src="file://IPevhZO6.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px"> </center> In this case, if you assign a weight of $1$ to each vertex, then the good vertices (which are painted black) are $1$, $3$ and $4$. It impossible to assign weights so that all vertices are good vertices. The minimum sum of weights in this case is $1+1+1+1=4$, and it is impossible to have a lower sum because the weights have to be positive integers.<p>This is the tree for the second test case: </p><center> <img class="tex-graphics" src="file://sr3MZ5Qa.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px"> </center> In this case, if you assign a weight of $1$ to each vertex, then the good vertices (which are painted black) are $2$ and $3$. It can be proven that this is an optimal assignment.
