## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The only difference between the two versions is the constraint on $n$. You can make hacks only if all versions of the problem are solved.</span></p><p>A forest is an undirected graph without cycles (not necessarily connected).</p><p>Mocha and Diana are friends in Zhijiang, both of them have a forest with nodes numbered from $1$ to $n$, and they would like to add edges to their forests such that: </p><ul> <li> After adding edges, both of their graphs are still forests. </li><li> They add the same edges. That is, if an edge $(u, v)$ is added to Mocha's forest, then an edge $(u, v)$ is added to Diana's forest, and vice versa. </li></ul><p>Mocha and Diana want to know the maximum number of edges they can add, and which edges to add.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m_1$ and $m_2$ ($1 \le n \le 1000$, $0 \le m_1, m_2 &lt; n$) — the number of nodes and the number of initial edges in Mocha's forest and Diana's forest.</p><p>Each of the next $m_1$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$) — the edges in Mocha's forest.</p><p>Each of the next $m_2$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$) — the edges in Diana's forest.</p></div><div class="output-specification"><p>The first line contains only one integer $h$, the maximum number of edges Mocha and Diana can add (in each forest).</p><p>Each of the next $h$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$) — the edge you add each time.</p><p>If there are multiple correct answers, you can print any one of them.</p></div>

## Input

<p>The first line contains three integers $n$, $m_1$ and $m_2$ ($1 \le n \le 1000$, $0 \le m_1, m_2 &lt; n$) — the number of nodes and the number of initial edges in Mocha's forest and Diana's forest.</p><p>Each of the next $m_1$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$) — the edges in Mocha's forest.</p><p>Each of the next $m_2$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$) — the edges in Diana's forest.</p>

## Output

<p>The first line contains only one integer $h$, the maximum number of edges Mocha and Diana can add (in each forest).</p><p>Each of the next $h$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$) — the edge you add each time.</p><p>If there are multiple correct answers, you can print any one of them.</p>





```input1
3 2 2
1 2
2 3
1 2
1 3
```




```input2
5 3 2
5 4
2 1
4 3
4 3
1 4
```




```input3
8 1 2
1 7
2 6
1 5
```




```output1
0
```




```output2
1
2 4
```




```output3
5
5 2
2 3
3 4
4 7
6 8
```



## Note

<p>In the first example, we cannot add any edge.</p><p>In the second example, the initial forests are as follows.</p><p><img class="tex-graphics" src="file://asyRBuHl.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>We can add an edge $(2, 4)$.</p><p><img class="tex-graphics" src="file://gYuJkGHT.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
