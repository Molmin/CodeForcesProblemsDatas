## Description

<div><div class="epigraph"><div class="epigraph-text">As for the technology in the outside world, it is really too advanced for Gensokyo to even look up to.</div><div class="epigraph-source">—Yasaka Kanako, <span class="tex-font-style-it">Symposium of Post-mysticism</span></div></div><p><span class="tex-font-style-it">This is an interactive problem</span>.</p><p>Under the direct supervision of Kanako and the Moriya Shrine, the railway system of Gensokyo is finally finished. GSKR (Gensokyo Railways) consists of $n$ stations with $m$ bidirectional tracks connecting them. The $i$-th track has length $l_i$ ($1\le l_i\le 10^6$). Due to budget limits, the railway system <span class="tex-font-style-bf">may not be connected</span>, though there may be more than one track between two stations.</p><p>The <span class="tex-font-style-it">value</span> of a railway system is defined as the total length of its all tracks. The <span class="tex-font-style-it">maximum (or minimum) capacity</span> of a railway system is defined as the maximum (or minimum) value among all of the currently functional system's <a href="https://en.wikipedia.org/wiki/Spanning_tree#Spanning_forests">full spanning forest</a>.</p><p>In brief, full spanning forest of a graph is a spanning forest with the same connectivity as the given graph.</p><p>Kanako has a simulator only able to process no more than $2m$ queries. The input of the simulator is a string $s$ of length $m$, consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>. The simulator will assume the $i$-th track functional if $s_i=$ <span class="tex-font-style-tt">1</span>. The device will then tell Kanako the maximum capacity of the system in the simulated state.</p><p>Kanako wants to know the the minimum capacity of the system with all tracks functional with the help of the simulator.</p><p>The structure of the railway system is fixed in advance. In other words, the interactor is not adaptive.</p></div><div class="input-specification"><p>The first and only line of input contains two integers $n,m$ ($2 \leq n \leq 200$, $1\le m \le 500$) — the number of stations and tracks.</p></div><div><h2>Interaction</h2><p>Begin the interaction by reading $n,m$.</p><p>To make a query, print "<span class="tex-font-style-tt">?</span> $s$" (without quotes, $s$ is a string of length $m$, consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>). Then you should read our response from standard input — the maximum capacity of the system in the simulated state.</p><p>If your program has made an invalid query or has run out of tries, the interactor will terminate immediately and your program will get a verdict <span class="tex-font-style-tt">Wrong answer</span>. </p><p>To give the final answer, print "<span class="tex-font-style-tt">!</span> $L$" (without the quotes, $L$ is the minimum capacity of the system with all tracks functional). Note that giving this answer is not counted towards the limit of $2m$ queries.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul> <p><span class="tex-font-style-bf">Hacks</span></p><p>The first line of input must contain two integers $n,m$ ($2 \leq n \leq 200$, $1\le m \le 500$) — the number of stations and tracks.</p><p>The next $m$ lines of input must contain exactly $3$ space-separated integers $u_i$, $v_i$, $l_i$ ($1\le u_i,v_i \le n$, $u_i\ne v_i$, $1 \leq l_i \leq 10^6$) — the endpoints and the length of the $i$-th track.</p></div>

## Input

<p>The first and only line of input contains two integers $n,m$ ($2 \leq n \leq 200$, $1\le m \le 500$) — the number of stations and tracks.</p>





```input1
5 4

0

5

9

7
```




```output1
? 0000

? 1110

? 1111

? 1101

! 7
```



## Note

<p>Here is the graph of the example, satisfying $l_i=i$.</p><center> <img class="tex-graphics" src="file://7jMduwuD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
