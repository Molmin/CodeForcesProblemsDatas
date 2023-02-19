## Description

<div><p>The sum of digits of a non-negative integer $a$ is the result of summing up its digits together when written in the decimal system. For example, the sum of digits of $123$ is $6$ and the sum of digits of $10$ is $1$. In a formal way, the sum of digits of $\displaystyle a=\sum_{i=0}^{\infty} a_i \cdot 10^i$, where $0 \leq a_i \leq 9$, is defined as $\displaystyle\sum_{i=0}^{\infty}{a_i}$.</p><p>Given an integer $n$, find two non-negative integers $x$ and $y$ which satisfy the following conditions.</p><ul> <li> $x+y=n$, and </li><li> the sum of digits of $x$ and the sum of digits of $y$ differ by at most $1$. </li></ul><p>It can be shown that such $x$ and $y$ always exist.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). </p><p>Each test case consists of a single integer $n$ ($1 \leq n \leq 10^9$)</p></div><div class="output-specification"><p>For each test case, print two integers $x$ and $y$.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). </p><p>Each test case consists of a single integer $n$ ($1 \leq n \leq 10^9$)</p>

## Output

<p>For each test case, print two integers $x$ and $y$.</p><p>If there are multiple answers, print any.</p>





```input1
5
1
161
67
1206
19
```




```output1
1 0
67 94
60 7
1138 68
14 5
```



## Note

<p>In the second test case, the sum of digits of $67$ and the sum of digits of $94$ are both $13$.</p><p>In the third test case, the sum of digits of $60$ is $6$, and the sum of digits of $7$ is $7$.</p>
