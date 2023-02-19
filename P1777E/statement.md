## Description

<div><p>You will be given a weighted directed graph of $n$ nodes and $m$ directed edges, where the $i$-th edge has a weight of $w_i$ ($1 \le i \le m$).</p><p>You need to reverse some edges of this graph so that there is at least one node in the graph from which every other node is reachable. The cost of these reversals is equal to the maximum weight of all reversed edges. If no edge reversal is required, assume the cost to be $0$.</p><p>It is guaranteed that no self-loop or duplicate edge exists.</p><p>Find the minimum cost required for completing the task. If there is no solution, print a single integer $-1$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>Each test case begins with a line containing two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m \le 2 \cdot 10^5$) — the number of nodes in the graph and the number of edges in the graph.</p><p>The next $m$ lines of each test case contain $3$ integers each — $u$, $v$, $w$ ($1 \le u, v \le n$, $1 \le w \le 10^9$), indicating an edge from $u$ to $v$ with a weight of $w$. It is guaranteed that no edge connects a vertex to itself, and no pair of edges share the same origin and destination simultaneously.</p><p>It is guaranteed that the sum of $n$ and the sum of $m$ over all test cases do not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the minimum cost. If there is no solution, print $-1$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>Each test case begins with a line containing two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m \le 2 \cdot 10^5$) — the number of nodes in the graph and the number of edges in the graph.</p><p>The next $m$ lines of each test case contain $3$ integers each — $u$, $v$, $w$ ($1 \le u, v \le n$, $1 \le w \le 10^9$), indicating an edge from $u$ to $v$ with a weight of $w$. It is guaranteed that no edge connects a vertex to itself, and no pair of edges share the same origin and destination simultaneously.</p><p>It is guaranteed that the sum of $n$ and the sum of $m$ over all test cases do not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the minimum cost. If there is no solution, print $-1$.</p>





```input1|2,3,9,10,11,12,13,14
4
2 1
1 2 3
5 4
1 2 10
2 3 10
3 1 10
4 5 10
4 5
1 2 10000
2 3 20000
1 3 30000
4 2 500
4 3 20
4 5
1 2 10000
2 3 20000
1 3 30000
4 2 5
4 3 20
```




```output1
0
-1
20
5
```



## Note

<p>In the first test case, an edge exists from $1$ to $2$, so all nodes are reachable (from $1$).</p><p>In the second test case, no nodes are reachable from any node no matter what edges we reverse, so the answer is $-1$.</p><p>In the third test case, reversing the $4$-th or $5$-th edge allows all nodes to be reachable from $1$. We choose the $5$-th edge here because its weight is smaller.</p>
