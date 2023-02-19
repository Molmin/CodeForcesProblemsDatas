## Description

<div><p>You are given $n$ integers $a_1, a_2, \ldots, a_n$. Find the maximum value of $max(a_l, a_{l + 1}, \ldots, a_r) \cdot min(a_l, a_{l + 1}, \ldots, a_r)$ over all pairs $(l, r)$ of integers for which $1 \le l &lt; r \le n$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer &nbsp;— the maximum possible value of the product from the statement.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer &nbsp;— the maximum possible value of the product from the statement.</p>





```input1
4
3
2 4 3
4
3 2 3 1
2
69 69
6
719313 273225 402638 473783 804745 323328
```




```output1
12
6
4761
381274500335
```



## Note

<p>Let $f(l, r) = max(a_l, a_{l + 1}, \ldots, a_r) \cdot min(a_l, a_{l + 1}, \ldots, a_r)$.</p><p>In the first test case, </p><ul> <li> $f(1, 2) = max(a_1, a_2) \cdot min(a_1, a_2) = max(2, 4) \cdot min(2, 4) = 4 \cdot 2 = 8$. </li><li> $f(1, 3) = max(a_1, a_2, a_3) \cdot min(a_1, a_2, a_3) = max(2, 4, 3) \cdot min(2, 4, 3) = 4 \cdot 2 = 8$. </li><li> $f(2, 3) = max(a_2, a_3) \cdot min(a_2, a_3) = max(4, 3) \cdot min(4, 3) = 4 \cdot 3 = 12$. </li></ul><p>So the maximum is $f(2, 3) = 12$.</p><p>In the second test case, the maximum is $f(1, 2) = f(1, 3) = f(2, 3) = 6$.</p>
