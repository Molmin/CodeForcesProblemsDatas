## Description

<div><p>You have a simple undirected graph consisting of $n$ vertices and $m$ edges. The graph doesn't contain self-loops, there is at most one edge between a pair of vertices. The given graph can be disconnected.</p><p>Let's make a definition.</p><p>Let $v_1$ and $v_2$ be two some nonempty subsets of vertices that do not intersect. Let $f(v_{1}, v_{2})$ be true if and only if all the conditions are satisfied:</p><ol> <li> There are no edges with both endpoints in vertex set $v_1$. </li><li> There are no edges with both endpoints in vertex set $v_2$. </li><li> For every two vertices $x$ and $y$ such that $x$ is in $v_1$ and $y$ is in $v_2$, there is an edge between $x$ and $y$. </li></ol><p>Create three vertex sets ($v_{1}$, $v_{2}$, $v_{3}$) which satisfy the conditions below;</p><ol> <li> All vertex sets should not be empty. </li><li> Each vertex should be assigned to only one vertex set. </li><li> $f(v_{1}, v_{2})$, $f(v_{2}, v_{3})$, $f(v_{3}, v_{1})$ are all true. </li></ol><p>Is it possible to create such three vertex sets? If it's possible, print matching vertex set for each vertex.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($3 \le n \le 10^{5}$, $0 \le m \le \text{min}(3 \cdot 10^{5}, \frac{n(n-1)}{2})$)&nbsp;— the number of vertices and edges in the graph.</p><p>The $i$-th of the next $m$ lines contains two integers $a_{i}$ and $b_{i}$ ($1 \le a_{i} \lt b_{i} \le n$)&nbsp;— it means there is an edge between $a_{i}$ and $b_{i}$. The graph doesn't contain self-loops, there is at most one edge between a pair of vertices. The given graph can be disconnected.</p></div><div class="output-specification"><p>If the answer exists, print $n$ integers. $i$-th integer means the vertex set number (from $1$ to $3$) of $i$-th vertex. Otherwise, print $-1$.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($3 \le n \le 10^{5}$, $0 \le m \le \text{min}(3 \cdot 10^{5}, \frac{n(n-1)}{2})$)&nbsp;— the number of vertices and edges in the graph.</p><p>The $i$-th of the next $m$ lines contains two integers $a_{i}$ and $b_{i}$ ($1 \le a_{i} \lt b_{i} \le n$)&nbsp;— it means there is an edge between $a_{i}$ and $b_{i}$. The graph doesn't contain self-loops, there is at most one edge between a pair of vertices. The given graph can be disconnected.</p>

## Output

<p>If the answer exists, print $n$ integers. $i$-th integer means the vertex set number (from $1$ to $3$) of $i$-th vertex. Otherwise, print $-1$.</p><p>If there are multiple answers, print any.</p>





```input1
6 11
1 2
1 3
1 4
1 5
1 6
2 4
2 5
2 6
3 4
3 5
3 6
```




```input2
4 6
1 2
1 3
1 4
2 3
2 4
3 4
```




```output1
1 2 2 3 3 3
```




```output2
-1
```



## Note

<p>In the first example, if $v_{1} = \{ 1 \}$, $v_{2} = \{ 2, 3 \}$, and $v_{3} = \{ 4, 5, 6 \}$ then vertex sets will satisfy all conditions. But you can assign vertices to vertex sets in a different way; Other answers like "<span class="tex-font-style-tt">2 3 3 1 1 1</span>" will be accepted as well.</p><center> <img class="tex-graphics" src="file://u8iaLJ6n.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, it's impossible to make such vertex sets.</p>
