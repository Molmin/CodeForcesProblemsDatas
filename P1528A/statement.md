## Description

<div><p>Parsa has a humongous tree on $n$ vertices.</p><p>On each vertex $v$ he has written two integers $l_v$ and $r_v$.</p><p>To make Parsa's tree look even more majestic, Nima wants to assign a number $a_v$ ($l_v \le a_v \le r_v$) to each vertex $v$ such that the beauty of Parsa's tree is maximized.</p><p>Nima's sense of the beauty is rather bizarre. He defines the beauty of the tree as the sum of $|a_u - a_v|$ over all edges $(u, v)$ of the tree.</p><p>Since Parsa's tree is too large, Nima can't maximize its beauty on his own. Your task is to find the <span class="tex-font-style-bf">maximum</span> possible beauty for Parsa's tree.</p></div><div class="input-specification"><p>The first line contains an integer $t$ $(1\le t\le 250)$ — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2\le n\le 10^5)$ — the number of vertices in Parsa's tree.</p><p>The $i$-th of the following $n$ lines contains two integers $l_i$ and $r_i$ $(1 \le l_i \le r_i \le 10^9)$.</p><p>Each of the next $n-1$ lines contains two integers $u$ and $v$ $(1 \le u , v \le n, u\neq v)$ meaning that there is an edge between the vertices $u$ and $v$ in Parsa's tree.</p><p>It is guaranteed that the given graph is a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print the <span class="tex-font-style-bf">maximum</span> possible beauty for Parsa's tree.</p></div>

## Input

<p>The first line contains an integer $t$ $(1\le t\le 250)$ — the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2\le n\le 10^5)$ — the number of vertices in Parsa's tree.</p><p>The $i$-th of the following $n$ lines contains two integers $l_i$ and $r_i$ $(1 \le l_i \le r_i \le 10^9)$.</p><p>Each of the next $n-1$ lines contains two integers $u$ and $v$ $(1 \le u , v \le n, u\neq v)$ meaning that there is an edge between the vertices $u$ and $v$ in Parsa's tree.</p><p>It is guaranteed that the given graph is a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print the <span class="tex-font-style-bf">maximum</span> possible beauty for Parsa's tree.</p>





```input1
3
2
1 6
3 8
1 2
3
1 3
4 6
7 9
1 2
2 3
6
3 14
12 20
12 19
2 12
10 17
3 17
3 2
6 5
1 5
2 6
4 6
```




```output1
7
8
62
```



## Note

<p>The trees in the example:</p><center> <img class="tex-graphics" src="file://UJrYAUVV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the first test case, one possible assignment is $a = \{1, 8\}$ which results in $|1 - 8| = 7$.</p><p>In the second test case, one of the possible assignments is $a = \{1, 5, 9\}$ which results in a beauty of $|1 - 5| + |5 - 9| = 8$</p>
