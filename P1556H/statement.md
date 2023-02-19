## Description

<div><center> <img class="tex-graphics" height="302px" src="file://5vM05l3Y.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>William really likes puzzle kits. For one of his birthdays, his friends gifted him a complete undirected edge-weighted graph consisting of $n$ vertices.</p><p>He wants to build a spanning tree of this graph, such that for the first $k$ vertices the following condition is satisfied: the degree of a vertex with index $i$ does not exceed $d_i$. Vertices from $k + 1$ to $n$ may have any degree.</p><p>William wants you to find the minimum weight of a spanning tree that satisfies all the conditions.</p><p>A spanning tree is a subset of edges of a graph that forms a tree on all $n$ vertices of the graph. The weight of a spanning tree is defined as the sum of weights of all the edges included in a spanning tree.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$, $k$ ($2 \leq n \leq 50$, $1 \leq k \leq min(n - 1, 5)$).</p><p>The second line contains $k$ integers $d_1, d_2, \ldots, d_k$ ($1 \leq d_i \leq n$). </p><p>The $i$-th of the next $n - 1$ lines contains $n - i$ integers $w_{i,i+1}, w_{i,i+2}, \ldots, w_{i,n}$ ($1 \leq w_{i,j} \leq 100$): weights of edges $(i,i+1),(i,i+2),\ldots,(i,n)$.</p></div><div class="output-specification"><p>Print one integer: the minimum weight of a spanning tree under given degree constraints for the first $k$ vertices. </p></div>

## Input

<p>The first line of input contains two integers $n$, $k$ ($2 \leq n \leq 50$, $1 \leq k \leq min(n - 1, 5)$).</p><p>The second line contains $k$ integers $d_1, d_2, \ldots, d_k$ ($1 \leq d_i \leq n$). </p><p>The $i$-th of the next $n - 1$ lines contains $n - i$ integers $w_{i,i+1}, w_{i,i+2}, \ldots, w_{i,n}$ ($1 \leq w_{i,j} \leq 100$): weights of edges $(i,i+1),(i,i+2),\ldots,(i,n)$.</p>

## Output

<p>Print one integer: the minimum weight of a spanning tree under given degree constraints for the first $k$ vertices. </p>





```input1
10 5
5 3 4 2 1
29 49 33 12 55 15 32 62 37
61 26 15 58 15 22 8 58
37 16 9 39 20 14 58
10 15 40 3 19 55
53 13 37 44 52
23 59 58 4
69 80 29
89 28
48
```




```output1
95
```


