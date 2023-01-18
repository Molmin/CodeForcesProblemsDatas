## Description

<div><p>You are given three integers $n$, $d$ and $k$.</p><p>Your task is to construct an undirected tree on $n$ vertices with diameter $d$ and degree of each vertex at most $k$, or say that it is impossible.</p><p>An undirected tree is a connected undirected graph with $n - 1$ edges.</p><p>Diameter of a tree is the maximum length of a simple path (a path in which each vertex appears at most once) between all pairs of vertices of this tree.</p><p>Degree of a vertex is the number of edges incident to this vertex (i.e. for a vertex $u$ it is the number of edges $(u, v)$ that belong to the tree, where $v$ is any other vertex of a tree).</p></div><div class="input-specification"><p>The first line of the input contains three integers $n$, $d$ and $k$ ($1 \le n, d, k \le 4 \cdot 10^5$).</p></div><div class="output-specification"><p>If there is no tree satisfying the conditions above, print only one word "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise in the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes), and then print $n - 1$ lines describing edges of a tree satisfying the conditions above. Vertices of the tree must be numbered from $1$ to $n$. You can print edges and vertices connected by an edge in any order. If there are multiple answers, print any of them.1</p></div>

## Input

<p>The first line of the input contains three integers $n$, $d$ and $k$ ($1 \le n, d, k \le 4 \cdot 10^5$).</p>

## Output

<p>If there is no tree satisfying the conditions above, print only one word "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise in the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes), and then print $n - 1$ lines describing edges of a tree satisfying the conditions above. Vertices of the tree must be numbered from $1$ to $n$. You can print edges and vertices connected by an edge in any order. If there are multiple answers, print any of them.1</p>





```input1
6 3 3

```




```input2
6 2 3

```




```input3
10 4 3

```




```input4
8 5 3

```




```output1
YES
3 1
4 1
1 2
5 2
2 6

```




```output2
NO

```




```output3
YES
2 9
2 10
10 3
3 1
6 10
8 2
4 3
5 6
6 7

```




```output4
YES
2 5
7 2
3 7
3 1
1 6
8 7
4 3

```


