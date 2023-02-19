## Description

<div><p>You are given a connected undirected graph consisting of $n$ vertices and $m$ edges. The weight of the $i$-th edge is $i$.</p><p>Here is a wrong algorithm of finding a <a href="https://en.wikipedia.org/wiki/Minimum_spanning_tree">minimum spanning tree</a> (MST) of a graph:</p><pre class="verbatim"><br>vis := an array of length n<br>s := a set of edges<br><br>function dfs(u):<br>    vis[u] := true<br>    iterate through each edge (u, v) in the order from smallest to largest edge weight<br>        if vis[v] = false<br>            add edge (u, v) into the set (s)<br>            dfs(v)<br><br>function findMST(u):<br>    reset all elements of (vis) to false<br>    reset the edge set (s) to empty<br>    dfs(u)<br>    return the edge set (s)<br></pre><p>Each of the calls <span class="tex-font-style-tt">findMST(1)</span>, <span class="tex-font-style-tt">findMST(2)</span>, ..., <span class="tex-font-style-tt">findMST(n)</span> gives you a spanning tree of the graph. Determine which of these trees are minimum spanning trees.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$, $m$ ($2\le n\le 10^5$, $n-1\le m\le 2\cdot 10^5$)&nbsp;— the number of vertices and the number of edges in the graph.</p><p>Each of the following $m$ lines contains two integers $u_i$ and $v_i$ ($1\le u_i, v_i\le n$, $u_i\ne v_i$), describing an undirected edge $(u_i,v_i)$ in the graph. The $i$-th edge in the input has weight $i$.</p><p>It is guaranteed that the graph is connected and there is at most one edge between any pair of vertices.</p></div><div class="output-specification"><p>You need to output a binary string $s$, where $s_i=1$ if <span class="tex-font-style-tt">findMST(i)</span> creates an MST, and $s_i = 0$ otherwise.</p></div>

## Input

<p>The first line of the input contains two integers $n$, $m$ ($2\le n\le 10^5$, $n-1\le m\le 2\cdot 10^5$)&nbsp;— the number of vertices and the number of edges in the graph.</p><p>Each of the following $m$ lines contains two integers $u_i$ and $v_i$ ($1\le u_i, v_i\le n$, $u_i\ne v_i$), describing an undirected edge $(u_i,v_i)$ in the graph. The $i$-th edge in the input has weight $i$.</p><p>It is guaranteed that the graph is connected and there is at most one edge between any pair of vertices.</p>

## Output

<p>You need to output a binary string $s$, where $s_i=1$ if <span class="tex-font-style-tt">findMST(i)</span> creates an MST, and $s_i = 0$ otherwise.</p>





```input1
5 5
1 2
3 5
1 3
3 2
4 2
```




```input2
10 11
1 2
2 5
3 4
4 2
8 1
4 5
10 5
9 5
8 2
5 7
4 6
```




```output1
01111
```




```output2
0011111011
```



## Note

<p>Here is the graph given in the first example.</p><center> <img class="tex-graphics" src="file://hkJ7fOp4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There is only one minimum spanning tree in this graph. A minimum spanning tree is $(1,2),(3,5),(1,3),(2,4)$ which has weight $1+2+3+5=11$.</p><p>Here is a part of the process of calling <span class="tex-font-style-tt">findMST(1)</span>:</p><ul> <li> reset the array <span class="tex-font-style-tt">vis</span> and the edge set <span class="tex-font-style-tt">s</span>; </li><li> calling <span class="tex-font-style-tt">dfs(1)</span>; </li><li> <span class="tex-font-style-tt">vis[1] := true</span>; </li><li> iterate through each edge $(1,2),(1,3)$; </li><li> add edge $(1,2)$ into the edge set <span class="tex-font-style-tt">s</span>, calling <span class="tex-font-style-tt">dfs(2)</span>: <ul> <li> <span class="tex-font-style-tt">vis[2] := true</span> </li><li> iterate through each edge $(2,1),(2,3),(2,4)$; </li><li> because <span class="tex-font-style-tt">vis[1] = true</span>, ignore the edge $(2,1)$; </li><li> add edge $(2,3)$ into the edge set <span class="tex-font-style-tt">s</span>, calling <span class="tex-font-style-tt">dfs(3)</span>: <ul> <li> ... </li></ul> </li></ul> </li></ul><p>In the end, it will select edges $(1,2),(2,3),(3,5),(2,4)$ with total weight $1+4+2+5=12&gt;11$, so <span class="tex-font-style-tt">findMST(1)</span> does not find a minimum spanning tree.</p><p>It can be shown that the other trees are all MSTs, so the answer is <span class="tex-font-style-tt">01111</span>.</p>
