## Description

<div><p><span class="tex-font-style-it">Nastia has received an array of $n$ positive integers as a gift</span>.</p><p>She calls such an array $a$ good that for all $i$ ($2 \le i \le n$) takes place $gcd(a_{i - 1}, a_{i}) = 1$, where $gcd(u, v)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $u$ and $v$.</p><p>You can perform the operation: select two <span class="tex-font-style-bf">different</span> indices $i, j$ ($1 \le i, j \le n$, $i \neq j$) and two integers $x, y$ ($1 \le x, y \le 2 \cdot 10^9$) so that $\min{(a_i, a_j)} = \min{(x, y)}$. Then change $a_i$ to $x$ and $a_j$ to $y$.</p><p>The girl asks you to make the array good using <span class="tex-font-style-bf">at most</span> $n$ operations.</p><p>It can be proven that this is always possible.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_{n}$ ($1 \le a_i \le 10^9$)&nbsp;— the array which Nastia has received as a gift.</p><p>It's guaranteed that the sum of $n$ in one test doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each of $t$ test cases print a single integer $k$ ($0 \le k \le n$)&nbsp;— the number of operations. You don't need to minimize this number.</p><p>In each of the next $k$ lines print $4$ integers $i$, $j$, $x$, $y$ ($1 \le i \neq j \le n$, $1 \le x, y \le 2 \cdot 10^9$) so that $\min{(a_i, a_j)} = \min{(x, y)}$&nbsp;— in this manner you replace $a_i$ with $x$ and $a_j$ with $y$.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_{n}$ ($1 \le a_i \le 10^9$)&nbsp;— the array which Nastia has received as a gift.</p><p>It's guaranteed that the sum of $n$ in one test doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each of $t$ test cases print a single integer $k$ ($0 \le k \le n$)&nbsp;— the number of operations. You don't need to minimize this number.</p><p>In each of the next $k$ lines print $4$ integers $i$, $j$, $x$, $y$ ($1 \le i \neq j \le n$, $1 \le x, y \le 2 \cdot 10^9$) so that $\min{(a_i, a_j)} = \min{(x, y)}$&nbsp;— in this manner you replace $a_i$ with $x$ and $a_j$ with $y$.</p><p>If there are multiple answers, print any.</p>





```input1
2
5
9 6 3 11 15
3
7 5 13
```




```output1
2
1 5 11 9
2 5 7 6
0
```



## Note

<p>Consider the first test case.</p><p>Initially $a = [9, 6, 3, 11, 15]$.</p><p>In the first operation replace $a_1$ with $11$ and $a_5$ with $9$. It's valid, because $\min{(a_1, a_5)} = \min{(11, 9)} = 9$.</p><p>After this $a = [11, 6, 3, 11, 9]$.</p><p>In the second operation replace $a_2$ with $7$ and $a_5$ with $6$. It's valid, because $\min{(a_2, a_5)} = \min{(7, 6)} = 6$.</p><p>After this $a = [11, 7, 3, 11, 6]$&nbsp;— a good array.</p><p>In the second test case, the initial array is already good.</p>
