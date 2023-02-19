## Description

<div><p>You are given the sequence of integers $a_1, a_2, \ldots, a_n$ of length $n$. </p><p>The sequence of indices $i_1 &lt; i_2 &lt; \ldots &lt; i_k$ of length $k$ denotes the subsequence $a_{i_1}, a_{i_2}, \ldots, a_{i_k}$ of length $k$ of sequence $a$.</p><p>The subsequence $a_{i_1}, a_{i_2}, \ldots, a_{i_k}$ of length $k$ of sequence $a$ is called increasing subsequence if $a_{i_j} &lt; a_{i_{j+1}}$ for each $1 \leq j &lt; k$.</p><p>The <span class="tex-font-style-it">weight</span> of the increasing subsequence $a_{i_1}, a_{i_2}, \ldots, a_{i_k}$ of length $k$ of sequence $a$ is the number of $1 \leq j \leq k$, such that exists index $i_k &lt; x \leq n$ and $a_x &gt; a_{i_j}$.</p><p>For example, if $a = [6, 4, 8, 6, 5]$, then the sequence of indices $i = [2, 4]$ denotes increasing subsequence $[4, 6]$ of sequence $a$. The weight of this increasing subsequence is $1$, because for $j = 1$ exists $x = 5$ and $a_5 = 5 &gt; a_{i_1} = 4$, but for $j = 2$ such $x$ doesn't exist.</p><p>Find the sum of weights of all increasing subsequences of $a$ modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the sequence $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the sum of weights of all increasing subsequences $a$ modulo $10^9+7$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the sequence $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the sum of weights of all increasing subsequences $a$ modulo $10^9+7$.</p>





```input1|2,3,6,7
4
5
6 4 8 6 5
4
1 2 3 4
3
3 2 2
4
4 5 6 5
```




```output1
4
12
0
6
```



## Note

<p>In the first test case the following increasing subsequences of $a$ have not zero weight: </p><ul> <li> The weight of $[a_1] = [6]$ is $1$. </li><li> The weight of $[a_2] = [4]$ is $1$. </li><li> The weight of $[a_2, a_3] = [4, 8]$ is $1$. </li><li> The weight of $[a_2, a_4] = [4, 6]$ is $1$. </li></ul> The sum of weights of increasing subsequences is $4$.<p>In the second test case there are $7$ increasing subsequences of $a$ with not zero weight: $3$ with weight $1$, $3$ with weight $2$ and $1$ with weight $3$. The sum of weights is $12$.</p>
