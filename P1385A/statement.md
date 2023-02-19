## Description

<div><p>You are given three positive (i.e. strictly greater than zero) integers $x$, $y$ and $z$.</p><p>Your task is to find positive integers $a$, $b$ and $c$ such that $x = \max(a, b)$, $y = \max(a, c)$ and $z = \max(b, c)$, or determine that it is impossible to find such $a$, $b$ and $c$.</p><p>You have to answer $t$ independent test cases. Print required $a$, $b$ and $c$ in any (arbitrary) order.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains three integers $x$, $y$, and $z$ ($1 \le x, y, z \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print the answer:</p><ul> <li> "<span class="tex-font-style-tt">NO</span>" in the only line of the output if a solution doesn't exist; </li><li> or "<span class="tex-font-style-tt">YES</span>" in the first line and <span class="tex-font-style-bf">any</span> valid triple of positive integers $a$, $b$ and $c$ ($1 \le a, b, c \le 10^9$) in the second line. You can print $a$, $b$ and $c$ <span class="tex-font-style-bf">in any order</span>. </li></ul></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains three integers $x$, $y$, and $z$ ($1 \le x, y, z \le 10^9$).</p>

## Output

<p>For each test case, print the answer:</p><ul> <li> "<span class="tex-font-style-tt">NO</span>" in the only line of the output if a solution doesn't exist; </li><li> or "<span class="tex-font-style-tt">YES</span>" in the first line and <span class="tex-font-style-bf">any</span> valid triple of positive integers $a$, $b$ and $c$ ($1 \le a, b, c \le 10^9$) in the second line. You can print $a$, $b$ and $c$ <span class="tex-font-style-bf">in any order</span>. </li></ul>





```input1
5
3 2 3
100 100 100
50 49 49
10 30 20
1 1000000000 1000000000
```




```output1
YES
3 2 1
YES
100 100 100
NO
NO
YES
1 1 1000000000
```


