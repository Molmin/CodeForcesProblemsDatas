## Description

<div><p>You are given an undirected graph with $n$ vertices and $m$ edges. Also, you are given an integer $k$.</p><p>Find either a clique of size $k$ or a non-empty subset of vertices such that each vertex of this subset has at least $k$ neighbors in the subset. If there are no such cliques and subsets report about it.</p><p>A subset of vertices is called a clique of size $k$ if its size is $k$ and there exists an edge between every two vertices from the subset. A vertex is called a neighbor of the other vertex if there exists an edge between them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;— the number of test cases. The next lines contain descriptions of test cases.</p><p>The first line of the description of each test case contains three integers $n$, $m$, $k$ ($1 \leq n, m, k \leq 10^5$, $k \leq n$).</p><p>Each of the next $m$ lines contains two integers $u, v$ $(1 \leq u, v \leq n, u \neq v)$, denoting an edge between vertices $u$ and $v$.</p><p>It is guaranteed that there are no self-loops or multiple edges. It is guaranteed that the sum of $n$ for all test cases and the sum of $m$ for all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case: </p><p>If you found a subset of vertices such that each vertex of this subset has at least $k$ neighbors in the subset in the first line output $1$ and the size of the subset. On the second line output the vertices of the subset in any order.</p><p>If you found a clique of size $k$ then in the first line output $2$ and in the second line output the vertices of the clique in any order.</p><p>If there are no required subsets and cliques print $-1$.</p><p>If there exists multiple possible answers you can print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;— the number of test cases. The next lines contain descriptions of test cases.</p><p>The first line of the description of each test case contains three integers $n$, $m$, $k$ ($1 \leq n, m, k \leq 10^5$, $k \leq n$).</p><p>Each of the next $m$ lines contains two integers $u, v$ $(1 \leq u, v \leq n, u \neq v)$, denoting an edge between vertices $u$ and $v$.</p><p>It is guaranteed that there are no self-loops or multiple edges. It is guaranteed that the sum of $n$ for all test cases and the sum of $m$ for all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case: </p><p>If you found a subset of vertices such that each vertex of this subset has at least $k$ neighbors in the subset in the first line output $1$ and the size of the subset. On the second line output the vertices of the subset in any order.</p><p>If you found a clique of size $k$ then in the first line output $2$ and in the second line output the vertices of the clique in any order.</p><p>If there are no required subsets and cliques print $-1$.</p><p>If there exists multiple possible answers you can print any of them.</p>





```input1
3
5 9 4
1 2
1 3
1 4
1 5
2 3
2 4
2 5
3 4
3 5
10 15 3
1 2
2 3
3 4
4 5
5 1
1 7
2 8
3 9
4 10
5 6
7 10
10 8
8 6
6 9
9 7
4 5 4
1 2
2 3
3 4
4 1
1 3
```




```output1
2
4 1 2 3 
1 10
1 2 3 4 5 6 7 8 9 10 
-1
```



## Note

<p>In the first test case: the subset $\{1, 2, 3, 4\}$ is a clique of size $4$.</p><p>In the second test case: degree of each vertex in the original graph is at least $3$. So the set of all vertices is a correct answer.</p><p>In the third test case: there are no cliques of size $4$ or required subsets, so the answer is $-1$.</p>
