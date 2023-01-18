## Description

<div><p>Consider a sequence of digits of length $2^k$ $[a_1, a_2, \ldots, a_{2^k}]$. We perform the following operation with it: replace pairs $(a_{2i+1}, a_{2i+2})$ with $(a_{2i+1} + a_{2i+2})\bmod 10$ for $0\le i&lt;2^{k-1}$. For every $i$ where $a_{2i+1} + a_{2i+2}\ge 10$ we get a candy! As a result, we will get a sequence of length $2^{k-1}$.</p><p>Less formally, we partition sequence of length $2^k$ into $2^{k-1}$ pairs, each consisting of 2 numbers: the first pair consists of the first and second numbers, the second of the third and fourth $\ldots$, the last pair consists of the ($2^k-1$)-th and ($2^k$)-th numbers. For every pair such that sum of numbers in it is at least $10$, we get a candy. After that, we replace every pair of numbers with a remainder of the division of their sum by $10$ (and don't change the order of the numbers).</p><p>Perform this operation with a resulting array until it becomes of length $1$. Let $f([a_1, a_2, \ldots, a_{2^k}])$ denote the number of candies we get in this process. </p><p>For example: if the starting sequence is $[8, 7, 3, 1, 7, 0, 9, 4]$ then:</p><p>After the first operation the sequence becomes $[(8 + 7)\bmod 10, (3 + 1)\bmod 10, (7 + 0)\bmod 10, (9 + 4)\bmod 10]$ $=$ $[5, 4, 7, 3]$, and we get $2$ candies as $8 + 7 \ge 10$ and $9 + 4 \ge 10$.</p><p>After the second operation the sequence becomes $[(5 + 4)\bmod 10, (7 + 3)\bmod 10]$ $=$ $[9, 0]$, and we get one more candy as $7 + 3 \ge 10$. </p><p>After the final operation sequence becomes $[(9 + 0) \bmod 10]$ $=$ $[9]$. </p><p>Therefore, $f([8, 7, 3, 1, 7, 0, 9, 4]) = 3$ as we got $3$ candies in total.</p><p>You are given a sequence of digits of length $n$ $s_1, s_2, \ldots s_n$. You have to answer $q$ queries of the form $(l_i, r_i)$, where for $i$-th query you have to output $f([s_{l_i}, s_{l_i+1}, \ldots, s_{r_i}])$. It is guaranteed that $r_i-l_i+1$ is of form $2^k$ for some nonnegative integer $k$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the sequence.</p><p>The second line contains $n$ digits $s_1, s_2, \ldots, s_n$ ($0 \le s_i \le 9$).</p><p>The third line contains a single integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contains two integers $l_i$, $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— $i$-th query. It is guaranteed that $r_i-l_i+1$ is a nonnegative integer power of $2$.</p></div><div class="output-specification"><p>Output $q$ lines, in $i$-th line output single integer&nbsp;— $f([s_{l_i}, s_{l_i + 1}, \ldots, s_{r_i}])$, answer to the $i$-th query.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the sequence.</p><p>The second line contains $n$ digits $s_1, s_2, \ldots, s_n$ ($0 \le s_i \le 9$).</p><p>The third line contains a single integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contains two integers $l_i$, $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— $i$-th query. It is guaranteed that $r_i-l_i+1$ is a nonnegative integer power of $2$.</p>

## Output

<p>Output $q$ lines, in $i$-th line output single integer&nbsp;— $f([s_{l_i}, s_{l_i + 1}, \ldots, s_{r_i}])$, answer to the $i$-th query.</p>





```input1
8
8 7 3 1 7 0 9 4
3
1 8
2 5
7 7
```




```input2
6
0 1 2 3 3 5
3
1 2
1 4
3 6
```




```output1
3
1
0
```




```output2
0
0
1
```



## Note

<p>The first example illustrates an example from the statement.</p><p>$f([7, 3, 1, 7]) = 1$: sequence of operations is $[7, 3, 1, 7] \to [(7 + 3)\bmod 10, (1 + 7)\bmod 10]$ $=$ $[0, 8]$ and one candy as $7 + 3 \ge 10$ $\to$ $[(0 + 8) \bmod 10]$ $=$ $[8]$, so we get only $1$ candy.</p><p>$f([9]) = 0$ as we don't perform operations with it.</p>
