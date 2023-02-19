## Description

<div><p>You are given two integers $n$ and $m$. Find the $\operatorname{MEX}$ of the sequence $n \oplus 0, n \oplus 1, \ldots, n \oplus m$. Here, $\oplus$ is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operator</a>.</p><p>$\operatorname{MEX}$ of the sequence of non-negative integers is the smallest non-negative integer that doesn't appear in this sequence. For example, $\operatorname{MEX}(0, 1, 2, 4) = 3$, and $\operatorname{MEX}(1, 2021) = 0$. </p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 30\,000$) &nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $n$ and $m$ ($0 \le n, m \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print a single integer &nbsp;— the answer to the problem.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 30\,000$) &nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $n$ and $m$ ($0 \le n, m \le 10^9$).</p>

## Output

<p>For each test case, print a single integer &nbsp;— the answer to the problem.</p>





```input1
5
3 5
4 6
3 2
69 696
123456 654321
```




```output1
4
3
0
640
530866
```



## Note

<p>In the first test case, the sequence is $3 \oplus 0, 3 \oplus 1, 3 \oplus 2, 3 \oplus 3, 3 \oplus 4, 3 \oplus 5$, or $3, 2, 1, 0, 7, 6$. The smallest non-negative integer which isn't present in the sequence i.&nbsp;e. the $\operatorname{MEX}$ of the sequence is $4$.</p><p>In the second test case, the sequence is $4 \oplus 0, 4 \oplus 1, 4 \oplus 2, 4 \oplus 3, 4 \oplus 4, 4 \oplus 5, 4 \oplus 6$, or $4, 5, 6, 7, 0, 1, 2$. The smallest non-negative integer which isn't present in the sequence i.&nbsp;e. the $\operatorname{MEX}$ of the sequence is $3$.</p><p>In the third test case, the sequence is $3 \oplus 0, 3 \oplus 1, 3 \oplus 2$, or $3, 2, 1$. The smallest non-negative integer which isn't present in the sequence i.&nbsp;e. the $\operatorname{MEX}$ of the sequence is $0$.</p>
