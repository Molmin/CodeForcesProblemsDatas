## Description

<div><p>You are given a tree consisting of $n$ vertices. Initially, each vertex has a value $0$.</p><p>You need to perform $m$ queries of two types: </p><ol> <li> You are given a vertex index $v$. Print the value of the vertex $v$. </li><li> You are given two vertex indices $u$ and $v$ and values $k$ and $d$ ($d \le 20$). You need to add $k$ to the value of each vertex such that the distance from that vertex to the path from $u$ to $v$ is less than or equal to $d$. </li></ol><p>The <span class="tex-font-style-it">distance</span> between two vertices $x$ and $y$ is equal to the number of <span class="tex-font-style-it">edges</span> on the path from $x$ to $y$. For example, the distance from $x$ to $x$ itself is equal to $0$.</p><p>The distance from the vertex $v$ to some path from $x$ to $y$ is equal to the minimum among distances from $v$ to any vertex on the path from $x$ to $y$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>Next $n - 1$ lines contain the edges of the tree&nbsp;— one per line. Each line contains two integers $u$ and $v$ ($1 \le u, v \le n$; $u \neq v$) representing one edge of the tree. It's guaranteed that the given edges form a tree.</p><p>The next line contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Next $m$ lines contain the queries&nbsp;— one per line. Each query has one of the following two types: </p><ul> <li> $1$ $v$ ($1 \le v \le n$)&nbsp;— the query of the first type; </li><li> $2$ $u$ $v$ $k$ $d$ ($1 \le u, v \le n$; $1 \le k \le 1000$; $0 \le d \le 20$)&nbsp;— the query of the second type. </li></ul><p>Additional constraint on the input: there is at least one query of the first type.</p></div><div class="output-specification"><p>For each query of the first type, print the value of the corresponding vertex.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of vertices in the tree.</p><p>Next $n - 1$ lines contain the edges of the tree&nbsp;— one per line. Each line contains two integers $u$ and $v$ ($1 \le u, v \le n$; $u \neq v$) representing one edge of the tree. It's guaranteed that the given edges form a tree.</p><p>The next line contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Next $m$ lines contain the queries&nbsp;— one per line. Each query has one of the following two types: </p><ul> <li> $1$ $v$ ($1 \le v \le n$)&nbsp;— the query of the first type; </li><li> $2$ $u$ $v$ $k$ $d$ ($1 \le u, v \le n$; $1 \le k \le 1000$; $0 \le d \le 20$)&nbsp;— the query of the second type. </li></ul><p>Additional constraint on the input: there is at least one query of the first type.</p>

## Output

<p>For each query of the first type, print the value of the corresponding vertex.</p>





```input1
6
1 2
1 3
4 2
5 2
3 6
14
2 4 5 10 2
1 3
1 6
2 1 1 10 20
2 6 6 10 20
1 3
2 3 2 10 0
2 5 2 10 1
1 1
1 2
1 3
1 4
1 5
1 6
```




```output1
10
0
30
50
50
40
40
40
20
```



## Note

<p>The tree from the first example: </p><center> <img class="tex-graphics" src="file://NiwmLxVH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> Some query explanations: <ul> <li> "$2$ $4$ $5$ $10$ $2$": affected vertices are $\{4, 2, 5, 1, 3\}$; </li><li> "$2$ $1$ $1$ $10$ $20$" and "$2$ $6$ $6$ $10$ $20$": all vertices are affected, since distance to $1$ ($6$) is less that $20$ for any vertex; </li><li> "$2$ $3$ $2$ $10$ $0$": affected vertices are $\{3, 1, 2\}$; </li><li> "$2$ $5$ $2$ $10$ $1$": affected vertices are $\{5, 2, 4, 1\}$. </li></ul>
