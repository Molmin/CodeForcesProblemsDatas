## Description

<div><p><span class="tex-font-style-it">It is a complicated version of problem F1. The difference between them is the constraints (F1: $k \le 2$, F2: $k \le 10$).</span></p><p>You are given an integer $n$. Find the minimum integer $x$ such that $x \ge n$ and the number $x$ is $k$-<span class="tex-font-style-it">beautiful</span>.</p><p>A number is called $k$-<span class="tex-font-style-it">beautiful</span> if its decimal representation having no leading zeroes contains no more than $k$ different digits. E.g. if $k = 2$, the numbers $3434443$, $55550$, $777$ and $21$ are $k$-<span class="tex-font-style-it">beautiful</span> whereas the numbers $120$, $445435$ and $998244353$ are not.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one line containing two integers $n$ and $k$ ($1 \le n \le 10^9$, $1 \le k \le 10$).</p></div><div class="output-specification"><p>For each test case output on a separate line $x$ — the minimum $k$-<span class="tex-font-style-it">beautiful</span> integer such that $x \ge n$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one line containing two integers $n$ and $k$ ($1 \le n \le 10^9$, $1 \le k \le 10$).</p>

## Output

<p>For each test case output on a separate line $x$ — the minimum $k$-<span class="tex-font-style-it">beautiful</span> integer such that $x \ge n$.</p>





```input1
6
2021 3
177890 2
34512 3
724533 4
998244353 1
12345678 10
```




```output1
2021
181111
34533
724542
999999999
12345678
```


