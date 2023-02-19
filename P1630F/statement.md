## Description

<div><p>You are given an undirected graph of $n$ vertices indexed from $1$ to $n$, where vertex $i$ has a value $a_i$ assigned to it and all values $a_i$ are <span class="tex-font-style-bf">different</span>. There is an edge between two vertices $u$ and $v$ if either $a_u$ divides $a_v$ or $a_v$ divides $a_u$.</p><p>Find the minimum number of vertices to remove such that the remaining graph is bipartite, when you remove a vertex you remove all the edges incident to it.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5\cdot10^4$) — the number of vertices in the graph.</p><p>The second line of each test case contains $n$ integers, the $i$-th of them is the value $a_i$ ($1 \le a_i \le 5\cdot10^4$) assigned to the $i$-th vertex, all values $a_i$ are <span class="tex-font-style-bf">different</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5\cdot10^4$.</p></div><div class="output-specification"><p>For each test case print a single integer — the minimum number of vertices to remove such that the remaining graph is bipartite.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5\cdot10^4$) — the number of vertices in the graph.</p><p>The second line of each test case contains $n$ integers, the $i$-th of them is the value $a_i$ ($1 \le a_i \le 5\cdot10^4$) assigned to the $i$-th vertex, all values $a_i$ are <span class="tex-font-style-bf">different</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5\cdot10^4$.</p>

## Output

<p>For each test case print a single integer — the minimum number of vertices to remove such that the remaining graph is bipartite.</p>





```input1|2,3,6,7
4
4
8 4 2 1
4
30 2 3 5
5
12 4 6 2 3
10
85 195 5 39 3 13 266 154 14 2
```




```output1
2
0
1
2
```



## Note

<p>In the first test case if we remove the vertices with values $1$ and $2$ we will obtain a bipartite graph, so the answer is $2$, it is impossible to remove less than $2$ vertices and still obtain a bipartite graph.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span>Before</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span>After</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://9mqr8bPf.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://sf035M0C.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> <span class="tex-font-size-small">test case #1</span> </center><p>In the second test case we do not have to remove any vertex because the graph is already bipartite, so the answer is $0$.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span>Before</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span>After</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://RfR1HgDC.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://Vcghy8lg.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> <span class="tex-font-size-small">test case #2</span> </center><p>In the third test case we only have to remove the vertex with value $12$, so the answer is $1$.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span>Before</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span>After</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://tK0kTRll.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://95utKfnG.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> <span class="tex-font-size-small">test case #3</span> </center><p>In the fourth test case we remove the vertices with values $2$ and $195$, so the answer is $2$.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span>Before</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span>After</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://0tt3QYgG.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><img class="tex-graphics" src="file://d5BKrA3I.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> <span class="tex-font-size-small">test case #4</span> </center>
