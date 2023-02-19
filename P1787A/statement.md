## Description

<div><p>You are given an integer $n$.</p><p>Find any pair of integers $(x,y)$ ($1\leq x,y\leq n$) such that $x^y\cdot y+y^x\cdot x = n$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\leq t\leq 10^4$) — the number of test cases.</p><p>Each test case contains one line with a single integer $n$ ($1\leq n\leq 10^9$).</p></div><div class="output-specification"><p>For each test case, if possible, print two integers $x$ and $y$ ($1\leq x,y\leq n$). If there are multiple answers, print any.</p><p>Otherwise, print $-1$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\leq t\leq 10^4$) — the number of test cases.</p><p>Each test case contains one line with a single integer $n$ ($1\leq n\leq 10^9$).</p>

## Output

<p>For each test case, if possible, print two integers $x$ and $y$ ($1\leq x,y\leq n$). If there are multiple answers, print any.</p><p>Otherwise, print $-1$.</p>





```input1|2,4,6
5
3
7
42
31250
20732790
```




```output1
-1
-1
2 3
5 5
3 13
```



## Note

<p>In the third test case, $2^3 \cdot 3+3^2 \cdot 2 = 42$, so $(2,3),(3,2)$ will be considered as legal solutions.</p><p>In the fourth test case, $5^5 \cdot 5+5^5 \cdot 5 = 31250$, so $(5,5)$ is a legal solution.</p>
