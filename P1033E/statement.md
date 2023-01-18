## Description

<div><p>Bob has a simple undirected connected graph (without self-loops and multiple edges). He wants to learn whether his graph is bipartite (that is, you can paint all vertices of the graph into two colors so that there is no edge connecting two vertices of the same color) or not. As he is not very good at programming, he asked Alice for help. He does not want to disclose his graph to Alice, but he agreed that Alice can ask him some questions about the graph.</p><p>The only question that Alice can ask is the following: she sends $s$&nbsp;— a subset of vertices of the original graph. Bob answers with the number of edges that have both endpoints in $s$. Since he doesn't want Alice to learn too much about the graph, he allows her to ask no more than $20000$ questions. Furthermore, he suspects that Alice might introduce false messages to their communication channel, so when Alice finally tells him whether the graph is bipartite or not, she also needs to provide a proof&nbsp;— either the partitions themselves or a cycle of odd length.</p><p>Your task is to help Alice to construct the queries, find whether the graph is bipartite. </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 600$)&nbsp;— the number of vertices in Bob's graph.</p></div><div><h2>Interaction</h2><p>First, read an integer $n$ ($1\leq n\leq 600$)&nbsp;— the number of vertices in Bob's graph.</p><p>To make a query, print two lines. First of which should be in the format "<span class="tex-font-style-tt">? k</span>" ($1 \leq k \leq n$), where $k$ is the size of the set to be queried. The second line should contain $k$ space separated distinct integers $s_1, s_2, \dots, s_k$ ($1 \leq s_i \leq n$)&nbsp;— the vertices of the queried set.</p><p>After each query read a single integer $m$ ($0 \leq m \leq \frac{n(n-1)}{2}$)&nbsp;— the number of edges between the vertices of the set $\{s_i\}$.</p><p>You are not allowed to ask more than $20000$ queries.</p><p>If $m = -1$, it means that you asked more queries than allowed, or asked an invalid query. Your program should immediately terminate (for example, by calling exit(0)). You will receive <span class="tex-font-style-tt">Wrong Answer</span>; it means that you asked more queries than allowed, or asked an invalid query. If you ignore this, you can get other verdicts since your program will continue to read from a closed stream.</p><p>After printing a query do not forget to print end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p>When you know the answer, you need to print it.</p><p>The format of the answer depends on whether the graph is bipartite or not.</p><p>If the graph is bipartite, print two lines. The first should contain the letter "<span class="tex-font-style-tt">Y</span>" (short for "<span class="tex-font-style-tt">YES</span>") followed by a space, and then a single integer $s$&nbsp;($0 \leq s \leq n$)&nbsp;— the number of vertices in one of the partitions. Second line should contain $s$ integers $a_1, a_2, \dots, a_s$&nbsp;— vertices belonging to the first partition. All $a_i$ must be distinct, and all edges in the main graph must have exactly one endpoint in the set $\{a_i\}$.</p><p>If the graph is not bipartite, print two lines. The first should contain the letter "<span class="tex-font-style-tt">N</span>" (short for "<span class="tex-font-style-tt">NO</span>") followed by a space, and then a single integer $l$&nbsp;($3 \leq l \leq n$)&nbsp;— the length of one simple cycle of odd length. Second line should contain $l$ integers $c_1, c_2, \dots, c_l$&nbsp;— the vertices along the cycle. It must hold that for all $1 \leq i \leq l$, there is an edge $\{c_i, c_{(i \mod l)+1}\}$ in the main graph, and all $c_i$ are distinct.</p><p>If there are multiple possible answers, you may print any of them.</p><p><span class="tex-font-style-bf">Hacks format</span> For hacks, use the following format:</p><p>The first line contains two integers $n$ and $m~(1 \leq n \leq 600, 0 \leq m \leq \frac{n(n-1)}{2})$&nbsp;— the number of vertices and edges of the graph, respectively.</p><p>Each of the next $m$ lines contains two integers $u_i$ and $v_i~(1 \leq u_i, v_i \leq n)$ mean that there is an edge between $u_i$ and $v_i$. There must not be any multiple edges, no loops, and the graph must be connected.</p><p>For example, you need to use this test to get the first sample:</p><pre class="verbatim"><br>4 4<br>4 1<br>1 3<br>3 2<br>2 4<br></pre></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 600$)&nbsp;— the number of vertices in Bob's graph.</p>





```input1
4
4
0
1
1
1
0
```




```input2
4
4
3
```




```output1
? 4 
1 2 3 4
? 2
1 2
? 2
1 3
? 2
1 4
? 2
2 4
? 2
3 4
Y 2
1 2
```




```output2
? 4
1 4 2 3
? 3
1 2 4
N 3
2 1 4
```



## Note

<p>In the first case, Alice learns that there are $4$ edges in the whole graph. Over the course of the next three queries, she learns that vertex $1$ has two neighbors: $3$ and $4$. She then learns that while vertex $2$ is adjacent to $4$, the vertex $3$ isn't adjacent to $4$. There is only one option for the remaining edge, and that is $(2, 3)$. This means that the graph is a cycle on four vertices, with $(1, 2)$ being one partition and $(3, 4)$ being the second. Here, it would be also valid to output "<span class="tex-font-style-tt">3 4</span>" on the second line.</p><p>In the second case, we also have a graph on four vertices and four edges. In the second query, Alice learns that there are three edges among vertices $(1, 2, 4)$. The only way this could possibly happen is that those form a triangle. As the triangle is not bipartite, Alice can report it as a proof. Notice that she does not learn where the fourth edge is, but she is able to answer Bob correctly anyway.</p>
