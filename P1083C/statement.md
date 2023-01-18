## Description

<div><p>Once Grisha found a tree (connected graph without cycles) with a root in node $1$.</p><p>But this tree was not just a tree. A permutation $p$ of integers from $0$ to $n - 1$ is written in nodes, a number $p_i$ is written in node $i$.</p><p>As Grisha likes to invent some strange and interesting problems for himself, but not always can solve them, you need to help him deal with two types of queries on this tree.</p><p>Let's define a function $MEX(S)$, where $S$ is a set of non-negative integers, as a smallest non-negative integer that is not included in this set.</p><p>Let $l$ be a simple path in this tree. So let's define indices of nodes which lie on $l$ as $u_1$, $u_2$, $\ldots$, $u_k$. </p><p>Define $V(l)$ as a set {$p_{u_1}$, $p_{u_2}$, $\ldots$ , $p_{u_k}$}. </p><p>Then queries are: </p><ol> <li> For two nodes $i$ and $j$, swap $p_i$ and $p_j$. </li><li> Find the maximum value of $MEX(V(l))$ in all possible $l$. </li></ol></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \leq n \leq 2 \cdot 10^5$)&nbsp;— the number of nodes of a tree.</p><p>The second line contains $n$ integers&nbsp;— $p_1$, $p_2$, $\ldots$, $p_n$ ($0\leq p_i &lt; n$)&nbsp;— the permutation $p$, it's guaranteed that all numbers are different .</p><p>The third line contains $n - 1$ integers&nbsp;— $d_2$, $d_3$, $\ldots$, $d_n$ ($1 \leq d_i &lt; i$), where $d_i$ is a direct ancestor of node $i$ in a tree.</p><p>The fourth line contains a single integer $q$ ($1 \leq q \leq 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>The following $q$ lines contain the description of queries:</p><p>At the beginning of each of next $q$ lines, there is a single integer $t$ ($1$ or $2$)&nbsp;— the type of a query: </p><ol> <li> If $t = 1$, the line also contains two integers $i$ and $j$ ($1 \leq i, j \leq n$)&nbsp;— the indices of nodes, where values of the permutation should be swapped. </li><li> If $t = 2$, you need to find the maximum value of $MEX(V(l))$ in all possible $l$. </li></ol> </div><div class="output-specification"><p>For each type 2 query print a single integer&nbsp;— the answer for this query.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \leq n \leq 2 \cdot 10^5$)&nbsp;— the number of nodes of a tree.</p><p>The second line contains $n$ integers&nbsp;— $p_1$, $p_2$, $\ldots$, $p_n$ ($0\leq p_i &lt; n$)&nbsp;— the permutation $p$, it's guaranteed that all numbers are different .</p><p>The third line contains $n - 1$ integers&nbsp;— $d_2$, $d_3$, $\ldots$, $d_n$ ($1 \leq d_i &lt; i$), where $d_i$ is a direct ancestor of node $i$ in a tree.</p><p>The fourth line contains a single integer $q$ ($1 \leq q \leq 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>The following $q$ lines contain the description of queries:</p><p>At the beginning of each of next $q$ lines, there is a single integer $t$ ($1$ or $2$)&nbsp;— the type of a query: </p><ol> <li> If $t = 1$, the line also contains two integers $i$ and $j$ ($1 \leq i, j \leq n$)&nbsp;— the indices of nodes, where values of the permutation should be swapped. </li><li> If $t = 2$, you need to find the maximum value of $MEX(V(l))$ in all possible $l$. </li></ol>

## Output

<p>For each type 2 query print a single integer&nbsp;— the answer for this query.</p>





```input1
6
2 5 0 3 1 4
1 1 3 3 3
3
2
1 6 3
2
```




```input2
6
5 2 1 4 3 0
1 1 1 3 3
9
2
1 5 3
2
1 6 1
2
1 4 2
2
1 1 6
2
```




```output1
3
2
```




```output2
3
2
4
4
2
```



## Note

<p>Number written in brackets is a permutation value of a node. </p><center> <img class="tex-graphics" height="302px" src="file://rznoctKO.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center> In the first example, for the first query, optimal path is a path from node $1$ to node $5$. For it, set of values is $\{0, 1, 2\}$ and $MEX$ is $3$. <center> <img class="tex-graphics" height="302px" src="file://MgdLayh6.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center> For the third query, optimal path is a path from node $5$ to node $6$. For it, set of values is $\{0, 1, 4\}$ and $MEX$ is $2$. <center> <img class="tex-graphics" height="302px" src="file://UBlCRRAZ.png" style="max-width: 100.0%;max-height: 100.0%;" width="242px"> </center> In the second example, for the first query, optimal path is a path from node $2$ to node $6$. For it, set of values is $\{0, 1, 2, 5\}$ and $MEX$ is $3$. <center> <img class="tex-graphics" height="302px" src="file://j2VNLIs2.png" style="max-width: 100.0%;max-height: 100.0%;" width="276px"> </center> For the third query, optimal path is a path from node $5$ to node $6$. For it, set of values is $\{0, 1, 3\}$ and $MEX$ is $2$. <center> <img class="tex-graphics" height="302px" src="file://UjN302Kq.png" style="max-width: 100.0%;max-height: 100.0%;" width="242px"> </center> For the fifth query, optimal path is a path from node $5$ to node $2$. For it, set of values is $\{0, 1, 2, 3\}$ and $MEX$ is $4$. <center> <img class="tex-graphics" height="302px" src="file://FWvbdKcB.png" style="max-width: 100.0%;max-height: 100.0%;" width="249px"> </center> For the seventh query, optimal path is a path from node $5$ to node $4$. For it, set of values is $\{0, 1, 2, 3\}$ and $MEX$ is $4$. <center> <img class="tex-graphics" height="302px" src="file://Hsj13SJB.png" style="max-width: 100.0%;max-height: 100.0%;" width="249px"> </center> For the ninth query, optimal path is a path from node $6$ to node $5$. For it, set of values is $\{0, 1, 3\}$ and $MEX$ is $2$.
