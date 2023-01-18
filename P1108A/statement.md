## Description

<div><p>You are given two segments $[l_1; r_1]$ and $[l_2; r_2]$ on the $x$-axis. It is guaranteed that $l_1 &lt; r_1$ and $l_2 &lt; r_2$. Segments <span class="tex-font-style-bf">may intersect, overlap or even coincide with each other</span>.</p><center> <img class="tex-graphics" src="file://SCIolbCn.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The example of two segments on the $x$-axis.</span> </center><p>Your problem is to find two <span class="tex-font-style-bf">integers</span> $a$ and $b$ such that $l_1 \le a \le r_1$, $l_2 \le b \le r_2$ and $a \ne b$. In other words, you have to choose two <span class="tex-font-style-bf">distinct</span> integer points in such a way that the first point belongs to the segment $[l_1; r_1]$ and the second one belongs to the segment $[l_2; r_2]$.</p><p>It is guaranteed that <span class="tex-font-style-bf">the answer exists</span>. If there are multiple answers, you can print <span class="tex-font-style-bf">any</span> of them.</p><p>You have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 500$) — the number of queries.</p><p>Each of the next $q$ lines contains four integers $l_{1_i}, r_{1_i}, l_{2_i}$ and $r_{2_i}$ ($1 \le l_{1_i}, r_{1_i}, l_{2_i}, r_{2_i} \le 10^9, l_{1_i} &lt; r_{1_i}, l_{2_i} &lt; r_{2_i}$) — the ends of the segments in the $i$-th query.</p></div><div class="output-specification"><p>Print $2q$ integers. For the $i$-th query print two integers $a_i$ and $b_i$ — such numbers that $l_{1_i} \le a_i \le r_{1_i}$, $l_{2_i} \le b_i \le r_{2_i}$ and $a_i \ne b_i$. Queries are numbered in order of the input.</p><p>It is guaranteed that <span class="tex-font-style-bf">the answer exists</span>. If there are multiple answers, you can print <span class="tex-font-style-bf">any</span>.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 500$) — the number of queries.</p><p>Each of the next $q$ lines contains four integers $l_{1_i}, r_{1_i}, l_{2_i}$ and $r_{2_i}$ ($1 \le l_{1_i}, r_{1_i}, l_{2_i}, r_{2_i} \le 10^9, l_{1_i} &lt; r_{1_i}, l_{2_i} &lt; r_{2_i}$) — the ends of the segments in the $i$-th query.</p>

## Output

<p>Print $2q$ integers. For the $i$-th query print two integers $a_i$ and $b_i$ — such numbers that $l_{1_i} \le a_i \le r_{1_i}$, $l_{2_i} \le b_i \le r_{2_i}$ and $a_i \ne b_i$. Queries are numbered in order of the input.</p><p>It is guaranteed that <span class="tex-font-style-bf">the answer exists</span>. If there are multiple answers, you can print <span class="tex-font-style-bf">any</span>.</p>





```input1
5
1 2 1 2
2 6 3 4
2 4 1 3
1 2 1 3
1 4 5 8
```




```output1
2 1
3 4
3 2
1 2
3 7
```


