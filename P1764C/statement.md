## Description

<div><p>Doremy's new city is under construction! The city can be regarded as a simple undirected graph with $n$ vertices. The $i$-th vertex has altitude $a_i$. Now Doremy is deciding which pairs of vertices should be connected with edges.</p><p>Due to economic reasons, there should be no self-loops or multiple edges in the graph.</p><p>Due to safety reasons, there should not be <span class="tex-font-style-bf">pairwise distinct</span> vertices $u$, $v$, and $w$ such that $a_u \leq a_v \leq a_w$ and the edges $(u,v)$ and $(v,w)$ exist.</p><p>Under these constraints, Doremy would like to know the maximum possible number of edges in the graph. Can you help her?</p><p>Note that the constructed graph is allowed to be disconnected.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2\cdot 10^5$)&nbsp;— the number of vertices.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1\le a_i\le 10^6$)&nbsp;— the altitudes of each vertex.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum possible number of edges in the graph.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2\cdot 10^5$)&nbsp;— the number of vertices.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1\le a_i\le 10^6$)&nbsp;— the altitudes of each vertex.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the maximum possible number of edges in the graph.</p>





```input1|2,3,6,7
4
4
2 2 3 1
6
5 2 3 1 5 2
12
7 2 4 9 1 4 6 3 7 4 2 3
4
1000000 1000000 1000000 1000000
```




```output1
3
9
35
2
```



## Note

<p>In the first test case, there can only be at most $3$ edges in the graph. A possible construction is to connect $(1,3)$, $(2,3)$, $(3,4)$. In the picture below the red number above node $i$ is $a_i$.</p><p><img class="tex-graphics" src="file://Yxm9FQ5N.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The following list shows all such $u$, $v$, $w$ that the edges $(u,v)$ and $(v,w)$ exist.</p><ul> <li> $u=1$, $v=3$, $w=2$; </li><li> $u=1$, $v=3$, $w=4$; </li><li> $u=2$, $v=3$, $w=1$; </li><li> $u=2$, $v=3$, $w=4$; </li><li> $u=4$, $v=3$, $w=1$; </li><li> $u=4$, $v=3$, $w=2$. </li></ul><p>Another possible construction is to connect $(1,4)$, $(2,4)$, $(3,4)$.</p><p><img class="tex-graphics" src="file://LyfN3pxI.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>An unacceptable construction is to connect $(1,3)$, $(2,3)$, $(2,4)$, $(3,4)$. Because when $u=4$, $v=2$, $w=3$, $a_u\le a_v \le a_w$ holds, and the respective edges exist.</p><p><img class="tex-graphics" src="file://QVdAZZGY.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
