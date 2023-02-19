## Description

<div><p>On the competitive programming platform CodeCook, every person has a rating graph described by an array of integers $a$ of length $n$. You are now updating the infrastructure, so you've created a program to compress these graphs.</p><p>The program works as follows. Given an integer parameter $k$, the program takes the minimum of each contiguous subarray of length $k$ in $a$.</p><p>More formally, for an array $a$ of length $n$ and an integer $k$, define the $k$-compression array of $a$ as an array $b$ of length $n-k+1$, such that $$b_j =\min_{j\le i\le j+k-1}a_i$$</p><p>For example, the $3$-compression array of $[1, 3, 4, 5, 2]$ is $[\min\{1, 3, 4\}, \min\{3, 4, 5\}, \min\{4, 5, 2\}]=[1, 3, 2].$</p><p>A permutation of length $m$ is an array consisting of $m$ distinct integers from $1$ to $m$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($m=3$ but there is $4$ in the array).</p><p>A $k$-compression array will make CodeCook users happy if it will be a permutation. Given an array $a$, determine for all $1\leq k\leq n$ if CodeCook users will be happy after a $k$-compression of this array or not.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\leq t\leq 10^4$) — the number of test cases.</p><p>The first line of the description of each test case contains a single integer $n$ ($1\leq n\leq 3\cdot 10^5$) — the length of the array.</p><p>The second line of the description of each test case contains $n$ integers $a_1,\ldots,a_n$ ($1\leq a_i\leq n$) — the elements of the array.</p><p>It is guaranteed, that the sum of $n$ for all test cases does not exceed $3\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a binary string of length $n$. </p><p>The $k$-th character of the string should be $1$ if CodeCook users will be happy after a $k$-compression of the array $a$, and $0$ otherwise. </p></div>

## Input

<p>The first line contains a single integer $t$ ($1\leq t\leq 10^4$) — the number of test cases.</p><p>The first line of the description of each test case contains a single integer $n$ ($1\leq n\leq 3\cdot 10^5$) — the length of the array.</p><p>The second line of the description of each test case contains $n$ integers $a_1,\ldots,a_n$ ($1\leq a_i\leq n$) — the elements of the array.</p><p>It is guaranteed, that the sum of $n$ for all test cases does not exceed $3\cdot 10^5$.</p>

## Output

<p>For each test case, print a binary string of length $n$. </p><p>The $k$-th character of the string should be $1$ if CodeCook users will be happy after a $k$-compression of the array $a$, and $0$ otherwise. </p>





```input1
5
5
1 5 3 4 2
4
1 3 2 1
5
1 3 3 3 2
10
1 2 3 4 5 6 7 8 9 10
3
3 3 2
```




```output1
10111
0001
00111
1111111111
000
```



## Note

<p>In the first test case, $a=[1, 5, 3, 4, 2]$.</p><ul> <li> The $1$-compression of $a$ is $[1, 5, 3, 4, 2]$ and it is a permutation. </li><li> The $2$-compression of $a$ is $[1, 3, 3, 2]$ and it is not a permutation, since $3$ appears twice. </li><li> The $3$-compression of $a$ is $[1, 3, 2]$ and it is a permutation. </li><li> The $4$-compression of $a$ is $[1, 2]$ and it is a permutation. </li><li> The $5$-compression of $a$ is $[1]$ and it is a permutation. </li></ul>
