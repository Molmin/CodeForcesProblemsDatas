## Description

<div><p>Petya and his friend, robot Petya++, like to solve exciting math problems.</p><p>One day Petya++ came up with the numbers $n$ and $x$ and wrote the following equality on the board: $$n\ \&amp;\ (n+1)\ \&amp;\ \dots\ \&amp;\ m = x,$$ where $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>. Then he suggested his friend Petya find such a minimal $m$ ($m \ge n$) that the equality on the board holds.</p><p>Unfortunately, Petya couldn't solve this problem in his head and decided to ask for computer help. He quickly wrote a program and found the answer.</p><p>Can you solve this difficult problem?</p><center> <img class="tex-graphics" src="file://h94YafCl.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2000$). The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$, $x$ ($0\le n, x \le 10^{18}$).</p></div><div class="output-specification"><p>For every test case, output the smallest possible value of $m$ such that equality holds.</p><p>If the equality does not hold for any $m$, print $-1$ instead.</p><p>We can show that if the required $m$ exists, it does not exceed $5 \cdot 10^{18}$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2000$). The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$, $x$ ($0\le n, x \le 10^{18}$).</p>

## Output

<p>For every test case, output the smallest possible value of $m$ such that equality holds.</p><p>If the equality does not hold for any $m$, print $-1$ instead.</p><p>We can show that if the required $m$ exists, it does not exceed $5 \cdot 10^{18}$.</p>





```input1|2,4,6
5
10 8
10 10
10 42
20 16
1000000000000000000 0
```




```output1
12
10
-1
24
1152921504606846976
```



## Note

<p>In the first example, $10\ \&amp;\ 11 = 10$, but $10\ \&amp;\ 11\ \&amp;\ 12 = 8$, so the answer is $12$.</p><p>In the second example, $10 = 10$, so the answer is $10$.</p><p>In the third example, we can see that the required $m$ does not exist, so we have to print $-1$.</p>
