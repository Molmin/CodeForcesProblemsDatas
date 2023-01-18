## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>You're given a tree consisting of $n$ nodes, rooted at node $1$. A tree is a connected graph with no cycles.</p><p>We chose a hidden node $x$. In order to find this node, you can ask queries of two types: </p><ul> <li> <span class="tex-font-style-tt">d</span> $u$ ($1 \le u \le n$). We will answer with the distance between nodes $u$ and $x$. The distance between two nodes is the number of edges in the shortest path between them. </li><li> <span class="tex-font-style-tt">s</span> $u$ ($1 \le u \le n$). We will answer with the second node on the path from $u$ to $x$. However, there's a plot twist. If $u$ is <span class="tex-font-style-bf">not</span> an ancestor of $x$, you'll receive "<span class="tex-font-style-tt">Wrong answer</span>" verdict! </li></ul><p>Node $a$ is called an ancestor of node $b$ if $a \ne b$ and the shortest path from node $1$ to node $b$ passes through node $a$. <span class="tex-font-style-bf">Note that in this problem a node is not an ancestor of itself</span>.</p><p>Can you find $x$ in no more than $36$ queries? The hidden node is fixed in each test beforehand and does not depend on your queries.</p></div><div class="input-specification"><p>The first line contains the integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of nodes in the tree.</p><p>Each of the next $n-1$ lines contains two space-separated integers $u$ and $v$ ($1 \le u,v \le n$) that mean there's an edge between nodes $u$ and $v$. It's guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>To print the answer, print "<span class="tex-font-style-tt">! x</span>" (without quotes).</p></div><div><h2>Interaction</h2><p>To ask a question, print it in one of the formats above: </p><ul> <li> <span class="tex-font-style-tt">d</span> $u$ ($1 \le u \le n$), or </li><li> <span class="tex-font-style-tt">s</span> $u$ ($1 \le u \le n$). </li></ul><p>After each question, you should read the answer: either the distance or the second vertex on the path, as mentioned in the legend. </p><p>If we answer with $-1$ instead of a valid answer, that means you exceeded the number of queries, made an invalid query, or violated the condition in the second type of queries. Exit immediately after receiving $-1$ and you will see <span class="tex-font-style-tt">Wrong answer</span> verdict. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>After printing a query, do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> See the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks:</span></p><p>The first line should contain two integers $n$ and $x$ ($2 \le n \le 2 \cdot 10^5$, $1 \le x \le n$).</p><p>Each of the next $n-1$ lines should contain two integers $u$ and $v$ ($1 \le u,v \le n$) that mean there is an edge between nodes $u$ and $v$. The edges must form a tree.</p></div>

## Input

<p>The first line contains the integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of nodes in the tree.</p><p>Each of the next $n-1$ lines contains two space-separated integers $u$ and $v$ ($1 \le u,v \le n$) that mean there's an edge between nodes $u$ and $v$. It's guaranteed that the given graph is a tree.</p>

## Output

<p>To print the answer, print "<span class="tex-font-style-tt">! x</span>" (without quotes).</p>





```input1
5
1 2
1 3
3 4
3 5
3
5
```




```output1
d 2
s 3
! 5
```



## Note

<p>In the first example, the hidden node is node $5$.</p><center> <img class="tex-graphics" src="file://muRgZnQY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>We first ask about the distance between node $x$ and node $2$. The answer is $3$, so node $x$ is either $4$ or $5$. We then ask about the second node in the path from node $3$ to node $x$. Note here that node $3$ is an ancestor of node $5$. We receive node $5$ as the answer. Finally, we report that the hidden node is node $5$.</p>
