## Description

<div><p>You are given a tree consisting of $n$ vertices. Recall that a tree is an undirected connected acyclic graph. The given tree is rooted at the vertex $1$.</p><p>You have to process $q$ queries. In each query, you are given a vertex of the tree $v$ and an integer $k$.</p><p>To process a query, you may delete any vertices from the tree in any order, except for the root and the vertex $v$. When a vertex is deleted, its children become the children of its parent. You have to process a query in such a way that maximizes the value of $c(v) - m \cdot k$ (where $c(v)$ is the resulting number of children of the vertex $v$, and $m$ is the number of vertices you have deleted). Print the maximum possible value you can obtain.</p><p>The queries are independent: the changes you make to the tree while processing a query don't affect the tree in other queries.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>Then $n-1$ lines follow, the $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$; $x_i \ne y_i$)&nbsp;— the endpoints of the $i$-th edge. These edges form a tree.</p><p>The next line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Then $q$ lines follow, the $j$-th of them contains two integers $v_j$ and $k_j$ ($1 \le v_j \le n$; $0 \le k_j \le 2 \cdot 10^5$)&nbsp;— the parameters of the $j$-th query.</p></div><div class="output-specification"><p>For each query, print one integer&nbsp;— the maximum value of $c(v) - m \cdot k$ you can achieve.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>Then $n-1$ lines follow, the $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$; $x_i \ne y_i$)&nbsp;— the endpoints of the $i$-th edge. These edges form a tree.</p><p>The next line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Then $q$ lines follow, the $j$-th of them contains two integers $v_j$ and $k_j$ ($1 \le v_j \le n$; $0 \le k_j \le 2 \cdot 10^5$)&nbsp;— the parameters of the $j$-th query.</p>

## Output

<p>For each query, print one integer&nbsp;— the maximum value of $c(v) - m \cdot k$ you can achieve.</p>





```input1
8
6 7
3 2
8 3
5 7
7 4
7 1
7 3
6
1 0
1 2
1 3
7 1
5 0
7 200000
```




```output1
5
2
1
4
0
4
```



## Note

<p>The tree in the first example is shown in the following picture:</p><center> <img class="tex-graphics" src="file://4jzJNfI8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Answers to the queries are obtained as follows:</p><ol> <li> $v=1,k=0$: you can delete vertices $7$ and $3$, so the vertex $1$ has $5$ children (vertices $2$, $4$, $5$, $6$, and $8$), and the score is $5 - 2 \cdot 0 = 5$; </li><li> $v=1,k=2$: you can delete the vertex $7$, so the vertex $1$ has $4$ children (vertices $3$, $4$, $5$, and $6$), and the score is $4 - 1 \cdot 2 = 2$. </li><li> $v=1,k=3$: you shouldn't delete any vertices, so the vertex $1$ has only one child (vertex $7$), and the score is $1 - 0 \cdot 3 = 1$; </li><li> $v=7,k=1$: you can delete the vertex $3$, so the vertex $7$ has $5$ children (vertices $2$, $4$, $5$, $6$, and $8$), and the score is $5 - 1 \cdot 1 = 4$; </li><li> $v=5,k=0$: no matter what you do, the vertex $5$ will have no children, so the score is $0$; </li><li> $v=7,k=200000$: you shouldn't delete any vertices, so the vertex $7$ has $4$ children (vertices $3$, $4$, $5$, and $6$), and the score is $4 - 0 \cdot 200000 = 4$. </li></ol>
