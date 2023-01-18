## Description

<div><p>Vasya has a tree consisting of $n$ vertices with root in vertex $1$. At first all vertices has $0$ written on it.</p><p>Let $d(i, j)$ be the distance between vertices $i$ and $j$, i.e. number of edges in the shortest path from $i$ to $j$. Also, let's denote $k$-subtree of vertex $x$ — set of vertices $y$ such that next two conditions are met: </p><ul> <li> $x$ is the ancestor of $y$ (each vertex is the ancestor of itself); </li><li> $d(x, y) \le k$. </li></ul><p>Vasya needs you to process $m$ queries. The $i$-th query is a triple $v_i$, $d_i$ and $x_i$. For each query Vasya adds value $x_i$ to each vertex from $d_i$-subtree of $v_i$.</p><p>Report to Vasya all values, written on vertices of the tree after processing all queries.</p></div><div class="input-specification"><p>The first line contains single integer $n$ ($1 \le n \le 3 \cdot 10^5$) — number of vertices in the tree.</p><p>Each of next $n - 1$ lines contains two integers $x$ and $y$ ($1 \le x, y \le n$) — edge between vertices $x$ and $y$. It is guarantied that given graph is a tree.</p><p>Next line contains single integer $m$ ($1 \le m \le 3 \cdot 10^5$) — number of queries.</p><p>Each of next $m$ lines contains three integers $v_i$, $d_i$, $x_i$ ($1 \le v_i \le n$, $0 \le d_i \le 10^9$, $1 \le x_i \le 10^9$) — description of the $i$-th query.</p></div><div class="output-specification"><p>Print $n$ integers. The $i$-th integers is the value, written in the $i$-th vertex after processing all queries.</p></div>

## Input

<p>The first line contains single integer $n$ ($1 \le n \le 3 \cdot 10^5$) — number of vertices in the tree.</p><p>Each of next $n - 1$ lines contains two integers $x$ and $y$ ($1 \le x, y \le n$) — edge between vertices $x$ and $y$. It is guarantied that given graph is a tree.</p><p>Next line contains single integer $m$ ($1 \le m \le 3 \cdot 10^5$) — number of queries.</p><p>Each of next $m$ lines contains three integers $v_i$, $d_i$, $x_i$ ($1 \le v_i \le n$, $0 \le d_i \le 10^9$, $1 \le x_i \le 10^9$) — description of the $i$-th query.</p>

## Output

<p>Print $n$ integers. The $i$-th integers is the value, written in the $i$-th vertex after processing all queries.</p>





```input1
5
1 2
1 3
2 4
2 5
3
1 1 1
2 0 10
4 10 100
```




```input2
5
2 3
2 1
5 4
3 4
5
2 0 4
3 10 1
1 2 3
2 3 10
1 1 7
```




```output1
1 11 1 100 0
```




```output2
10 24 14 11 11
```



## Note

<p>In the first exapmle initial values in vertices are $0, 0, 0, 0, 0$. After the first query values will be equal to $1, 1, 1, 0, 0$. After the second query values will be equal to $1, 11, 1, 0, 0$. After the third query values will be equal to $1, 11, 1, 100, 0$.</p>
