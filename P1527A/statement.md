## Description

<div><p>Given an integer $n$, find the maximum value of integer $k$ such that the following condition holds: </p><center> $n$ &amp; ($n-1$) &amp; ($n-2$) &amp; ($n-3$) &amp; ... ($k$) = $0$ </center> where &amp; denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation.</a></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 3 \cdot 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^9$).</p></div><div class="output-specification"><p>For each test case, output a single integer — the required integer $k$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 3 \cdot 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^9$).</p>

## Output

<p>For each test case, output a single integer — the required integer $k$.</p>





```input1
3
2
5
17
```




```output1
1
3
15
```



## Note

<p>In the first testcase, the maximum value for which the continuous &amp; operation gives 0 value, is 1.</p><p>In the second testcase, the maximum value for which the continuous &amp; operation gives 0 value, is 3. No value greater then 3, say for example 4, will give the &amp; sum 0. </p><ul> <li> $5 \, \&amp; \, 4 \neq 0$, </li><li> $5 \, \&amp; \, 4 \, \&amp; \, 3 = 0$. </li></ul><p>Hence, 3 is the answer.</p>
