## Description

<div><p>You are given array $a_1, a_2, \dots, a_n$. Find the subsegment $a_l, a_{l+1}, \dots, a_r$ ($1 \le l \le r \le n$) with maximum arithmetic mean $\frac{1}{r - l + 1}\sum\limits_{i=l}^{r}{a_i}$ (in floating-point numbers, i.e. without any rounding).</p><p>If there are many such subsegments find the <span class="tex-font-style-bf">longest</span> one.</p></div><div class="input-specification"><p>The first line contains single integer $n$ ($1 \le n \le 10^5$) — length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$) — the array $a$.</p></div><div class="output-specification"><p>Print the single integer — the length of the longest subsegment with maximum possible arithmetic mean.</p></div>

## Input

<p>The first line contains single integer $n$ ($1 \le n \le 10^5$) — length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$) — the array $a$.</p>

## Output

<p>Print the single integer — the length of the longest subsegment with maximum possible arithmetic mean.</p>





```input1
5
6 1 6 6 0
```




```output1
2
```



## Note

<p>The subsegment $[3, 4]$ is the longest among all subsegments with maximum arithmetic mean.</p>
