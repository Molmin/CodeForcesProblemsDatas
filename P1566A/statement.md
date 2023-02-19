## Description

<div><p>You are given two positive integers $n$ and $s$. Find the maximum possible median of an array of $n$ <span class="tex-font-style-bf">non-negative</span> integers (not necessarily distinct), such that the sum of its elements is equal to $s$.</p><p>A <span class="tex-font-style-bf">median</span> of an array of integers of length $m$ is the number standing on the $\lceil {\frac{m}{2}} \rceil$-th (rounding up) position in the non-decreasing ordering of its elements. Positions are numbered starting from $1$. For example, a median of the array $[20,40,20,50,50,30]$ is the $\lceil \frac{m}{2} \rceil$-th element of $[20,20,30,40,50,50]$, so it is $30$. There exist other definitions of the median, but in this problem we use the described definition.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>Each test case contains a single line with two integers $n$ and $s$ ($1 \le n, s \le 10^9$)&nbsp;— the length of the array and the required sum of the elements.</p></div><div class="output-specification"><p>For each test case print a single integer&nbsp;— the maximum possible median.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>Each test case contains a single line with two integers $n$ and $s$ ($1 \le n, s \le 10^9$)&nbsp;— the length of the array and the required sum of the elements.</p>

## Output

<p>For each test case print a single integer&nbsp;— the maximum possible median.</p>





```input1
8
1 5
2 5
3 5
2 1
7 17
4 14
1 1000000000
1000000000 1
```




```output1
5
2
2
0
4
4
1000000000
0
```



## Note

<p>Possible arrays for the first three test cases (in each array the median is underlined):</p><ul> <li> In the first test case $[\underline{5}]$ </li><li> In the second test case $[\underline{2}, 3]$ </li><li> In the third test case $[1, \underline{2}, 2]$ </li></ul>
