## Description

<div><p>You are given three positive integers $a$, $b$, $c$ ($a &lt; b &lt; c$). You have to find three positive integers $x$, $y$, $z$ such that:</p><p>$$x \bmod y = a,$$ $$y \bmod z = b,$$ $$z \bmod x = c.$$</p><p>Here $p \bmod q$ denotes the remainder from dividing $p$ by $q$. It is possible to show that for such constraints the answer always exists.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>Each test case contains a single line with three integers $a$, $b$, $c$ ($1 \le a &lt; b &lt; c \le 10^8$).</p></div><div class="output-specification"><p>For each test case output three positive integers $x$, $y$, $z$ ($1 \le x, y, z \le 10^{18}$) such that $x \bmod y = a$, $y \bmod z = b$, $z \bmod x = c$.</p><p>You can output any correct answer.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>Each test case contains a single line with three integers $a$, $b$, $c$ ($1 \le a &lt; b &lt; c \le 10^8$).</p>

## Output

<p>For each test case output three positive integers $x$, $y$, $z$ ($1 \le x, y, z \le 10^{18}$) such that $x \bmod y = a$, $y \bmod z = b$, $z \bmod x = c$.</p><p>You can output any correct answer.</p>





```input1
4
1 3 4
127 234 421
2 7 8
59 94 388
```




```output1
12 11 4
1063 234 1484
25 23 8
2221 94 2609
```



## Note

<p>In the first test case:</p><p>$$x \bmod y = 12 \bmod 11 = 1;$$</p><p>$$y \bmod z = 11 \bmod 4 = 3;$$</p><p>$$z \bmod x = 4 \bmod 12 = 4.$$</p>
