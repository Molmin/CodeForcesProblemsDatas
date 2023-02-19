## Description

<div><p>The position of the leftmost maximum on the segment $[l; r]$ of array $x = [x_1, x_2, \ldots, x_n]$ is the smallest integer $i$ such that $l \le i \le r$ and $x_i = \max(x_l, x_{l+1}, \ldots, x_r)$.</p><p>You are given an array $a = [a_1, a_2, \ldots, a_n]$ of length $n$. Find the number of integer arrays $b = [b_1, b_2, \ldots, b_n]$ of length $n$ that satisfy the following conditions: </p><ul> <li> $1 \le b_i \le m$ for all $1 \le i \le n$; </li><li> for all pairs of integers $1 \le l \le r \le n$, the position of the leftmost maximum on the segment $[l; r]$ of the array $b$ is equal to the position of the leftmost maximum on the segment $[l; r]$ of the array $a$. </li></ul><p>Since the answer might be very large, print its remainder modulo $10^9+7$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^3$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n,m \le 2 \cdot 10^5$, $n \cdot m \le 10^6$).</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le m$)&nbsp;— the array $a$.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases doesn't exceed $10^6$.</p></div><div class="output-specification"><p>For each test case print one integer&nbsp;— the number of arrays $b$ that satisfy the conditions from the statement, modulo $10^9+7$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^3$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n,m \le 2 \cdot 10^5$, $n \cdot m \le 10^6$).</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le m$)&nbsp;— the array $a$.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases doesn't exceed $10^6$.</p>

## Output

<p>For each test case print one integer&nbsp;— the number of arrays $b$ that satisfy the conditions from the statement, modulo $10^9+7$.</p>





```input1|2,3,6,7
4
3 3
1 3 2
4 2
2 2 2 2
6 9
6 9 6 9 6 9
9 100
10 40 20 20 100 60 80 60 60
```




```output1
8
5
11880
351025663
```



## Note

<p>In the first test case, the following $8$ arrays satisfy the conditions from the statement: </p><ul> <li> $[1,2,1]$; </li><li> $[1,2,2]$; </li><li> $[1,3,1]$; </li><li> $[1,3,2]$; </li><li> $[1,3,3]$; </li><li> $[2,3,1]$; </li><li> $[2,3,2]$; </li><li> $[2,3,3]$. </li></ul><p>In the second test case, the following $5$ arrays satisfy the conditions from the statement: </p><ul> <li> $[1,1,1,1]$; </li><li> $[2,1,1,1]$; </li><li> $[2,2,1,1]$; </li><li> $[2,2,2,1]$; </li><li> $[2,2,2,2]$. </li></ul>
