## Description

<div><p>Abendsen assigned a mission to Juliana. In this mission, Juliana has a rooted tree with $n$ vertices. Vertex number $1$ is the root of this tree. Each vertex can be either black or white. At first, all vertices are white. Juliana is asked to process $q$ queries. Each query is one of three types:</p><ol> <li> If vertex $v$ is white, mark it as black; otherwise, perform this operation on all direct sons of $v$ instead. </li><li> Mark all vertices in the subtree of $v$ (including $v$) as white. </li><li> Find the color of the $i$-th vertex. </li></ol><center> <img class="tex-graphics" height="212px" src="file://TBMc0nw1.png" style="max-width: 100.0%;max-height: 100.0%;" width="510px"> <span class="tex-font-size-small">An example of operation "<span class="tex-font-style-tt">1 1</span>" (corresponds to the first example test). The vertices $1$ and $2$ are already black, so the operation goes to their sons instead.</span> </center><p>Can you help Juliana to process all these queries?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($2\leq n\leq 10^5$, $1\leq q\leq 10^5$)&nbsp;— the number of vertices and the number of queries.</p><p>The second line contains $n-1$ integers $p_2, p_3, \ldots, p_n$ ($1\leq p_i&lt;i$), where $p_i$ means that there is an edge between vertices $i$ and $p_i$. </p><p>Each of the next $q$ lines contains two integers $t_i$ and $v_i$ ($1\leq t_i\leq 3$, $1\leq v_i\leq n$)&nbsp;— the type of the $i$-th query and the vertex of the $i$-th query.</p><p>It is guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>For each query of type $3$, print "<span class="tex-font-style-tt">black</span>" if the vertex is black; otherwise, print "<span class="tex-font-style-tt">white</span>".</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($2\leq n\leq 10^5$, $1\leq q\leq 10^5$)&nbsp;— the number of vertices and the number of queries.</p><p>The second line contains $n-1$ integers $p_2, p_3, \ldots, p_n$ ($1\leq p_i&lt;i$), where $p_i$ means that there is an edge between vertices $i$ and $p_i$. </p><p>Each of the next $q$ lines contains two integers $t_i$ and $v_i$ ($1\leq t_i\leq 3$, $1\leq v_i\leq n$)&nbsp;— the type of the $i$-th query and the vertex of the $i$-th query.</p><p>It is guaranteed that the given graph is a tree.</p>

## Output

<p>For each query of type $3$, print "<span class="tex-font-style-tt">black</span>" if the vertex is black; otherwise, print "<span class="tex-font-style-tt">white</span>".</p>





```input1
8 10
1 2 1 2 5 4 5
1 2
3 2
3 1
1 1
1 1
3 5
3 7
3 4
2 2
3 5

```




```input2
8 11
1 1 2 3 3 6 6
1 1
1 1
1 3
3 2
3 4
3 6
3 7
2 3
1 6
3 7
3 6

```




```output1
black
white
black
white
black
white

```




```output2
black
white
black
white
white
black

```



## Note

<p>The first example is shown on the picture below.</p><center> <img class="tex-graphics" height="321px" src="file://M3jePdSB.png" style="max-width: 100.0%;max-height: 100.0%;" width="605px"> </center><p>The second example is shown on the picture below.</p><center> <img class="tex-graphics" height="265px" src="file://uDz1vEHP.png" style="max-width: 100.0%;max-height: 100.0%;" width="605px"> </center>
