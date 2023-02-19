## Description

<div><p>Bethany would like to tile her bathroom. The bathroom has width $w$ centimeters and length $l$ centimeters. If Bethany simply used the basic tiles of size $1 \times 1$ centimeters, she would use $w \cdot l$ of them. </p><p>However, she has something different in mind. </p><ul> <li> On the interior of the floor she wants to use the $1 \times 1$ tiles. She needs exactly $(w-2) \cdot (l-2)$ of these. </li><li> On the floor boundary she wants to use tiles of size $1 \times a$ for some positive integer $a$. The tiles can also be rotated by $90$ degrees. </li></ul><p>For which values of $a$ can Bethany tile the bathroom floor as described? Note that $a$ can also be $1$. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 100$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>Each test case consist of a single line, which contains two integers $w$, $l$ ($3 \leq w, l \leq 10^{9}$) — the dimensions of the bathroom.</p></div><div class="output-specification"><p>For each test case, print an integer $k$ ($0\le k$) — the number of valid values of $a$ for the given test case — followed by $k$ integers $a_1, a_2,\dots, a_k$ ($1\le a_i$) — the valid values of $a$. The values $a_1, a_2, \dots, a_k$ have to be sorted from smallest to largest.</p><p>It is guaranteed that under the problem constraints, the output contains at most $200\,000$ integers. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 100$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>Each test case consist of a single line, which contains two integers $w$, $l$ ($3 \leq w, l \leq 10^{9}$) — the dimensions of the bathroom.</p>

## Output

<p>For each test case, print an integer $k$ ($0\le k$) — the number of valid values of $a$ for the given test case — followed by $k$ integers $a_1, a_2,\dots, a_k$ ($1\le a_i$) — the valid values of $a$. The values $a_1, a_2, \dots, a_k$ have to be sorted from smallest to largest.</p><p>It is guaranteed that under the problem constraints, the output contains at most $200\,000$ integers. </p>





```input1
3
3 5
12 12
314159265 358979323
```




```output1
3 1 2 3
3 1 2 11
2 1 2
```



## Note

<p>In the <span class="tex-font-style-bf">first test case</span>, the bathroom is $3$ centimeters wide and $5$ centimeters long. There are three values of $a$ such that Bethany can tile the floor as described in the statement, namely $a=1$, $a=2$ and $a=3$. The three tilings are represented in the following pictures. </p><center> <img class="tex-graphics" src="file://iHpsnRw5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
