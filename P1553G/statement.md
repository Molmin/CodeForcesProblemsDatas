## Description

<div><p>Consider a sequence of distinct integers $a_1, \ldots, a_n$, each representing one node of a graph. There is an edge between two nodes if the two values are not coprime, i.&nbsp;e. they have a common divisor greater than $1$.</p><p>There are $q$ queries, in each query, you want to get from one given node $a_s$ to another $a_t$. In order to achieve that, you can choose an existing value $a_i$ and create new value $a_{n+1} = a_i \cdot (1 + a_i)$, with edges to all values that are not coprime with $a_{n+1}$. Also, $n$ gets increased by $1$. You can repeat that operation multiple times, possibly making the sequence much longer and getting huge or repeated values. What's the minimum possible number of newly created nodes so that $a_t$ is reachable from $a_s$?</p><p>Queries are independent. In each query, you start with the initial sequence $a$ given in the input.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($2 \leq n \leq 150\,000$, $1 \leq q \leq 300\,000$)&nbsp;— the size of the sequence and the number of queries.</p><p>The second line contains $n$ <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \ldots, a_n$ ($2 \leq a_i \leq 10^6$, $a_i \neq a_j$ if $i \ne j$).</p><p>The $j$-th of the following $q$ lines contains two distinct integers $s_j$ and $t_j$ ($1 \leq s_j, t_j \leq n$, $s_j \neq t_j$)&nbsp;— indices of nodes for $j$-th query.</p></div><div class="output-specification"><p>Print $q$ lines. The $j$-th line should contain one integer: the minimum number of new nodes you create in order to move from $a_{s_j}$ to $a_{t_j}$.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($2 \leq n \leq 150\,000$, $1 \leq q \leq 300\,000$)&nbsp;— the size of the sequence and the number of queries.</p><p>The second line contains $n$ <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \ldots, a_n$ ($2 \leq a_i \leq 10^6$, $a_i \neq a_j$ if $i \ne j$).</p><p>The $j$-th of the following $q$ lines contains two distinct integers $s_j$ and $t_j$ ($1 \leq s_j, t_j \leq n$, $s_j \neq t_j$)&nbsp;— indices of nodes for $j$-th query.</p>

## Output

<p>Print $q$ lines. The $j$-th line should contain one integer: the minimum number of new nodes you create in order to move from $a_{s_j}$ to $a_{t_j}$.</p>





```input1
3 3
2 10 3
1 2
1 3
2 3
```




```input2
5 12
3 8 7 6 25
1 2
1 3
1 4
1 5
2 1
2 3
2 4
2 5
3 1
3 2
3 4
3 5
```




```output1
0
1
1
```




```output2
0
1
0
1
0
1
0
1
1
1
1
2
```



## Note

<p>In the first example, you can first create new value $2 \cdot 3 = 6$ or $10 \cdot 11 = 110$ or $3 \cdot 4 = 12$. None of that is needed in the first query because you can already get from $a_1 = 2$ to $a_2 = 10$.</p><p>In the second query, it's optimal to first create $6$ or $12$. For example, creating $6$ makes it possible to get from $a_1 = 2$ to $a_3 = 3$ with a path $(2, 6, 3)$.</p><center> <img class="tex-graphics" src="file://iAcuRmXC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the last query of the second example, we want to get from $a_3 = 7$ to $a_5 = 25$. One way to achieve that is to first create $6 \cdot 7 = 42$ and then create $25 \cdot 26 = 650$. The final graph has seven nodes and it contains a path from $a_3 = 7$ to $a_5 = 25$.</p>
