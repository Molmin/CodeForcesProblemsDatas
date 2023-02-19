## Description

<div><p>Last summer, Feluda gifted Lalmohan-Babu a <span class="tex-font-style-bf">balanced</span> bracket sequence $s$ of length $2 n$.</p><p>Topshe was bored during his summer vacations, and hence he decided to draw an undirected graph of $2 n$ vertices using the <span class="tex-font-style-underline">balanced bracket sequence</span> $s$. For any two distinct vertices $i$ and $j$ ($1 \le i &lt; j \le 2 n$), Topshe draws an edge (undirected and unweighted) between these two nodes if and only if the <span class="tex-font-style-underline">subsegment</span> $s[i \ldots j]$ forms a balanced bracket sequence.</p><p>Determine the number of <span class="tex-font-style-underline">connected components</span> in Topshe's graph.</p><p>See the Notes section for definitions of the underlined terms.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) — the number of opening brackets in string $s$.</p><p>The second line of each test case contains a string $s$ of length $2 n$&nbsp;— a balanced bracket sequence consisting of $n$ opening brackets "<span class="tex-font-style-tt">(</span>", and $n$ closing brackets "<span class="tex-font-style-tt">)</span>".</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the number of connected components in Topshe's graph.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) — the number of opening brackets in string $s$.</p><p>The second line of each test case contains a string $s$ of length $2 n$&nbsp;— a balanced bracket sequence consisting of $n$ opening brackets "<span class="tex-font-style-tt">(</span>", and $n$ closing brackets "<span class="tex-font-style-tt">)</span>".</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the number of connected components in Topshe's graph.</p>





```input1|2,3,6,7
4
1
()
3
()(())
3
((()))
4
(())(())
```




```output1
1
2
3
3
```



## Note

<p><span class="tex-font-style-underline">Sample explanation</span>:</p><p>In the first test case, the graph constructed from the bracket sequence <span class="tex-font-style-tt">()</span>, is just a graph containing nodes $1$ and $2$ connected by a single edge. </p><p>In the second test case, the graph constructed from the bracket sequence <span class="tex-font-style-tt">()(())</span> would be the following (containing two connected components):</p><center> <img class="tex-graphics" src="file://oxBLS8r4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p><span class="tex-font-style-underline">Definition of Underlined Terms</span>:</p><ul><li> A sequence of brackets is called balanced if one can turn it into a valid math expression by adding characters $+$ and $1$. For example, sequences <span class="tex-font-style-tt">(())()</span>, <span class="tex-font-style-tt">()</span>, and <span class="tex-font-style-tt">(()(()))</span> are balanced, while <span class="tex-font-style-tt">)(</span>, <span class="tex-font-style-tt">(()</span>, and <span class="tex-font-style-tt">(()))(</span> are not.</li><li> The subsegment $s[l \ldots r]$ denotes the sequence $[s_l, s_{l + 1}, \ldots, s_r]$.</li><li> A connected component is a set of vertices $X$ such that for every two vertices from this set there exists at least one path in the graph connecting these vertices, but adding any other vertex to $X$ violates this rule.</li></ul>
