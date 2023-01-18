## Description

<div><p>For an array $b$ of length $m$ we define the function $f$ as </p><center> $ f(b) = \begin{cases} b[1] &amp; \quad \text{if } m = 1 \\ f(b[1] \oplus b[2],b[2] \oplus b[3],\dots,b[m-1] \oplus b[m]) &amp; \quad \text{otherwise,} \end{cases} $ </center><p>where $\oplus$ is <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise exclusive OR</a>.</p><p>For example, $f(1,2,4,8)=f(1\oplus2,2\oplus4,4\oplus8)=f(3,6,12)=f(3\oplus6,6\oplus12)=f(5,10)=f(5\oplus10)=f(15)=15$</p><p>You are given an array $a$ and a few queries. Each query is represented as two integers $l$ and $r$. The answer is the maximum value of $f$ on all continuous subsegments of the array $a_l, a_{l+1}, \ldots, a_r$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;— the length of $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2^{30}-1$)&nbsp;— the elements of the array.</p><p>The third line contains a single integer $q$ ($1 \le q \le 100\,000$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contains a query represented as two integers $l$, $r$ ($1 \le l \le r \le n$).</p></div><div class="output-specification"><p>Print $q$ lines&nbsp;— the answers for the queries.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;— the length of $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 2^{30}-1$)&nbsp;— the elements of the array.</p><p>The third line contains a single integer $q$ ($1 \le q \le 100\,000$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contains a query represented as two integers $l$, $r$ ($1 \le l \le r \le n$).</p>

## Output

<p>Print $q$ lines&nbsp;— the answers for the queries.</p>





```input1
3
8 4 1
2
2 3
1 2

```




```input2
6
1 2 4 8 16 32
4
1 6
2 5
3 4
1 2

```




```output1
5
12

```




```output2
60
30
12
3

```



## Note

<p>In first sample in both queries the maximum value of the function is reached on the subsegment that is equal to the whole segment.</p><p>In second sample, optimal segment for first query are $[3,6]$, for second query — $[2,5]$, for third — $[3,4]$, for fourth — $[1,2]$.</p>
