## Description

<div><p><span class="tex-font-style-bf">Note that the only difference between the easy and hard version is the constraint on the number of queries. You can make hacks only if all versions of the problem are solved.</span></p><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>You are given a tree consisting of $n$ nodes numbered with integers from $1$ to $n$. Ayush and Ashish chose two secret distinct nodes in the tree. You need to find out both the nodes. You can make the following query: </p><ul> <li> Provide a list of nodes and you will receive a node from that list whose sum of distances to both the hidden nodes is minimal (if there are multiple such nodes in the list, you will receive any one of them). You will also get the sum of distances of that node to the hidden nodes. </li></ul><p>Recall that a tree is a connected graph without cycles. The distance between two nodes is defined as the number of edges in the simple path between them.</p><p>More formally, let's define two hidden nodes as $s$ and $f$. In one query you can provide the set of nodes $\{a_1, a_2, \ldots, a_c\}$ of the tree. As a result, you will get two numbers $a_i$ and $dist(a_i, s) + dist(a_i, f)$. The node $a_i$ is any node from the provided set, for which the number $dist(a_i, s) + dist(a_i, f)$ is minimal.</p><p><span class="tex-font-style-bf">You can ask no more than $11$ queries.</span></p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \leq t \leq 10)$&nbsp;— the number of test cases. <span class="tex-font-style-bf">Please note, how the interaction process is organized.</span></p><p>The first line of each test case consists of a single integer $n$ $(2 \le n \le 1000)$&nbsp;— the number of nodes in the tree.</p><p>The next $n - 1$ lines consist of two integers $u$, $v$ $(1 \le u, v \le n, u \ne v)$&nbsp;— the edges of the tree.</p></div><div><h2>Interaction</h2><p>To ask a query print a single line: </p><ul> <li> In the beginning print "<span class="tex-font-style-tt">? c</span> " (without quotes) where $c$ $(1 \leq c \leq n)$ denotes the number of nodes being queried, followed by $c$ <span class="tex-font-style-bf">distinct</span> integers in the range $[1, n]$ &nbsp;— the indices of nodes from the list. </li></ul><p>For each query, you will receive two integers $x$, $d$&nbsp;— the node (among the queried nodes) with the minimum sum of distances to the hidden nodes and the sum of distances from that node to the hidden nodes. If the subset of nodes queried is invalid or you exceeded the number of queries then you will get $x = d = -1$. In this case, you should terminate the program immediately.</p><p>When you have guessed the hidden nodes, print a single line "<span class="tex-font-style-tt">!</span> " (without quotes), followed by two integers in the range $[1, n]$ &nbsp;— the hidden nodes. You can output the hidden nodes in any order.</p><p><span class="tex-font-style-bf">After this, you should read a string.</span> If you guess the nodes correctly, you will receive the string "<span class="tex-font-style-tt">Correct</span>". In this case, you should continue solving the remaining test cases or terminate the program, if all test cases were solved. Otherwise, you will receive the string "<span class="tex-font-style-tt">Incorrect</span>". In this case, you should terminate the program immediately.</p><p>Guessing the hidden nodes does <span class="tex-font-style-bf">not</span> count towards the number of queries asked.</p><p><span class="tex-font-style-bf">The interactor is not adaptive.</span> The hidden nodes do not change with queries.</p><p><span class="tex-font-style-bf">Do not forget</span> to read the string "<span class="tex-font-style-tt">Correct</span>" / "<span class="tex-font-style-tt">Incorrect</span>" after guessing the hidden nodes.</p><p>You need to solve each test case before receiving the input for the next test case.</p><p><span class="tex-font-style-bf">The limit of $11$ queries applies to each test case and not to the entire input.</span></p><p>After printing a query do not forget to output the end of the line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack the solution, use the following test format:</p><p>The first line should contain a single integer $t$ $(1 \leq t \leq 10)$&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case should contain a single integer $n$ $(2 \le n \le 1000)$&nbsp;— the number of nodes in the tree. The second line should contain two distinct integers in the range $[1, n]$ &nbsp;— the hidden nodes. The next $n - 1$ lines should contain two integers $u$, $v$ $(1 \le u, v \le n, u \ne v)$ &nbsp;— the edges of the tree.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \leq t \leq 10)$&nbsp;— the number of test cases. <span class="tex-font-style-bf">Please note, how the interaction process is organized.</span></p><p>The first line of each test case consists of a single integer $n$ $(2 \le n \le 1000)$&nbsp;— the number of nodes in the tree.</p><p>The next $n - 1$ lines consist of two integers $u$, $v$ $(1 \le u, v \le n, u \ne v)$&nbsp;— the edges of the tree.</p>





```input1
1
3
1 2
1 3

1 1

2 3

3 1

3 1

Correct
```




```output1
? 1 1

? 1 2

? 1 3

? 2 2 3

! 1 3
```



## Note

<p>The tree from the first test is shown below, and the hidden nodes are $1$ and $3$.</p><center><img class="tex-graphics" src="file://uXvI4SoI.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
