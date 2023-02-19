## Description

<div><p>You are given two integers $x$ and $y$. You want to choose two <span class="tex-font-style-bf">strictly positive</span> (greater than zero) integers $a$ and $b$, and then apply the following operation to $x$ <span class="tex-font-style-bf">exactly</span> $a$ times: replace $x$ with $b \cdot x$.</p><p>You want to find two positive integers $a$ and $b$ such that $x$ becomes equal to $y$ after this process. If there are multiple possible pairs, you can choose <span class="tex-font-style-bf">any of them</span>. If there is no such pair, report it.</p><p>For example: </p><ul> <li> if $x = 3$ and $y = 75$, you may choose $a = 2$ and $b = 5$, so that $x$ becomes equal to $3 \cdot 5 \cdot 5 = 75$; </li><li> if $x = 100$ and $y = 100$, you may choose $a = 3$ and $b = 1$, so that $x$ becomes equal to $100 \cdot 1 \cdot 1 \cdot 1 = 100$; </li><li> if $x = 42$ and $y = 13$, there is no answer since you cannot decrease $x$ with the given operations. </li></ul></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of one line containing two integers $x$ and $y$ ($1 \le x, y \le 100$).</p></div><div class="output-specification"><p>If it is possible to choose a pair of positive integers $a$ and $b$ so that $x$ becomes $y$ after the aforementioned process, print these two integers. <span class="tex-font-style-bf">The integers you print should be not less than $1$ and not greater than $10^9$</span> (it can be shown that if the answer exists, there is a pair of integers $a$ and $b$ meeting these constraints). If there are multiple such pairs, print any of them.</p><p>If it is impossible to choose a pair of integers $a$ and $b$ so that $x$ becomes $y$, print the integer $0$ twice.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of one line containing two integers $x$ and $y$ ($1 \le x, y \le 100$).</p>

## Output

<p>If it is possible to choose a pair of positive integers $a$ and $b$ so that $x$ becomes $y$ after the aforementioned process, print these two integers. <span class="tex-font-style-bf">The integers you print should be not less than $1$ and not greater than $10^9$</span> (it can be shown that if the answer exists, there is a pair of integers $a$ and $b$ meeting these constraints). If there are multiple such pairs, print any of them.</p><p>If it is impossible to choose a pair of integers $a$ and $b$ so that $x$ becomes $y$, print the integer $0$ twice.</p>





```input1
3
3 75
100 100
42 13
```




```output1
2 5
3 1
0 0
```


