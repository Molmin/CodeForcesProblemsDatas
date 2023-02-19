## Description

<div><p>AquaMoon has a string $a$ consisting of only $0$ and $1$. She wants to add $+$ and $-$ between all pairs of consecutive positions to make the absolute value of the resulting expression as small as possible. Can you help her?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 2\,000$) &nbsp;– the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 100$) — the length of $a$.</p><p>The second line of each test case contains a string $a$ of length $n$, consisting of only $0$ and $1$.</p></div><div class="output-specification"><p>For each test case, output a string of length $n - 1$ consisting of $-$ and $+$ on a separate line. If there is more than one assignment of signs that produces the smallest possible absolute value, any of them is accepted.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 2\,000$) &nbsp;– the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 100$) — the length of $a$.</p><p>The second line of each test case contains a string $a$ of length $n$, consisting of only $0$ and $1$.</p>

## Output

<p>For each test case, output a string of length $n - 1$ consisting of $-$ and $+$ on a separate line. If there is more than one assignment of signs that produces the smallest possible absolute value, any of them is accepted.</p>





```input1|2,3,6,7
3
2
11
5
01101
5
10001
```




```output1
-
+-++
+++-
```



## Note

<p>In the first test case, we can get the expression $1 - 1 = 0$, with absolute value $0$.</p><p>In the second test case, we can get the expression $0 + 1 - 1 + 0 + 1 = 1$, with absolute value $1$.</p><p>In the third test case, we can get the expression $1 + 0 + 0 + 0 - 1 = 0$, with absolute value $0$.</p>
