## Description

<div><p>You are given an angle $\text{ang}$. </p><p>The Jury asks You to find such <span class="tex-font-style-bf">regular</span> $n$-gon (regular polygon with $n$ vertices) that it has three vertices $a$, $b$ and $c$ (they can be non-consecutive) with $\angle{abc} = \text{ang}$ or report that there is no such $n$-gon.</p><center> <img class="tex-graphics" src="file://3sxXvh3R.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>If there are several answers, print the <span class="tex-font-style-bf">minimal</span> one. It is guarantied that if answer exists then it doesn't exceed $998244353$.</p></div><div class="input-specification"><p>The first line contains single integer $T$ ($1 \le T \le 180$) — the number of queries. </p><p>Each of the next $T$ lines contains one integer $\text{ang}$ ($1 \le \text{ang} &lt; 180$) — the angle measured <span class="tex-font-style-bf">in degrees</span>. </p></div><div class="output-specification"><p>For each query print single integer $n$ ($3 \le n \le 998244353$) — minimal possible number of vertices in the regular $n$-gon or $-1$ if there is no such $n$.</p></div>

## Input

<p>The first line contains single integer $T$ ($1 \le T \le 180$) — the number of queries. </p><p>Each of the next $T$ lines contains one integer $\text{ang}$ ($1 \le \text{ang} &lt; 180$) — the angle measured <span class="tex-font-style-bf">in degrees</span>. </p>

## Output

<p>For each query print single integer $n$ ($3 \le n \le 998244353$) — minimal possible number of vertices in the regular $n$-gon or $-1$ if there is no such $n$.</p>





```input1
4
54
50
2
178
```




```output1
10
18
90
180
```



## Note

<p>The answer for the first query is on the picture above.</p><p>The answer for the second query is reached on a regular $18$-gon. For example, $\angle{v_2 v_1 v_6} = 50^{\circ}$.</p><p>The example angle for the third query is $\angle{v_{11} v_{10} v_{12}} = 2^{\circ}$.</p><p>In the fourth query, minimal possible $n$ is $180$ (not $90$).</p>
