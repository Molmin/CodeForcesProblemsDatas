## Description

<div><p>Given an array $a$ of length $n$ and an integer $k$, you are tasked to find any two numbers $l$ and $r$ ($l \leq r$) such that: </p><ul> <li> For each $x$ $(l \leq x \leq r)$, $x$ appears in $a$ at least $k$ times (i.e. $k$ or more array elements are equal to $x$). </li><li> The value $r-l$ is maximized. </li></ul><p>If no numbers satisfy the conditions, output <span class="tex-font-style-tt">-1</span>.</p><p>For example, if $a=[11, 11, 12, 13, 13, 14, 14]$ and $k=2$, then: </p><ul> <li> for $l=12$, $r=14$ the first condition fails because $12$ does not appear at least $k=2$ times. </li><li> for $l=13$, $r=14$ the first condition holds, because $13$ occurs at least $k=2$ times in $a$ and $14$ occurs at least $k=2$ times in $a$. </li><li> for $l=11$, $r=11$ the first condition holds, because $11$ occurs at least $k=2$ times in $a$. </li></ul><p>A pair of $l$ and $r$ for which the first condition holds and $r-l$ is maximal is $l = 13$, $r = 14$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 1000$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains the integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $1 \leq k \leq n$) — the length of the array $a$ and the minimum amount of times each number in the range $[l, r]$ should appear respectively.</p><p>Then a single line follows, containing $n$ integers describing the array $a$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output $2$ numbers, $l$ and $r$ that satisfy the conditions, or "<span class="tex-font-style-tt">-1</span>" if no numbers satisfy the conditions.</p><p>If multiple answers exist, you can output any.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 1000$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains the integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $1 \leq k \leq n$) — the length of the array $a$ and the minimum amount of times each number in the range $[l, r]$ should appear respectively.</p><p>Then a single line follows, containing $n$ integers describing the array $a$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output $2$ numbers, $l$ and $r$ that satisfy the conditions, or "<span class="tex-font-style-tt">-1</span>" if no numbers satisfy the conditions.</p><p>If multiple answers exist, you can output any.</p>





```input1
4
7 2
11 11 12 13 13 14 14
5 1
6 3 5 2 1
6 4
4 3 4 3 3 4
14 2
1 1 2 2 2 3 3 3 3 4 4 4 4 4
```




```output1
13 14
1 3
-1
1 4
```


