## Description

<div><p>You are given an undirected graph consisting of $n$ vertices and $m$ edges. Initially there is a single integer written on every vertex: the vertex $i$ has $p_i$ written on it. All $p_i$ are distinct integers from $1$ to $n$.</p><p>You have to process $q$ queries of two types:</p><ul> <li> $1$ $v$ — among all vertices reachable from the vertex $v$ using the edges of the graph (including the vertex $v$ itself), find a vertex $u$ with the largest number $p_u$ written on it, print $p_u$ and replace $p_u$ with $0$; </li><li> $2$ $i$ — delete the $i$-th edge from the graph. </li></ul> <p>Note that, in a query of the first type, it is possible that all vertices reachable from $v$ have $0$ written on them. In this case, $u$ is not explicitly defined, but since the selection of $u$ does not affect anything, you can choose any vertex reachable from $v$ and print its value (which is $0$). </p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $q$ ($1 \le n \le 2 \cdot 10^5$; $1 \le m \le 3 \cdot 10^5$; $1 \le q \le 5 \cdot 10^5$).</p><p>The second line contains $n$ distinct integers $p_1$, $p_2$, ..., $p_n$, where $p_i$ is the number initially written on vertex $i$ ($1 \le p_i \le n$).</p><p>Then $m$ lines follow, the $i$-th of them contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$, $a_i \ne b_i$) and means that the $i$-th edge connects vertices $a_i$ and $b_i$. It is guaranteed that the graph does not contain multi-edges.</p><p>Then $q$ lines follow, which describe the queries. Each line is given by one of the following formats:</p><ul> <li> $1$ $v$ — denotes a query of the first type with a vertex $v$ ($1 \le v \le n$). </li><li> $2$ $i$ — denotes a query of the second type with an edge $i$ ($1 \le i \le m$). For each query of the second type, it is guaranteed that the corresponding edge is not deleted from the graph yet. </li></ul></div><div class="output-specification"><p>For every query of the first type, print the value of $p_u$ written on the chosen vertex $u$.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $q$ ($1 \le n \le 2 \cdot 10^5$; $1 \le m \le 3 \cdot 10^5$; $1 \le q \le 5 \cdot 10^5$).</p><p>The second line contains $n$ distinct integers $p_1$, $p_2$, ..., $p_n$, where $p_i$ is the number initially written on vertex $i$ ($1 \le p_i \le n$).</p><p>Then $m$ lines follow, the $i$-th of them contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$, $a_i \ne b_i$) and means that the $i$-th edge connects vertices $a_i$ and $b_i$. It is guaranteed that the graph does not contain multi-edges.</p><p>Then $q$ lines follow, which describe the queries. Each line is given by one of the following formats:</p><ul> <li> $1$ $v$ — denotes a query of the first type with a vertex $v$ ($1 \le v \le n$). </li><li> $2$ $i$ — denotes a query of the second type with an edge $i$ ($1 \le i \le m$). For each query of the second type, it is guaranteed that the corresponding edge is not deleted from the graph yet. </li></ul>

## Output

<p>For every query of the first type, print the value of $p_u$ written on the chosen vertex $u$.</p>





```input1
5 4 6
1 2 5 4 3
1 2
2 3
1 3
4 5
1 1
2 1
2 3
1 1
1 2
1 2
```




```output1
5
1
2
0
```


