## Description

<div><p>There is a new attraction in Singapore Zoo: The Infinite Zoo.</p><p>The Infinite Zoo can be represented by a graph with an infinite number of vertices labeled $1,2,3,\ldots$. There is a directed edge from vertex $u$ to vertex $u+v$ if and only if $u\&amp;v=v$, where $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>. There are no other edges in the graph.</p><p>Zookeeper has $q$ queries. In the $i$-th query she will ask you if she can travel from vertex $u_i$ to vertex $v_i$ by going through directed edges.</p></div><div class="input-specification"><p>The first line contains an integer $q$ ($1 \leq q \leq 10^5$) — the number of queries.</p><p>The $i$-th of the next $q$ lines will contain two integers $u_i$, $v_i$ ($1 \leq u_i, v_i &lt; 2^{30}$) — a query made by Zookeeper.</p></div><div class="output-specification"><p>For the $i$-th of the $q$ queries, output "<span class="tex-font-style-tt">YES</span>" in a single line if Zookeeper can travel from vertex $u_i$ to vertex $v_i$. Otherwise, output "<span class="tex-font-style-tt">NO</span>".</p><p>You can print your answer in any case. For example, if the answer is "<span class="tex-font-style-tt">YES</span>", then the output "<span class="tex-font-style-tt">Yes</span>" or "<span class="tex-font-style-tt">yeS</span>" will also be considered as correct answer.</p></div>

## Input

<p>The first line contains an integer $q$ ($1 \leq q \leq 10^5$) — the number of queries.</p><p>The $i$-th of the next $q$ lines will contain two integers $u_i$, $v_i$ ($1 \leq u_i, v_i &lt; 2^{30}$) — a query made by Zookeeper.</p>

## Output

<p>For the $i$-th of the $q$ queries, output "<span class="tex-font-style-tt">YES</span>" in a single line if Zookeeper can travel from vertex $u_i$ to vertex $v_i$. Otherwise, output "<span class="tex-font-style-tt">NO</span>".</p><p>You can print your answer in any case. For example, if the answer is "<span class="tex-font-style-tt">YES</span>", then the output "<span class="tex-font-style-tt">Yes</span>" or "<span class="tex-font-style-tt">yeS</span>" will also be considered as correct answer.</p>





```input1
5
1 4
3 6
1 6
6 2
5 5
```




```output1
YES
YES
NO
NO
YES
```



## Note

<p>The subgraph on vertices $1,2,3,4,5,6$ is shown below.</p><center> <img class="tex-graphics" src="file://CeW2N6oC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
