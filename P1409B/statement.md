## Description

<div><p>You are given four integers $a$, $b$, $x$ and $y$. Initially, $a \ge x$ and $b \ge y$. You can do the following operation <span class="tex-font-style-bf">no more than</span> $n$ times:</p><ul> <li> Choose either $a$ or $b$ and decrease it by one. However, as a result of this operation, value of $a$ cannot become less than $x$, and value of $b$ cannot become less than $y$. </li></ul><p>Your task is to find the <span class="tex-font-style-bf">minimum</span> possible product of $a$ and $b$ ($a \cdot b$) you can achieve by applying the given operation no more than $n$ times.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains five integers $a$, $b$, $x$, $y$ and $n$ ($1 \le a, b, x, y, n \le 10^9$). Additional constraint on the input: $a \ge x$ and $b \ge y$ always holds.</p></div><div class="output-specification"><p>For each test case, print one integer: the <span class="tex-font-style-bf">minimum</span> possible product of $a$ and $b$ ($a \cdot b$) you can achieve by applying the given operation no more than $n$ times.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains five integers $a$, $b$, $x$, $y$ and $n$ ($1 \le a, b, x, y, n \le 10^9$). Additional constraint on the input: $a \ge x$ and $b \ge y$ always holds.</p>

## Output

<p>For each test case, print one integer: the <span class="tex-font-style-bf">minimum</span> possible product of $a$ and $b$ ($a \cdot b$) you can achieve by applying the given operation no more than $n$ times.</p>





```input1
7
10 10 8 5 3
12 8 8 7 2
12343 43 4543 39 123212
1000000000 1000000000 1 1 1
1000000000 1000000000 1 1 1000000000
10 11 2 1 5
10 11 9 1 10
```




```output1
70
77
177177
999999999000000000
999999999
55
10
```



## Note

<p>In the first test case of the example, you need to decrease $b$ three times and obtain $10 \cdot 7 = 70$.</p><p>In the second test case of the example, you need to decrease $a$ one time, $b$ one time and obtain $11 \cdot 7 = 77$.</p><p>In the sixth test case of the example, you need to decrease $a$ five times and obtain $5 \cdot 11 = 55$.</p><p>In the seventh test case of the example, you need to decrease $b$ ten times and obtain $10 \cdot 1 = 10$.</p>
