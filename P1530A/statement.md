## Description

<div><p>Let's call a number a <span class="tex-font-style-it">binary decimal</span> if it's a positive integer and all digits in its decimal notation are either $0$ or $1$. For example, $1\,010\,111$ is a binary decimal, while $10\,201$ and $787\,788$ are not.</p><p>Given a number $n$, you are asked to represent $n$ as a sum of some (not necessarily distinct) binary decimals. Compute the smallest number of binary decimals required for that.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$), denoting the number of test cases.</p><p>The only line of each test case contains a single integer $n$ ($1 \le n \le 10^9$), denoting the number to be represented.</p></div><div class="output-specification"><p>For each test case, output the smallest number of binary decimals required to represent $n$ as a sum.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$), denoting the number of test cases.</p><p>The only line of each test case contains a single integer $n$ ($1 \le n \le 10^9$), denoting the number to be represented.</p>

## Output

<p>For each test case, output the smallest number of binary decimals required to represent $n$ as a sum.</p>





```input1
3
121
5
1000000000
```




```output1
2
5
1
```



## Note

<p>In the first test case, $121$ can be represented as $121 = 110 + 11$ or $121 = 111 + 10$.</p><p>In the second test case, $5$ can be represented as $5 = 1 + 1 + 1 + 1 + 1$.</p><p>In the third test case, $1\,000\,000\,000$ is a binary decimal itself, thus the answer is $1$.</p>
