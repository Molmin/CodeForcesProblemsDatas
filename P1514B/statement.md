## Description

<div><p>Baby Badawy's first words were "AND 0 SUM BIG", so he decided to solve the following problem. Given two integers $n$ and $k$, count the number of arrays of length $n$ such that:</p><ul> <li> all its elements are integers between $0$ and $2^k-1$ (inclusive); </li><li> the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND</a> of all its elements is $0$; </li><li> the sum of its elements is as large as possible. </li></ul><p>Since the answer can be very large, print its remainder when divided by $10^9+7$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10$)&nbsp;— the number of test cases you need to solve.</p><p>Each test case consists of a line containing two integers $n$ and $k$ ($1 \le n \le 10^{5}$, $1 \le k \le 20$).</p></div><div class="output-specification"><p>For each test case, print the number of arrays satisfying the conditions. Since the answer can be very large, print its remainder when divided by $10^9+7$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10$)&nbsp;— the number of test cases you need to solve.</p><p>Each test case consists of a line containing two integers $n$ and $k$ ($1 \le n \le 10^{5}$, $1 \le k \le 20$).</p>

## Output

<p>For each test case, print the number of arrays satisfying the conditions. Since the answer can be very large, print its remainder when divided by $10^9+7$.</p>





```input1
2
2 2
100000 20
```




```output1
4
226732710
```



## Note

<p>In the first example, the $4$ arrays are:</p><ul> <li> $[3,0]$, </li><li> $[0,3]$, </li><li> $[1,2]$, </li><li> $[2,1]$. </li></ul>
