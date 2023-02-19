## Description

<div><p>You are given an array $a$ of length $2^n$. You should process $q$ queries on it. Each query has one of the following $4$ types: </p><ol> <li> $Replace(x, k)$&nbsp;— change $a_x$ to $k$; </li><li> $Reverse(k)$&nbsp;— reverse each subarray $[(i-1) \cdot 2^k+1, i \cdot 2^k]$ for all $i$ ($i \ge 1$); </li><li> $Swap(k)$&nbsp;— swap subarrays $[(2i-2) \cdot 2^k+1, (2i-1) \cdot 2^k]$ and $[(2i-1) \cdot 2^k+1, 2i \cdot 2^k]$ for all $i$ ($i \ge 1$); </li><li> $Sum(l, r)$&nbsp;— print the sum of the elements of subarray $[l, r]$. </li></ol><p>Write a program that can quickly process given queries.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $q$ ($0 \le n \le 18$; $1 \le q \le 10^5$)&nbsp;— the length of array $a$ and the number of queries.</p><p>The second line contains $2^n$ integers $a_1, a_2, \ldots, a_{2^n}$ ($0 \le a_i \le 10^9$).</p><p>Next $q$ lines contains queries&nbsp;— one per line. Each query has one of $4$ types: </p><ul> <li> "$1$ $x$ $k$" ($1 \le x \le 2^n$; $0 \le k \le 10^9$)&nbsp;— $Replace(x, k)$; </li><li> "$2$ $k$" ($0 \le k \le n$)&nbsp;— $Reverse(k)$; </li><li> "$3$ $k$" ($0 \le k &lt; n$)&nbsp;— $Swap(k)$; </li><li> "$4$ $l$ $r$" ($1 \le l \le r \le 2^n$)&nbsp;— $Sum(l, r)$. </li></ul><p>It is guaranteed that there is at least one $Sum$ query.</p></div><div class="output-specification"><p>Print the answer for each $Sum$ query.</p></div>

## Input

<p>The first line contains two integers $n$, $q$ ($0 \le n \le 18$; $1 \le q \le 10^5$)&nbsp;— the length of array $a$ and the number of queries.</p><p>The second line contains $2^n$ integers $a_1, a_2, \ldots, a_{2^n}$ ($0 \le a_i \le 10^9$).</p><p>Next $q$ lines contains queries&nbsp;— one per line. Each query has one of $4$ types: </p><ul> <li> "$1$ $x$ $k$" ($1 \le x \le 2^n$; $0 \le k \le 10^9$)&nbsp;— $Replace(x, k)$; </li><li> "$2$ $k$" ($0 \le k \le n$)&nbsp;— $Reverse(k)$; </li><li> "$3$ $k$" ($0 \le k &lt; n$)&nbsp;— $Swap(k)$; </li><li> "$4$ $l$ $r$" ($1 \le l \le r \le 2^n$)&nbsp;— $Sum(l, r)$. </li></ul><p>It is guaranteed that there is at least one $Sum$ query.</p>

## Output

<p>Print the answer for each $Sum$ query.</p>





```input1
2 3
7 4 9 9
1 2 8
3 1
4 2 4
```




```input2
3 8
7 0 8 8 7 1 5 2
4 3 7
2 1
3 2
4 1 6
2 3
1 5 16
4 8 8
3 0
```




```output1
24
```




```output2
29
22
1
```



## Note

<p>In the first sample, initially, the array $a$ is equal to $\{7,4,9,9\}$.</p><p>After processing the first query. the array $a$ becomes $\{7,8,9,9\}$.</p><p>After processing the second query, the array $a_i$ becomes $\{9,9,7,8\}$</p><p>Therefore, the answer to the third query is $9+7+8=24$.</p><p>In the second sample, initially, the array $a$ is equal to $\{7,0,8,8,7,1,5,2\}$. What happens next is: </p><ol> <li> $Sum(3, 7)$ $\to$ $8 + 8 + 7 + 1 + 5 = 29$; </li><li> $Reverse(1)$ $\to$ $\{0,7,8,8,1,7,2,5\}$; </li><li> $Swap(2)$ $\to$ $\{1,7,2,5,0,7,8,8\}$; </li><li> $Sum(1, 6)$ $\to$ $1 + 7 + 2 + 5 + 0 + 7 = 22$; </li><li> $Reverse(3)$ $\to$ $\{8,8,7,0,5,2,7,1\}$; </li><li> $Replace(5, 16)$ $\to$ $\{8,8,7,0,16,2,7,1\}$; </li><li> $Sum(8, 8)$ $\to$ $1$; </li><li> $Swap(0)$ $\to$ $\{8,8,0,7,2,16,1,7\}$. </li></ol>
