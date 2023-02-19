## Description

<div><p>Moamen and Ezzat are playing a game. They create an array $a$ of $n$ non-negative integers where every element is less than $2^k$.</p><p>Moamen wins if $a_1 \,\&amp;\, a_2 \,\&amp;\, a_3 \,\&amp;\, \ldots \,\&amp;\, a_n \ge a_1 \oplus a_2 \oplus a_3 \oplus \ldots \oplus a_n$.</p><p>Here $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>, and $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>Please calculate the number of winning for Moamen arrays $a$.</p><p>As the result may be very large, print the value modulo $1\,000\,000\,007$ ($10^9 + 7$).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 5$)— the number of test cases. </p><p>Each test case consists of one line containing two integers $n$ and $k$ ($1 \le n\le 2\cdot 10^5$, $0 \le k \le 2\cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print a single value — the number of different arrays that Moamen wins with.</p><p>Print the result modulo $1\,000\,000\,007$ ($10^9 + 7$).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 5$)— the number of test cases. </p><p>Each test case consists of one line containing two integers $n$ and $k$ ($1 \le n\le 2\cdot 10^5$, $0 \le k \le 2\cdot 10^5$).</p>

## Output

<p>For each test case, print a single value — the number of different arrays that Moamen wins with.</p><p>Print the result modulo $1\,000\,000\,007$ ($10^9 + 7$).</p>





```input1
3
3 1
2 1
4 0
```




```output1
5
2
1
```



## Note

<p>In the first example, $n = 3$, $k = 1$. As a result, all the possible arrays are $[0,0,0]$, $[0,0,1]$, $[0,1,0]$, $[1,0,0]$, $[1,1,0]$, $[0,1,1]$, $[1,0,1]$, and $[1,1,1]$.</p><p>Moamen wins in only $5$ of them: $[0,0,0]$, $[1,1,0]$, $[0,1,1]$, $[1,0,1]$, and $[1,1,1]$.</p>
