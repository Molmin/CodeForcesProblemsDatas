## Description

<div><p>Recently, Vlad has been carried away by spanning trees, so his friends, without hesitation, gave him a connected weighted undirected graph of $n$ vertices and $m$ edges for his birthday.</p><p>Vlad defined the <span class="tex-font-style-it">ority</span> of a spanning tree as the <a href="https://tiny.cc/bitwise_or">bitwise OR</a> of all its weights, and now he is interested in what is the minimum possible <span class="tex-font-style-it">ority</span> that can be achieved by choosing a certain spanning tree. A spanning tree is a connected subgraph of a given graph that does not contain cycles.</p><p>In other words, you want to keep $n-1$ edges so that the graph remains connected and the bitwise OR weights of the edges are as small as possible. You have to find the minimum bitwise OR itself.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input.</p><p>An empty line is written in front of each test case.</p><p>This is followed by two numbers $n$ and $m$ ($3 \le n \le 2 \cdot 10^5, n - 1 \le m \le 2 \cdot 10^5$) — the number of vertices and edges of the graph, respectively.</p><p>The next $m$ lines contain the description of the edges. Line $i$ contains three numbers $v_i$, $u_i$ and $w_i$ ($1 \le v_i, u_i \le n$, $1 \le w_i \le 10^9$, $v_i \neq u_i$) — the vertices that the edge connects and its weight.</p><p>It is guaranteed that the sum $m$ and the sum $n$ over all test cases does not exceed $2 \cdot 10^5$ and each test case contains a connected graph.</p></div><div class="output-specification"><p>Print $t$ lines, each of which contains the answer to the corresponding set of input data&nbsp;— the minimum possible spanning tree <span class="tex-font-style-it">ority</span>.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input.</p><p>An empty line is written in front of each test case.</p><p>This is followed by two numbers $n$ and $m$ ($3 \le n \le 2 \cdot 10^5, n - 1 \le m \le 2 \cdot 10^5$) — the number of vertices and edges of the graph, respectively.</p><p>The next $m$ lines contain the description of the edges. Line $i$ contains three numbers $v_i$, $u_i$ and $w_i$ ($1 \le v_i, u_i \le n$, $1 \le w_i \le 10^9$, $v_i \neq u_i$) — the vertices that the edge connects and its weight.</p><p>It is guaranteed that the sum $m$ and the sum $n$ over all test cases does not exceed $2 \cdot 10^5$ and each test case contains a connected graph.</p>

## Output

<p>Print $t$ lines, each of which contains the answer to the corresponding set of input data&nbsp;— the minimum possible spanning tree <span class="tex-font-style-it">ority</span>.</p>





```input1
3

3 3
1 2 1
2 3 2
1 3 2

5 7
4 2 7
2 5 8
3 4 2
3 2 1
2 4 2
4 1 2
1 2 2

3 4
1 2 1
2 3 2
1 3 3
3 1 4
```




```output1
2
10
3
```



## Note

<center> <img class="tex-graphics" src="file://4bKPU38h.png" style="max-width: 100.0%;max-height: 100.0%;" width="340px"> <span class="tex-font-size-small">Graph from the first test case.</span> </center><center> <img class="tex-graphics" src="file://uthCnThK.png" style="max-width: 100.0%;max-height: 100.0%;" width="340px"> <span class="tex-font-size-small"><span class="tex-font-style-it">Ority</span> of this tree equals to <span class="tex-font-style-tt">2 or 2 = 2</span> and it's minimal.</span> </center><center> <img class="tex-graphics" src="file://UhtQ7fWc.png" style="max-width: 100.0%;max-height: 100.0%;" width="340px"> <span class="tex-font-size-small">Without excluding edge with weight $1$ <span class="tex-font-style-it">ority</span> is <span class="tex-font-style-tt">1 or 2 = 3</span>.</span> </center>
