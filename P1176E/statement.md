## Description

<div><p>You are given an undirected unweighted connected graph consisting of $n$ vertices and $m$ edges. It is guaranteed that there are no self-loops or multiple edges in the given graph.</p><p>Your task is to choose <span class="tex-font-style-bf">at most</span> $\lfloor\frac{n}{2}\rfloor$ vertices in this graph so <span class="tex-font-style-bf">each</span> unchosen vertex is adjacent (in other words, connected by an edge) to at least one of chosen vertices.</p><p>It is guaranteed that the answer exists. If there are multiple answers, you can print any.</p><p>You will be given multiple independent queries to answer.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^5$) — the number of queries.</p><p>Then $t$ queries follow.</p><p>The first line of each query contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $n - 1 \le m \le min(2 \cdot 10^5, \frac{n(n-1)}{2})$) — the number of vertices and the number of edges, respectively.</p><p>The following $m$ lines denote edges: edge $i$ is represented by a pair of integers $v_i$, $u_i$ ($1 \le v_i, u_i \le n$, $u_i \ne v_i$), which are the indices of vertices connected by the edge.</p><p>There are no self-loops or multiple edges in the given graph, i. e. for each pair ($v_i, u_i$) there are no other pairs ($v_i, u_i$) or ($u_i, v_i$) in the list of edges, and for each pair ($v_i, u_i$) the condition $v_i \ne u_i$ is satisfied. It is guaranteed that the given graph is <span class="tex-font-style-bf">connected</span>.</p><p>It is guaranteed that $\sum m \le 2 \cdot 10^5$ over all queries.</p></div><div class="output-specification"><p>For each query print two lines.</p><p>In the first line print $k$ ($1 \le \lfloor\frac{n}{2}\rfloor$) — the number of chosen vertices.</p><p>In the second line print $k$ <span class="tex-font-style-bf">distinct</span> integers $c_1, c_2, \dots, c_k$ in any order, where $c_i$ is the index of the $i$-th chosen vertex.</p><p>It is guaranteed that the answer exists. If there are multiple answers, you can print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^5$) — the number of queries.</p><p>Then $t$ queries follow.</p><p>The first line of each query contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $n - 1 \le m \le min(2 \cdot 10^5, \frac{n(n-1)}{2})$) — the number of vertices and the number of edges, respectively.</p><p>The following $m$ lines denote edges: edge $i$ is represented by a pair of integers $v_i$, $u_i$ ($1 \le v_i, u_i \le n$, $u_i \ne v_i$), which are the indices of vertices connected by the edge.</p><p>There are no self-loops or multiple edges in the given graph, i. e. for each pair ($v_i, u_i$) there are no other pairs ($v_i, u_i$) or ($u_i, v_i$) in the list of edges, and for each pair ($v_i, u_i$) the condition $v_i \ne u_i$ is satisfied. It is guaranteed that the given graph is <span class="tex-font-style-bf">connected</span>.</p><p>It is guaranteed that $\sum m \le 2 \cdot 10^5$ over all queries.</p>

## Output

<p>For each query print two lines.</p><p>In the first line print $k$ ($1 \le \lfloor\frac{n}{2}\rfloor$) — the number of chosen vertices.</p><p>In the second line print $k$ <span class="tex-font-style-bf">distinct</span> integers $c_1, c_2, \dots, c_k$ in any order, where $c_i$ is the index of the $i$-th chosen vertex.</p><p>It is guaranteed that the answer exists. If there are multiple answers, you can print any.</p>





```input1
2
4 6
1 2
1 3
1 4
2 3
2 4
3 4
6 8
2 5
5 4
4 3
4 1
1 3
2 3
2 6
5 6
```




```output1
2
1 3
3
4 3 6
```



## Note

<p>In the first query any vertex or any pair of vertices will suffice.</p><center> <img class="tex-graphics" src="file://2Zqw7v1p.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that you don't have to minimize the number of chosen vertices. In the second query two vertices can be enough (vertices $2$ and $4$) but three is also ok.</p><center> <img class="tex-graphics" src="file://oIvH2y2E.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
