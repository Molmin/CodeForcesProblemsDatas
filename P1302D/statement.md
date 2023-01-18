## Description

<div><p><span class="tex-font-style-it">This is an unusual problem in an unusual contest, here is the announcement: <a href="//codeforces.com/blog/entry/73543">http://codeforces.com/blog/entry/73543</a></span></p><p>Find the distance between vertices $1$ and $n$ in an undirected weighted graph.</p></div><div class="input-specification"><p>The first line contains two integers $n, m$ ($1 \leq n, m \leq 2 \cdot 10^5$) — the number of vertices and the number of edges.</p><p>Each of the next $m$ lines contain description of an edge $a_i~b_i~cost_i$ ($1 \leq a_i, b_i \leq n$, $1 \leq cost_i \leq 10^9$).</p><p>Loops and multiple edges? Hmm, why not?</p></div><div class="output-specification"><p>Print one integer — the answer to the problem. If there is no path, print $-1$ instead.</p></div>

## Input

<p>The first line contains two integers $n, m$ ($1 \leq n, m \leq 2 \cdot 10^5$) — the number of vertices and the number of edges.</p><p>Each of the next $m$ lines contain description of an edge $a_i~b_i~cost_i$ ($1 \leq a_i, b_i \leq n$, $1 \leq cost_i \leq 10^9$).</p><p>Loops and multiple edges? Hmm, why not?</p>

## Output

<p>Print one integer — the answer to the problem. If there is no path, print $-1$ instead.</p>





```input1
3 3
1 2 5
2 3 1
1 3 7
```




```output1
6
```


