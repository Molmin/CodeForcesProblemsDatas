## Description

<div><p>Define the <span class="tex-font-style-it">beauty value</span> of a sequence $b_1,b_2,\ldots,b_c$ as the maximum value of $\sum\limits_{i=1}^{q}b_i + \sum\limits_{i=s}^{t}b_i$, where $q$, $s$, $t$ are all integers and $s &gt; q$ or $t\leq q$. Note that $b_i = 0$ when $i&lt;1$ or $i&gt;c$, $\sum\limits_{i=s}^{t}b_i = 0$ when $s&gt;t$.</p><p>For example, when $b = [-1,-2,-3]$, we may have $q = 0$, $s = 3$, $t = 2$ so the <span class="tex-font-style-it">beauty</span> value is $0 + 0 = 0$. And when $b = [-1,2,-3]$, we have $q = s = t = 2$ so the <span class="tex-font-style-it">beauty</span> value is $1 + 2 = 3$.</p><p>You are given a sequence $a$ of length $n$, determine the sum of the <span class="tex-font-style-it">beauty value</span> of all non-empty subsegments $a_l,a_{l+1},\ldots,a_r$ ($1\leq l\leq r\leq n$) of the sequence $a$.</p><p>Print the answer modulo $998\,244\,353$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $T$ ($1 \le T \le 10^4$) — the number of test cases.</p><p>The first line contains an integer $n$ ($1\le n\le 10^6$) — the length of $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($-10^6 \leq a_i \leq 10^6$) — the given sequence.</p><p>It's guaranteed that the sum of $n$ does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print a line containing a single integer — the answer modulo $998\,244\,353$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $T$ ($1 \le T \le 10^4$) — the number of test cases.</p><p>The first line contains an integer $n$ ($1\le n\le 10^6$) — the length of $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($-10^6 \leq a_i \leq 10^6$) — the given sequence.</p><p>It's guaranteed that the sum of $n$ does not exceed $10^6$.</p>

## Output

<p>For each test case, print a line containing a single integer — the answer modulo $998\,244\,353$.</p>





```input1|2,3,6,7
4
7
80 59 100 -52 -86 -62 75
8
-48 -14 -26 43 -41 34 13 55
1
74
20
56 -60 62 13 88 -48 64 36 -10 19 94 25 -69 88 87 79 -70 74 -26 59
```




```output1
5924
2548
148
98887
```



## Note

<p>In the second test case, for the subsequence $[-26,43,-41,34,13]$, when $q=5$, $s=2$, $t=5$, $\sum\limits_{i=1}^{q}b_i + \sum\limits_{i=s}^{t}b_i = 23 + 49 = 72$.</p><p>In the third test case, there is only one non-empty consecutive subsequence $[74]$. When $q=1$, $s=1$, $t=1$, $\sum\limits_{i=1}^{q}b_i + \sum\limits_{i=s}^{t}b_i = 148$.</p>
