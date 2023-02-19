## Description

<div><p>A triple of points $i$, $j$ and $k$ on a coordinate line is called <span class="tex-font-style-bf">beautiful</span> if $i &lt; j &lt; k$ and $k - i \le d$.</p><p>You are given a set of points on a coordinate line, initially empty. You have to process queries of three types:</p><ul> <li> add a point; </li><li> remove a point; </li><li> calculate the number of beautiful triples consisting of points belonging to the set. </li></ul></div><div class="input-specification"><p>The first line contains two integers $q$ and $d$ ($1 \le q, d \le 2 \cdot 10^5$) — the number of queries and the parameter for defining if a triple is beautiful, respectively.</p><p>The second line contains $q$ integers $a_1, a_2, \dots, a_q$ ($1 \le a_i \le 2 \cdot 10^5$) denoting the queries. The integer $a_i$ denotes the $i$-th query in the following way:</p><ul> <li> if the point $a_i$ belongs to the set, remove it; otherwise, add it; </li><li> after adding or removing the point, print the number of beautiful triples. </li></ul></div><div class="output-specification"><p>For each query, print one integer — the number of beautiful triples after processing the respective query.</p></div>

## Input

<p>The first line contains two integers $q$ and $d$ ($1 \le q, d \le 2 \cdot 10^5$) — the number of queries and the parameter for defining if a triple is beautiful, respectively.</p><p>The second line contains $q$ integers $a_1, a_2, \dots, a_q$ ($1 \le a_i \le 2 \cdot 10^5$) denoting the queries. The integer $a_i$ denotes the $i$-th query in the following way:</p><ul> <li> if the point $a_i$ belongs to the set, remove it; otherwise, add it; </li><li> after adding or removing the point, print the number of beautiful triples. </li></ul>

## Output

<p>For each query, print one integer — the number of beautiful triples after processing the respective query.</p>





```input1
7 5
8 5 3 2 1 5 6
```




```output1
0
0
1
2
5
1
5
```


