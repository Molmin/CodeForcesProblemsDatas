## Description

<div><p>You are given a weighted undirected connected graph consisting of $n$ vertices and $m$ edges. It is guaranteed that there are no self-loops or multiple edges in the given graph.</p><p>Let's define the weight of the path consisting of $k$ edges with indices $e_1, e_2, \dots, e_k$ as $\sum\limits_{i=1}^{k}{w_{e_i}} - \max\limits_{i=1}^{k}{w_{e_i}} + \min\limits_{i=1}^{k}{w_{e_i}}$, where $w_i$ — weight of the $i$-th edge in the graph.</p><p>Your task is to find the minimum weight of the path from the $1$-st vertex to the $i$-th vertex for each $i$ ($2 \le i \le n$).</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$; $1 \le m \le 2 \cdot 10^5$) — the number of vertices and the number of edges in the graph.</p><p>Following $m$ lines contains three integers $v_i, u_i, w_i$ ($1 \le v_i, u_i \le n$; $1 \le w_i \le 10^9$; $v_i \neq u_i$) — endpoints of the $i$-th edge and its weight respectively.</p></div><div class="output-specification"><p>Print $n-1$ integers — the minimum weight of the path from $1$-st vertex to the $i$-th vertex for each $i$ ($2 \le i \le n$).</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$; $1 \le m \le 2 \cdot 10^5$) — the number of vertices and the number of edges in the graph.</p><p>Following $m$ lines contains three integers $v_i, u_i, w_i$ ($1 \le v_i, u_i \le n$; $1 \le w_i \le 10^9$; $v_i \neq u_i$) — endpoints of the $i$-th edge and its weight respectively.</p>

## Output

<p>Print $n-1$ integers — the minimum weight of the path from $1$-st vertex to the $i$-th vertex for each $i$ ($2 \le i \le n$).</p>





```input1
5 4
5 3 4
2 1 1
3 2 2
2 4 2
```




```input2
6 8
3 1 1
3 6 2
5 4 2
4 2 2
6 1 1
5 2 1
3 2 3
1 5 4
```




```input3
7 10
7 5 5
2 3 3
4 7 1
5 3 6
2 7 6
6 2 6
3 7 6
4 2 1
3 1 4
1 7 4
```




```output1
1 2 2 4
```




```output2
2 1 4 3 1
```




```output3
3 4 2 7 7 3
```


