## Description

<div><p>You are given a tree of $n$ vertices and $n - 1$ edges. The $i$-th vertex has an initial weight $a_i$.</p><p>Let the <span class="tex-font-style-it">distance</span> $d_v(u)$ from vertex $v$ to vertex $u$ be the number of edges on the path from $v$ to $u$. Note that $d_v(u) = d_u(v)$ and $d_v(v) = 0$.</p><p>Let the <span class="tex-font-style-it">weighted</span> distance $w_v(u)$ from $v$ to $u$ be $w_v(u) = d_v(u) + a_u$. Note that $w_v(v) = a_v$ and $w_v(u) \neq w_u(v)$ if $a_u \neq a_v$.</p><p>Analogically to usual distance, let's define the <span class="tex-font-style-it">eccentricity</span> $e(v)$ of vertex $v$ as the greatest weighted distance from $v$ to any other vertex (including $v$ itself), or $e(v) = \max\limits_{1 \le u \le n}{w_v(u)}$.</p><p>Finally, let's define the <span class="tex-font-style-it">radius</span> $r$ of the tree as the minimum eccentricity of any vertex, or $r = \min\limits_{1 \le v \le n}{e(v)}$.</p><p>You need to perform $m$ queries of the following form: </p><ul> <li> $v_j$ $x_j$&nbsp;— assign $a_{v_j} = x_j$. </li></ul><p>After performing each query, print the radius $r$ of the current tree.</p></div><div class="input-specification"><p>The first line contains the single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>The second line contains $n$ integers $a_1, \dots, a_n$ ($0 \le a_i \le 10^6$)&nbsp;— the initial weights of vertices.</p><p>Next $n - 1$ lines contain edges of tree. The $i$-th line contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$; $u_i \neq v_i$)&nbsp;— the corresponding edge. The given edges form a tree.</p><p>The next line contains the single integer $m$ ($1 \le m \le 10^5$)&nbsp;— the number of queries.</p><p>Next $m$ lines contain queries&nbsp;— one query per line. The $j$-th query contains two integers $v_j$ and $x_j$ ($1 \le v_j \le n$; $0 \le x_j \le 10^6$)&nbsp;— a vertex and it's new weight.</p></div><div class="output-specification"><p>Print $m$ integers&nbsp;— the radius $r$ of the tree after performing each query.</p></div>

## Input

<p>The first line contains the single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>The second line contains $n$ integers $a_1, \dots, a_n$ ($0 \le a_i \le 10^6$)&nbsp;— the initial weights of vertices.</p><p>Next $n - 1$ lines contain edges of tree. The $i$-th line contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$; $u_i \neq v_i$)&nbsp;— the corresponding edge. The given edges form a tree.</p><p>The next line contains the single integer $m$ ($1 \le m \le 10^5$)&nbsp;— the number of queries.</p><p>Next $m$ lines contain queries&nbsp;— one query per line. The $j$-th query contains two integers $v_j$ and $x_j$ ($1 \le v_j \le n$; $0 \le x_j \le 10^6$)&nbsp;— a vertex and it's new weight.</p>

## Output

<p>Print $m$ integers&nbsp;— the radius $r$ of the tree after performing each query.</p>





```input1
6
1 3 3 7 0 1
2 1
1 3
1 4
5 4
4 6
5
4 7
4 0
2 5
5 10
5 5
```




```output1
7
4
5
10
7
```



## Note

<p>After the first query, you have the following tree: </p><center> <img class="tex-graphics" src="file://NkIYAWSc.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> The marked vertex in the picture is the vertex with minimum $e(v)$, or $r = e(4) = 7$. The eccentricities of the other vertices are the following: $e(1) = 8$, $e(2) = 9$, $e(3) = 9$, $e(5) = 8$, $e(6) = 8$.<p>The tree after the second query: </p><center> <img class="tex-graphics" src="file://9LN38oNZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> The radius $r = e(1) = 4$.<p>After the third query, the radius $r = e(2) = 5$: </p><center> <img class="tex-graphics" src="file://1eY1gpbJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
