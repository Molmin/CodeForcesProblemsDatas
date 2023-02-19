## Description

<div><p>You are given an array $a$ consisting of $n$ nonnegative integers. </p><p>Let's define the prefix OR array $b$ as the array $b_i = a_1~\mathsf{OR}~a_2~\mathsf{OR}~\dots~\mathsf{OR}~a_i$, where $\mathsf{OR}$ represents the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>. In other words, the array $b$ is formed by computing the $\mathsf{OR}$ of every prefix of $a$.</p><p>You are asked to rearrange the elements of the array $a$ in such a way that its prefix OR array is lexicographically maximum.</p><p>An array $x$ is lexicographically greater than an array $y$ if in the first position where $x$ and $y$ differ, $x_i &gt; y_i$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) — the length of the array $a$.</p><p>The second line of each test case contains $n$ <span class="tex-font-style-bf">nonnegative</span> integers $a_1, \ldots, a_n$ ($0 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print $n$ integers — any rearrangement of the array $a$ that obtains the lexicographically maximum prefix OR array.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) — the length of the array $a$.</p><p>The second line of each test case contains $n$ <span class="tex-font-style-bf">nonnegative</span> integers $a_1, \ldots, a_n$ ($0 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print $n$ integers — any rearrangement of the array $a$ that obtains the lexicographically maximum prefix OR array.</p>





```input1|2,3,6,7,10,11
5
4
1 2 4 8
7
5 1 2 3 4 5 5
2
1 101
6
2 3 4 2 3 4
8
1 4 2 3 4 5 7 1
```




```output1
8 4 2 1 
5 2 1 3 4 5 5 
101 1 
4 3 2 2 3 4 
7 1 4 2 3 4 5 1
```


