## Description

<div><p><span class="tex-font-style-it">In order to celebrate Twice's 5th anniversary, Tzuyu and Sana decided to play a game.</span></p><p>Tzuyu gave Sana two integers $a$ and $b$ and a really important quest.</p><p>In order to complete the quest, Sana has to output the smallest possible value of ($a \oplus x$) + ($b \oplus x$) for any given $x$, where $\oplus$ denotes the <a href="http://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^{4}$). Description of the test cases follows.</p><p>The only line of each test case contains two integers $a$ and $b$ ($1 \le a, b \le 10^{9}$).</p></div><div class="output-specification"><p>For each testcase, output the smallest possible value of the given expression.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^{4}$). Description of the test cases follows.</p><p>The only line of each test case contains two integers $a$ and $b$ ($1 \le a, b \le 10^{9}$).</p>

## Output

<p>For each testcase, output the smallest possible value of the given expression.</p>





```input1
6
6 12
4 9
59 832
28 14
4925 2912
1 1
```




```output1
10
13
891
18
6237
0
```



## Note

<p>For the first test case Sana can choose $x=4$ and the value will be ($6 \oplus 4$) + ($12 \oplus 4$) = $2 + 8$ = $10$. It can be shown that this is the smallest possible value.</p>
