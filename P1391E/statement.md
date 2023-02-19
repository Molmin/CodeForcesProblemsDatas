## Description

<div><p>You have a simple and connected undirected graph consisting of $n$ nodes and $m$ edges.</p><p>Consider any way to pair some subset of these $n$ nodes such that no node is present in more than one pair. </p><p>This pairing is <span class="tex-font-style-bf">valid</span> if for every pair of pairs, the induced subgraph containing all $4$ nodes, two from each pair, has at most $2$ edges (out of the $6$ possible edges). More formally, for any two pairs, $(a,b)$ and $(c,d)$, the induced subgraph with nodes $\{a,b,c,d\}$ should have at most $2$ edges. </p><p>Please note that the subgraph induced by a set of nodes contains nodes only from this set and edges which have both of its end points in this set.</p><p>Now, do one of the following: </p><ul> <li> Find a simple path consisting of at least <span>$\lceil \frac{n}{2} \rceil$</span> nodes. Here, a path is called simple if it does not visit any node multiple times. </li><li> Find a valid pairing in which at least <span>$\lceil \frac{n}{2} \rceil$</span> nodes are paired. </li></ul><p>It can be shown that it is possible to find at least one of the two in every graph satisfying constraints from the statement. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains $2$ integers $n, m$ ($2 \le n \le 5\cdot 10^5$, $1 \le m \le 10^6$), denoting the number of nodes and edges, respectively. </p><p>The next $m$ lines each contain $2$ integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$), denoting that there is an undirected edge between nodes $u$ and $v$ in the given graph.</p><p>It is guaranteed that the given graph is connected, and simple &nbsp;— it does not contain multiple edges between the same pair of nodes, nor does it have any self-loops. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5\cdot 10^5$.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, the output format is as follows. </p><p>If you have found a pairing, in the first line output "PAIRING" (without quotes). </p><ul> <li> Then, output $k$ ($\lceil \frac{n}{2} \rceil \le 2\cdot k \le n$), the number of pairs in your pairing. </li><li> Then, in each of the next $k$ lines, output $2$ integers $a$ and $b$ &nbsp;— denoting that $a$ and $b$ are paired with each other. <span class="tex-font-style-bf">Note that the graph does not have to have an edge between $a$ and $b$!</span></li><li> This pairing has to be valid, and every node has to be a part of at most $1$ pair. </li></ul><p>Otherwise, in the first line output "PATH" (without quotes). </p><ul><li> Then, output $k$ ($\lceil \frac{n}{2} \rceil \le k \le n$), the number of nodes in your path. </li><li> Then, in the second line, output $k$ integers, $v_1, v_2, \ldots, v_k$, in the order in which they appear on the path. Formally, $v_i$ and $v_{i+1}$ should have an edge between them for every $i$ ($1 \le i &lt; k$).</li><li> This path has to be simple, meaning no node should appear more than once. </li></ul></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains $2$ integers $n, m$ ($2 \le n \le 5\cdot 10^5$, $1 \le m \le 10^6$), denoting the number of nodes and edges, respectively. </p><p>The next $m$ lines each contain $2$ integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$), denoting that there is an undirected edge between nodes $u$ and $v$ in the given graph.</p><p>It is guaranteed that the given graph is connected, and simple &nbsp;— it does not contain multiple edges between the same pair of nodes, nor does it have any self-loops. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5\cdot 10^5$.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, the output format is as follows. </p><p>If you have found a pairing, in the first line output "PAIRING" (without quotes). </p><ul> <li> Then, output $k$ ($\lceil \frac{n}{2} \rceil \le 2\cdot k \le n$), the number of pairs in your pairing. </li><li> Then, in each of the next $k$ lines, output $2$ integers $a$ and $b$ &nbsp;— denoting that $a$ and $b$ are paired with each other. <span class="tex-font-style-bf">Note that the graph does not have to have an edge between $a$ and $b$!</span></li><li> This pairing has to be valid, and every node has to be a part of at most $1$ pair. </li></ul><p>Otherwise, in the first line output "PATH" (without quotes). </p><ul><li> Then, output $k$ ($\lceil \frac{n}{2} \rceil \le k \le n$), the number of nodes in your path. </li><li> Then, in the second line, output $k$ integers, $v_1, v_2, \ldots, v_k$, in the order in which they appear on the path. Formally, $v_i$ and $v_{i+1}$ should have an edge between them for every $i$ ($1 \le i &lt; k$).</li><li> This path has to be simple, meaning no node should appear more than once. </li></ul>





```input1
4
6 5
1 4
2 5
3 6
1 5
3 5
6 5
1 4
2 5
3 6
1 5
3 5
12 14
1 2
2 3
3 4
4 1
1 5
1 12
2 6
2 7
3 8
3 9
4 10
4 11
2 4
1 3
12 14
1 2
2 3
3 4
4 1
1 5
1 12
2 6
2 7
3 8
3 9
4 10
4 11
2 4
1 3
```




```output1
PATH
4 
1 5 3 6
PAIRING
2
1 6
2 4
PAIRING
3
1 8
2 5
4 10
PAIRING
4
1 7
2 9
3 11
4 5
```



## Note

<p>The path outputted in the first case is the following. </p><center> <img class="tex-graphics" src="file://b8EKjFm1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The pairing outputted in the second case is the following. </p><center> <img class="tex-graphics" src="file://kxAjZ15R.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Here is an <span class="tex-font-style-bf">invalid</span> pairing for the same graph &nbsp;— the subgraph $\{1,3,4,5\}$ has $3$ edges. </p><center> <img class="tex-graphics" src="file://nlKGR7M4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Here is the pairing outputted in the third case. </p><center> <img class="tex-graphics" src="file://8g0dA8OX.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It's valid because&nbsp;— </p><ul> <li> The subgraph $\{1,8,2,5\}$ has edges ($1$,$2$) and ($1$,$5$). </li><li> The subgraph $\{1,8,4,10\}$ has edges ($1$,$4$) and ($4$,$10$). </li><li> The subgraph $\{4,10,2,5\}$ has edges ($2$,$4$) and ($4$,$10$). </li></ul><p>Here is the pairing outputted in the fourth case. </p><center> <img class="tex-graphics" src="file://RGrdoixW.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
