## Description

<div><p>It's the year 5555. You have a graph, and you want to find a long cycle and a huge independent set, just because you can. But for now, let's just stick with finding either.</p><p>Given a connected graph with $n$ vertices, you can choose to either:</p><ul> <li> find an independent set that has <span class="tex-font-style-bf">exactly</span> $\lceil\sqrt{n}\rceil$ vertices.</li><li> find a <span class="tex-font-style-bf">simple</span> cycle of length <span class="tex-font-style-bf">at least</span> $\lceil\sqrt{n}\rceil$. </li></ul><p>An independent set is a set of vertices such that no two of them are connected by an edge. A simple cycle is a cycle that doesn't contain any vertex twice. I have a proof you can always solve one of these problems, but it's too long to fit this margin.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($5 \le n \le 10^5$, $n-1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of vertices and edges in the graph.</p><p>Each of the next $m$ lines contains two space-separated integers $u$ and $v$ ($1 \le u,v \le n$) that mean there's an edge between vertices $u$ and $v$. It's guaranteed that the graph is connected and doesn't contain any self-loops or multiple edges.</p></div><div class="output-specification"><p>If you choose to solve the first problem, then on the first line print "1", followed by a line containing $\lceil\sqrt{n}\rceil$ distinct integers not exceeding $n$, the vertices in the desired independent set.</p><p>If you, however, choose to solve the second problem, then on the first line print "2", followed by a line containing one integer, $c$, representing the length of the found cycle, followed by a line containing $c$ distinct integers integers not exceeding $n$, the vertices in the desired cycle, <span class="tex-font-style-bf">in the order they appear in the cycle</span>.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($5 \le n \le 10^5$, $n-1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of vertices and edges in the graph.</p><p>Each of the next $m$ lines contains two space-separated integers $u$ and $v$ ($1 \le u,v \le n$) that mean there's an edge between vertices $u$ and $v$. It's guaranteed that the graph is connected and doesn't contain any self-loops or multiple edges.</p>

## Output

<p>If you choose to solve the first problem, then on the first line print "1", followed by a line containing $\lceil\sqrt{n}\rceil$ distinct integers not exceeding $n$, the vertices in the desired independent set.</p><p>If you, however, choose to solve the second problem, then on the first line print "2", followed by a line containing one integer, $c$, representing the length of the found cycle, followed by a line containing $c$ distinct integers integers not exceeding $n$, the vertices in the desired cycle, <span class="tex-font-style-bf">in the order they appear in the cycle</span>.</p>





```input1
6 6
1 3
3 4
4 2
2 6
5 6
5 1
```




```input2
6 8
1 3
3 4
4 2
2 6
5 6
5 1
1 4
2 5
```




```input3
5 4
1 2
1 3
2 4
2 5
```




```output1
1
1 6 4
```




```output2
2
4
1 5 2 4
```




```output3
1
3 4 5
```



## Note

<p>In the first sample:</p><p><img class="tex-graphics" src="file://ZXAtGaip.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Notice that you can solve either problem, so printing the cycle $2-4-3-1-5-6$ is also acceptable.</p><p>In the second sample:</p><p><img class="tex-graphics" src="file://Ka3oI2Tb.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Notice that if there are multiple answers you can print any, so printing the cycle $2-5-6$, for example, is acceptable.</p><p>In the third sample:</p><p><img class="tex-graphics" src="file://2SJ1JWmn.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
