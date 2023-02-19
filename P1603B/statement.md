## Description

<div><p>YouKn0wWho has two <span class="tex-font-style-bf">even</span> integers $x$ and $y$. Help him to find an integer $n$ such that $1 \le n \le 2 \cdot 10^{18}$ and $n \bmod x = y \bmod n$. Here, $a \bmod b$ denotes the remainder of $a$ after division by $b$. If there are multiple such integers, output any. It can be shown that such an integer always exists under the given constraints.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^5$) &nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $x$ and $y$ ($2 \le x, y \le 10^9$, both are <span class="tex-font-style-bf">even</span>).</p></div><div class="output-specification"><p>For each test case, print a single integer $n$ ($1 \le n \le 2 \cdot 10^{18}$) that satisfies the condition mentioned in the statement. If there are multiple such integers, output any. It can be shown that such an integer always exists under the given constraints.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^5$) &nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $x$ and $y$ ($2 \le x, y \le 10^9$, both are <span class="tex-font-style-bf">even</span>).</p>

## Output

<p>For each test case, print a single integer $n$ ($1 \le n \le 2 \cdot 10^{18}$) that satisfies the condition mentioned in the statement. If there are multiple such integers, output any. It can be shown that such an integer always exists under the given constraints.</p>





```input1
4
4 8
4 2
420 420
69420 42068
```




```output1
4
10
420
9969128
```



## Note

<p>In the first test case, $4 \bmod 4 = 8 \bmod 4 = 0$.</p><p>In the second test case, $10 \bmod 4 = 2 \bmod 10 = 2$.</p><p>In the third test case, $420 \bmod 420 = 420 \bmod 420 = 0$.</p>
