## Description

<div><p>You are given a tree of $n$ vertices numbered from $1$ to $n$, with edges numbered from $1$ to $n-1$. A tree is a connected undirected graph without cycles. You have to assign integer weights to each edge of the tree, such that the resultant graph is a prime tree.</p><p>A <span class="tex-font-style-it">prime tree</span> is a tree where the weight of every path consisting of <span class="tex-font-style-bf">one or two edges</span> is prime. A path should not visit any vertex twice. The weight of a path is the sum of edge weights on that path.</p><p>Consider the graph below. It is a prime tree as the weight of every path of two or less edges is prime. For example, the following path of two edges: $2 \to 1 \to 3$ has a weight of $11 + 2 = 13$, which is prime. Similarly, the path of one edge: $4 \to 3$ has a weight of $5$, which is also prime.</p><center> <img class="tex-graphics" src="file://DT28sWat.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Print <span class="tex-font-style-bf">any</span> valid assignment of weights such that the resultant tree is a prime tree. If there is no such assignment, then print $-1$. It can be proven that if a valid assignment exists, one exists with weights between $1$ and $10^5$ as well.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 10^5$)&nbsp;— the number of vertices in the tree.</p><p>Then, $n-1$ lines follow. The $i$-th line contains two integers $u$ and $v$ ($1 \leq u, v \leq n$) denoting that edge number $i$ is between vertices $u$ and $v$. It is guaranteed that the edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, if a valid assignment exists, then print a single line containing $n-1$ integers $a_1, a_2, \dots, a_{n-1}$ ($1 \leq a_i \le 10^5$), where $a_i$ denotes the weight assigned to the edge numbered $i$. Otherwise, print $-1$.</p><p>If there are multiple solutions, you may print any.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 10^5$)&nbsp;— the number of vertices in the tree.</p><p>Then, $n-1$ lines follow. The $i$-th line contains two integers $u$ and $v$ ($1 \leq u, v \leq n$) denoting that edge number $i$ is between vertices $u$ and $v$. It is guaranteed that the edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, if a valid assignment exists, then print a single line containing $n-1$ integers $a_1, a_2, \dots, a_{n-1}$ ($1 \leq a_i \le 10^5$), where $a_i$ denotes the weight assigned to the edge numbered $i$. Otherwise, print $-1$.</p><p>If there are multiple solutions, you may print any.</p>





```input1
3
2
1 2
4
1 3
4 3
2 1
7
1 2
1 3
3 4
3 5
6 2
7 2
```




```output1
17
2 5 11
-1
```



## Note

<p>For the first test case, there are only two paths having one edge each: $1 \to 2$ and $2 \to 1$, both having a weight of $17$, which is prime.</p><center> <img class="tex-graphics" src="file://w2jGhjJL.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The second test case is described in the statement.</p><p>It can be proven that no such assignment exists for the third test case.</p>
