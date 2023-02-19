## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem!</span></p><p><span class="tex-font-style-it">In the last regional contest Hemose, ZeyadKhattab and YahiaSherif — members of the team Carpe Diem — did not qualify to ICPC because of some <span class="tex-font-style-striked">un</span>known reasons. Hemose was very sad and had a bad day after the contest, but ZeyadKhattab is very wise and knows Hemose very well, and does not want to see him sad.</span></p><p>Zeyad knows that Hemose loves tree problems, so he gave him a tree problem with a very special device.</p><p>Hemose has a weighted tree with $n$ nodes and $n-1$ edges. Unfortunately, Hemose doesn't remember the weights of edges.</p><p>Let's define $Dist(u, v)$ for $u\neq v$ as the greatest common divisor of the weights of all edges on the path from node $u$ to node $v$.</p><p>Hemose has a special device. Hemose can give the device a set of nodes, and the device will return the largest $Dist$ between any two nodes from the set. More formally, if Hemose gives the device a set $S$ of nodes, the device will return the largest value of $Dist(u, v)$ over all pairs $(u, v)$ with $u$, $v$ $\in$ $S$ and $u \neq v$.</p><p>Hemose can use this Device <span class="tex-font-style-bf">at most $12$ times</span>, and wants to find any two distinct nodes $a$, $b$, such that $Dist(a, b)$ is maximum possible. Can you help him?</p></div><div><h2>Interaction</h2><p>Begin the interaction from reading a single integer $n$ ($2 \le n \le 10^3$) — the number of nodes in the tree.</p><p>Next, read $n-1$ lines. </p><p>The $i$-th of the next $n-1$ lines contains two integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$, $u_i\neq v_i$), which means that there's an edge between nodes $u_i$ and $v_i$.</p><p><span class="tex-font-style-bf">It's guaranteed that weights of edges were $\leq 10^9$</span>.</p><p>It is guaranteed that the given graph is a tree.</p><p>Now you may begin asking queries. To ask a query about a set of $k$ nodes $v_1, v_2, \ldots, v_k$ ($2 \le k \le n$, $1 \le v_i \le n$, all $v_i$ are distinct), output:</p><p> <span class="tex-font-style-tt">?</span> $k$ $v_1$ $v_2$ $\ldots$ $v_k$</p><p>You will then receive an integer $x$, the largest $Dist(v_i, v_j)$ over $1 \le i, j \le k$ with $i \neq j$.</p><p>When you have found $a$ and $b$ ($1 \le a, b \le n)$, $a\neq b$) such that $Dist(a, b)$ is the maximum possible, print the answer in the following format: </p><p><span class="tex-font-style-tt">!</span> $a$ $b$ </p><p><span class="tex-font-style-bf">Outputting answer doesn't count towards the limit of $12$ queries.</span></p><p>If there are several pairs $(a, b)$ with the same largest $Dist(a, b)$, you can output any.</p><p>After printing a query do not forget to output the end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack a solution, use the following format.</p><p>The first line should contain a single integer $n$ $(2 \leq n \le 10^3)$ — the number of nodes.</p><p>The $i$-th of the next $n-1$ lines should contain three integers $u_i$, $v_i$, $w_i$ ($1 \le u_i, v_i \le n$, $u_i\ne v_i$, $1 \le w \le 10^9$), which means that there's an edge between nodes $u_i$ and $v_i$ with weight $w_i$.</p><p>These $n-1$ edges must form a tree.</p></div>





```input1
6
1 2
2 3
2 4
1 5
5 6

10

2

10
```




```output1
? 6 1 2 3 4 5 6

? 3 3 1 5

? 2 1 2

! 1 2
```



## Note

<p>The tree in the first sample:</p><p><img class="tex-graphics" src="file://nM4bWQjK.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
