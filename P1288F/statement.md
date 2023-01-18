## Description

<div><p>You are given a bipartite graph: the first part of this graph contains $n_1$ vertices, the second part contains $n_2$ vertices, and there are $m$ edges. <span class="tex-font-style-bf">The graph can contain multiple edges</span>.</p><p>Initially, each edge is colorless. For each edge, you may either leave it uncolored (it is free), paint it red (it costs $r$ coins) or paint it blue (it costs $b$ coins). No edge can be painted red and blue simultaneously.</p><p>There are three types of vertices in this graph — colorless, red and blue. Colored vertices impose additional constraints on edges' colours:</p><ul> <li> for each red vertex, the number of red edges indicent to it should be <span class="tex-font-style-bf">strictly greater</span> than the number of blue edges incident to it; </li><li> for each blue vertex, the number of blue edges indicent to it should be <span class="tex-font-style-bf">strictly greater</span> than the number of red edges incident to it. </li></ul><p>Colorless vertices impose no additional constraints.</p><p>Your goal is to paint some (possibly none) edges so that all constraints are met, and among all ways to do so, you should choose the one with minimum total cost. </p></div><div class="input-specification"><p>The first line contains five integers $n_1$, $n_2$, $m$, $r$ and $b$ ($1 \le n_1, n_2, m, r, b \le 200$) — the number of vertices in the first part, the number of vertices in the second part, the number of edges, the amount of coins you have to pay to paint an edge red, and the amount of coins you have to pay to paint an edge blue, respectively.</p><p>The second line contains one string consisting of $n_1$ characters. Each character is either <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">R</span> or <span class="tex-font-style-tt">B</span>. If the $i$-th character is <span class="tex-font-style-tt">U</span>, then the $i$-th vertex of the first part is uncolored; <span class="tex-font-style-tt">R</span> corresponds to a red vertex, and <span class="tex-font-style-tt">B</span> corresponds to a blue vertex.</p><p>The third line contains one string consisting of $n_2$ characters. Each character is either <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">R</span> or <span class="tex-font-style-tt">B</span>. This string represents the colors of vertices of the second part in the same way.</p><p>Then $m$ lines follow, the $i$-th line contains two integers $u_i$ and $v_i$ ($1 \le u_i \le n_1$, $1 \le v_i \le n_2$) denoting an edge connecting the vertex $u_i$ from the first part and the vertex $v_i$ from the second part.</p><p>The graph may contain multiple edges.</p></div><div class="output-specification"><p>If there is no coloring that meets all the constraints, print one integer $-1$.</p><p>Otherwise, print an integer $c$ denoting the total cost of coloring, and a string consisting of $m$ characters. The $i$-th character should be <span class="tex-font-style-tt">U</span> if the $i$-th edge should be left uncolored, <span class="tex-font-style-tt">R</span> if the $i$-th edge should be painted red, or <span class="tex-font-style-tt">B</span> if the $i$-th edge should be painted blue. If there are multiple colorings with minimum possible cost, print any of them.</p></div>

## Input

<p>The first line contains five integers $n_1$, $n_2$, $m$, $r$ and $b$ ($1 \le n_1, n_2, m, r, b \le 200$) — the number of vertices in the first part, the number of vertices in the second part, the number of edges, the amount of coins you have to pay to paint an edge red, and the amount of coins you have to pay to paint an edge blue, respectively.</p><p>The second line contains one string consisting of $n_1$ characters. Each character is either <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">R</span> or <span class="tex-font-style-tt">B</span>. If the $i$-th character is <span class="tex-font-style-tt">U</span>, then the $i$-th vertex of the first part is uncolored; <span class="tex-font-style-tt">R</span> corresponds to a red vertex, and <span class="tex-font-style-tt">B</span> corresponds to a blue vertex.</p><p>The third line contains one string consisting of $n_2$ characters. Each character is either <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">R</span> or <span class="tex-font-style-tt">B</span>. This string represents the colors of vertices of the second part in the same way.</p><p>Then $m$ lines follow, the $i$-th line contains two integers $u_i$ and $v_i$ ($1 \le u_i \le n_1$, $1 \le v_i \le n_2$) denoting an edge connecting the vertex $u_i$ from the first part and the vertex $v_i$ from the second part.</p><p>The graph may contain multiple edges.</p>

## Output

<p>If there is no coloring that meets all the constraints, print one integer $-1$.</p><p>Otherwise, print an integer $c$ denoting the total cost of coloring, and a string consisting of $m$ characters. The $i$-th character should be <span class="tex-font-style-tt">U</span> if the $i$-th edge should be left uncolored, <span class="tex-font-style-tt">R</span> if the $i$-th edge should be painted red, or <span class="tex-font-style-tt">B</span> if the $i$-th edge should be painted blue. If there are multiple colorings with minimum possible cost, print any of them.</p>





```input1
3 2 6 10 15
RRB
UB
3 2
2 2
1 2
1 1
2 1
1 1
```




```input2
3 1 3 4 5
RRR
B
2 1
1 1
3 1
```




```input3
3 1 3 4 5
URU
B
2 1
1 1
3 1
```




```output1
35
BUURRU
```




```output2
-1
```




```output3
14
RBB
```


