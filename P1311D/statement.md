## Description

<div><p>You are given three integers $a \le b \le c$.</p><p>In one move, you can add $+1$ or $-1$ to <span class="tex-font-style-bf">any</span> of these integers (i.e. increase or decrease any number by one). You can perform such operation any (possibly, zero) number of times, you can even perform this operation several times with one number. <span class="tex-font-style-bf">Note that you cannot make non-positive numbers using such operations</span>.</p><p>You have to perform the minimum number of such operations in order to obtain three integers $A \le B \le C$ such that $B$ is divisible by $A$ and $C$ is divisible by $B$.</p><p>You have to answer $t$ independent test cases. </p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The next $t$ lines describe test cases. Each test case is given on a separate line as three space-separated integers $a, b$ and $c$ ($1 \le a \le b \le c \le 10^4$).</p></div><div class="output-specification"><p>For each test case, print the answer. In the first line print $res$ — the minimum number of operations you have to perform to obtain three integers $A \le B \le C$ such that $B$ is divisible by $A$ and $C$ is divisible by $B$. On the second line print <span class="tex-font-style-bf">any</span> suitable triple $A, B$ and $C$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>The next $t$ lines describe test cases. Each test case is given on a separate line as three space-separated integers $a, b$ and $c$ ($1 \le a \le b \le c \le 10^4$).</p>

## Output

<p>For each test case, print the answer. In the first line print $res$ — the minimum number of operations you have to perform to obtain three integers $A \le B \le C$ such that $B$ is divisible by $A$ and $C$ is divisible by $B$. On the second line print <span class="tex-font-style-bf">any</span> suitable triple $A, B$ and $C$.</p>





```input1
8
1 2 3
123 321 456
5 10 15
15 18 21
100 100 101
1 22 29
3 19 38
6 30 46
```




```output1
1
1 1 3
102
114 228 456
4
4 8 16
6
18 18 18
1
100 100 100
7
1 22 22
2
1 19 38
8
6 24 48
```


