## Description

<div><p>You are given an undirected tree consisting of $n$ vertices. An undirected tree is a connected undirected graph with $n - 1$ edges.</p><p>Your task is to add the minimum number of edges in such a way that the length of the shortest path from the vertex $1$ to any other vertex is at most $2$. Note that you are not allowed to add loops and multiple edges.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of vertices in the tree.</p><p>The following $n - 1$ lines contain edges: edge $i$ is given as a pair of vertices $u_i, v_i$ ($1 \le u_i, v_i \le n$). It is guaranteed that the given edges form a tree. <span class="tex-font-style-it">It is guaranteed that there are no loops and multiple edges in the given edges.</span></p></div><div class="output-specification"><p>Print a single integer — the minimum number of edges you have to add in order to make the shortest distance from the vertex $1$ to any other vertex at most $2$. Note that you are not allowed to add loops and multiple edges.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of vertices in the tree.</p><p>The following $n - 1$ lines contain edges: edge $i$ is given as a pair of vertices $u_i, v_i$ ($1 \le u_i, v_i \le n$). It is guaranteed that the given edges form a tree. <span class="tex-font-style-it">It is guaranteed that there are no loops and multiple edges in the given edges.</span></p>

## Output

<p>Print a single integer — the minimum number of edges you have to add in order to make the shortest distance from the vertex $1$ to any other vertex at most $2$. Note that you are not allowed to add loops and multiple edges.</p>





```input1
7
1 2
2 3
2 4
4 5
4 6
5 7

```




```input2
7
1 2
1 3
2 4
2 5
3 6
1 7

```




```input3
7
1 2
2 3
3 4
3 5
3 6
3 7

```




```output1
2

```




```output2
0

```




```output3
1

```



## Note

<p>The tree corresponding to the first example: <img class="tex-graphics" src="file://MhlhTMsD.png" style="max-width: 100.0%;max-height: 100.0%;"> The answer is $2$, some of the possible answers are the following: $[(1, 5), (1, 6)]$, $[(1, 4), (1, 7)]$, $[(1, 6), (1, 7)]$.</p><p>The tree corresponding to the second example: <img class="tex-graphics" src="file://BFo3RfTW.png" style="max-width: 100.0%;max-height: 100.0%;"> The answer is $0$.</p><p>The tree corresponding to the third example: <img class="tex-graphics" src="file://8et3Vlo8.png" style="max-width: 100.0%;max-height: 100.0%;"> The answer is $1$, only one possible way to reach it is to add the edge $(1, 3)$.</p>
