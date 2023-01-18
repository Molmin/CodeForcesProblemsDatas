## Description

<div><p>Given a connected undirected graph with $n$ vertices and an integer $k$, you have to either:</p><ul> <li> either find an independent set that has <span class="tex-font-style-bf">exactly</span> $\lceil\frac{k}{2}\rceil$ vertices.</li><li> or find a <span class="tex-font-style-bf">simple</span> cycle of length <span class="tex-font-style-bf">at most</span> $k$. </li></ul><p>An independent set is a set of vertices such that no two of them are connected by an edge. A simple cycle is a cycle that doesn't contain any vertex twice. </p><p>I have a proof that for any input you can always solve at least one of these problems, but it's left as an exercise for the reader.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, and $k$ ($3 \le k \le n \le 10^5$, $n-1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of vertices and edges in the graph, and the parameter $k$ from the statement.</p><p>Each of the next $m$ lines contains two integers $u$ and $v$ ($1 \le u,v \le n$) that mean there's an edge between vertices $u$ and $v$. It's guaranteed that the graph is connected and doesn't contain any self-loops or multiple edges.</p></div><div class="output-specification"><p>If you choose to solve the first problem, then on the first line print $1$, followed by a line containing $\lceil\frac{k}{2}\rceil$ distinct integers not exceeding $n$, the vertices in the desired independent set.</p><p>If you, however, choose to solve the second problem, then on the first line print $2$, followed by a line containing one integer, $c$, representing the length of the found cycle, followed by a line containing $c$ distinct integers not exceeding $n$, the vertices in the desired cycle, <span class="tex-font-style-bf">in the order they appear in the cycle</span>.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, and $k$ ($3 \le k \le n \le 10^5$, $n-1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of vertices and edges in the graph, and the parameter $k$ from the statement.</p><p>Each of the next $m$ lines contains two integers $u$ and $v$ ($1 \le u,v \le n$) that mean there's an edge between vertices $u$ and $v$. It's guaranteed that the graph is connected and doesn't contain any self-loops or multiple edges.</p>

## Output

<p>If you choose to solve the first problem, then on the first line print $1$, followed by a line containing $\lceil\frac{k}{2}\rceil$ distinct integers not exceeding $n$, the vertices in the desired independent set.</p><p>If you, however, choose to solve the second problem, then on the first line print $2$, followed by a line containing one integer, $c$, representing the length of the found cycle, followed by a line containing $c$ distinct integers not exceeding $n$, the vertices in the desired cycle, <span class="tex-font-style-bf">in the order they appear in the cycle</span>.</p>





```input1
4 4 3
1 2
2 3
3 4
4 1
```




```input2
4 5 3
1 2
2 3
3 4
4 1
2 4
```




```input3
4 6 3
1 2
2 3
3 4
4 1
1 3
2 4
```




```input4
5 4 5
1 2
1 3
2 4
2 5
```




```output1
1
1 3
```




```output2
2
3
2 3 4
```




```output3
2
3
1 2 3
```




```output4
1
1 4 5
```



## Note

<p>In the first sample:</p><p><img class="tex-graphics" src="file://mJ3e3OCC.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Notice that printing the independent set $\{2,4\}$ is also OK, but printing the cycle $1-2-3-4$ isn't, because its length must be at most $3$.</p><p>In the second sample:</p><p><img class="tex-graphics" src="file://AVIyqOaY.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Notice that printing the independent set $\{1,3\}$ or printing the cycle $2-1-4$ is also OK.</p><p>In the third sample:</p><p><img class="tex-graphics" src="file://HdZCqR4B.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the fourth sample:</p><p><img class="tex-graphics" src="file://Ge8E1HC7.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
