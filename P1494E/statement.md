## Description

<div><p>You are given a directed graph consisting of $n$ vertices. Each directed edge (or arc) labeled with a single character. Initially, the graph is empty.</p><p>You should process $m$ queries with it. Each query is one of three types: </p><ul> <li> "<span class="tex-font-style-tt">$+$ $u$ $v$ $c$</span>"&nbsp;— add arc from $u$ to $v$ with label $c$. It's guaranteed that there is no arc $(u, v)$ in the graph at this moment; </li><li> "<span class="tex-font-style-tt">$-$ $u$ $v$</span>"&nbsp;— erase arc from $u$ to $v$. It's guaranteed that the graph contains arc $(u, v)$ at this moment; </li><li> "<span class="tex-font-style-tt">$?$ $k$</span>"&nbsp;— find the sequence of $k$ vertices $v_1, v_2, \dots, v_k$ such that there exist both routes $v_1 \to v_2 \to \dots \to v_k$ and $v_k \to v_{k - 1} \to \dots \to v_1$ and if you write down characters along both routes you'll get the same string. You can visit the same vertices any number of times. </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$; $1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of vertices in the graph and the number of queries.</p><p>The next $m$ lines contain queries&nbsp;— one per line. Each query is one of three types: </p><ul> <li> "<span class="tex-font-style-tt">$+$ $u$ $v$ $c$</span>" ($1 \le u, v \le n$; $u \neq v$; $c$ is a lowercase Latin letter); </li><li> "<span class="tex-font-style-tt">$-$ $u$ $v$</span>" ($1 \le u, v \le n$; $u \neq v$); </li><li> "<span class="tex-font-style-tt">$?$ $k$</span>" ($2 \le k \le 10^5$). </li></ul><p>It's guaranteed that you don't add multiple edges and erase only existing edges. Also, there is at least one query of the third type.</p></div><div class="output-specification"><p>For each query of the third type, print <span class="tex-font-style-tt">YES</span> if there exist the sequence $v_1, v_2, \dots, v_k$ described above, or <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$; $1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of vertices in the graph and the number of queries.</p><p>The next $m$ lines contain queries&nbsp;— one per line. Each query is one of three types: </p><ul> <li> "<span class="tex-font-style-tt">$+$ $u$ $v$ $c$</span>" ($1 \le u, v \le n$; $u \neq v$; $c$ is a lowercase Latin letter); </li><li> "<span class="tex-font-style-tt">$-$ $u$ $v$</span>" ($1 \le u, v \le n$; $u \neq v$); </li><li> "<span class="tex-font-style-tt">$?$ $k$</span>" ($2 \le k \le 10^5$). </li></ul><p>It's guaranteed that you don't add multiple edges and erase only existing edges. Also, there is at least one query of the third type.</p>

## Output

<p>For each query of the third type, print <span class="tex-font-style-tt">YES</span> if there exist the sequence $v_1, v_2, \dots, v_k$ described above, or <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1
3 11
+ 1 2 a
+ 2 3 b
+ 3 2 a
+ 2 1 b
? 3
? 2
- 2 1
- 3 2
+ 2 1 c
+ 3 2 d
? 5
```




```output1
YES
NO
YES
```



## Note

<p>In the first query of the third type $k = 3$, we can, for example, choose a sequence $[1, 2, 3]$, since $1 \xrightarrow{\text{a}} 2 \xrightarrow{\text{b}} 3$ and $3 \xrightarrow{\text{a}} 2 \xrightarrow{\text{b}} 1$.</p><p>In the second query of the third type $k = 2$, and we can't find sequence $p_1, p_2$ such that arcs $(p_1, p_2)$ and $(p_2, p_1)$ have the same characters.</p><p>In the third query of the third type, we can, for example, choose a sequence $[1, 2, 3, 2, 1]$, where $1 \xrightarrow{\text{a}} 2 \xrightarrow{\text{b}} 3 \xrightarrow{\text{d}} 2 \xrightarrow{\text{c}} 1$.</p>
