## Description

<div><p><span class="tex-font-style-it">Byteland is a beautiful land known because of its beautiful trees.</span></p><p>Misha has found a binary tree with $n$ vertices, numbered from $1$ to $n$. A binary tree is an acyclic connected bidirectional graph containing $n$ vertices and $n - 1$ edges. Each vertex has a degree at most $3$, whereas the root is the vertex with the number $1$ and it has a degree at most $2$.</p><p>Unfortunately, the root got infected.</p><p>The following process happens $n$ times:</p><ul> <li> Misha either chooses a non-infected (and not deleted) vertex and deletes it with all edges which have an end in this vertex or just does nothing. </li><li> Then, the infection spreads to each vertex that is connected by an edge to an already infected vertex (all already infected vertices remain infected). </li></ul><p>As Misha does not have much time to think, please tell him what is the maximum number of vertices he can save from the infection (note that deleted vertices are not counted as saved).</p></div><div class="input-specification"><p>There are several test cases in the input data. The first line contains a single integer $t$ ($1\leq t\leq 5000$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains one integer $n$ ($2\leq n\leq 3\cdot 10^5$)&nbsp;— the number of vertices of the tree. </p><p>The $i$-th of the following $n-1$ lines in the test case contains two positive integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$), meaning that there exists an edge between them in the graph. </p><p>It is guaranteed that the graph is a binary tree rooted at $1$. It is also guaranteed that the sum of $n$ over all test cases won't exceed $3\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum number of vertices Misha can save.</p></div>

## Input

<p>There are several test cases in the input data. The first line contains a single integer $t$ ($1\leq t\leq 5000$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains one integer $n$ ($2\leq n\leq 3\cdot 10^5$)&nbsp;— the number of vertices of the tree. </p><p>The $i$-th of the following $n-1$ lines in the test case contains two positive integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$), meaning that there exists an edge between them in the graph. </p><p>It is guaranteed that the graph is a binary tree rooted at $1$. It is also guaranteed that the sum of $n$ over all test cases won't exceed $3\cdot 10^5$.</p>

## Output

<p>For each test case, output the maximum number of vertices Misha can save.</p>





```input1
4
2
1 2
4
1 2
2 3
2 4
7
1 2
1 5
2 3
2 4
5 6
5 7
15
1 2
2 3
3 4
4 5
4 6
3 7
2 8
1 9
9 10
9 11
10 12
10 13
11 14
11 15
```




```output1
0
2
2
10
```



## Note

<p>In the first test case, the only possible action is to delete vertex $2$, after which we save $0$ vertices in total.</p><p>In the second test case, if we delete vertex $2$, we can save vertices $3$ and $4$.</p><center> <img class="tex-graphics" src="file://zN9MhY2P.png" style="max-width: 100.0%;max-height: 100.0%;">   </center>
