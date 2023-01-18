## Description

<div><p>You are given a weighed undirected <span class="tex-font-style-bf">connected</span> graph, consisting of $n$ vertices and $m$ edges.</p><p>You should answer $q$ queries, the $i$-th query is to find the shortest distance between vertices $u_i$ and $v_i$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m~(1 \le n, m \le 10^5, m - n \le 20)$ — the number of vertices and edges in the graph.</p><p>Next $m$ lines contain the edges: the $i$-th edge is a triple of integers $v_i, u_i, d_i~(1 \le u_i, v_i \le n, 1 \le d_i \le 10^9, u_i \neq v_i)$. This triple means that there is an edge between vertices $u_i$ and $v_i$ of weight $d_i$. It is guaranteed that graph contains no self-loops and multiple edges.</p><p>The next line contains a single integer $q~(1 \le q \le 10^5)$ — the number of queries.</p><p>Each of the next $q$ lines contains two integers $u_i$ and $v_i~(1 \le u_i, v_i \le n)$ — descriptions of the queries.</p><p><span class="tex-font-style-bf">Pay attention to the restriction $m - n ~ \le ~ 20$.</span></p></div><div class="output-specification"><p>Print $q$ lines.</p><p>The $i$-th line should contain the answer to the $i$-th query — the shortest distance between vertices $u_i$ and $v_i$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m~(1 \le n, m \le 10^5, m - n \le 20)$ — the number of vertices and edges in the graph.</p><p>Next $m$ lines contain the edges: the $i$-th edge is a triple of integers $v_i, u_i, d_i~(1 \le u_i, v_i \le n, 1 \le d_i \le 10^9, u_i \neq v_i)$. This triple means that there is an edge between vertices $u_i$ and $v_i$ of weight $d_i$. It is guaranteed that graph contains no self-loops and multiple edges.</p><p>The next line contains a single integer $q~(1 \le q \le 10^5)$ — the number of queries.</p><p>Each of the next $q$ lines contains two integers $u_i$ and $v_i~(1 \le u_i, v_i \le n)$ — descriptions of the queries.</p><p><span class="tex-font-style-bf">Pay attention to the restriction $m - n ~ \le ~ 20$.</span></p>

## Output

<p>Print $q$ lines.</p><p>The $i$-th line should contain the answer to the $i$-th query — the shortest distance between vertices $u_i$ and $v_i$.</p>





```input1
3 3
1 2 3
2 3 1
3 1 5
3
1 2
1 3
2 3

```




```input2
8 13
1 2 4
2 3 6
3 4 1
4 5 12
5 6 3
6 7 8
7 8 7
1 4 1
1 8 3
2 6 9
2 7 1
4 6 3
6 8 2
8
1 5
1 7
2 3
2 8
3 7
3 4
6 8
7 8

```




```output1
3
4
1

```




```output2
7
5
6
7
7
1
2
7

```


