## Description

<div><p>There are $n$ piles of sand where the $i$-th pile has $a_i$ blocks of sand. The $i$-th pile is called <span class="tex-font-style-it">too tall</span> if $1 &lt; i &lt; n$ and $a_i &gt; a_{i-1} + a_{i+1}$. That is, a pile is too tall if it has more sand than its two neighbours combined. (Note that piles on the ends of the array cannot be too tall.)</p><p>You are given an integer $k$. An operation consists of picking $k$ consecutive piles of sand and adding one unit of sand to them all. Formally, pick $1 \leq l,r \leq n$ such that $r-l+1=k$. Then for all $l \leq i \leq r$, update $a_i \gets a_i+1$.</p><p>What is the <span class="tex-font-style-bf">maximum</span> number of piles that can simultaneously be too tall after some (possibly zero) operations?</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($3 \leq n \leq 2 \cdot 10^5$; $1 \leq k \leq n$)&nbsp;— the number of piles of sand and the size of the operation, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the sizes of the piles.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the maximum number of piles that are simultaneously too tall after some (possibly zero) operations.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($3 \leq n \leq 2 \cdot 10^5$; $1 \leq k \leq n$)&nbsp;— the number of piles of sand and the size of the operation, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the sizes of the piles.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the maximum number of piles that are simultaneously too tall after some (possibly zero) operations.</p>





```input1|2,3,6,7
3
5 2
2 9 2 4 1
4 4
1 3 2 1
3 1
1 3 1
```




```output1
2
0
1
```



## Note

<p>In the first test case, we can perform the following three operations: </p><ul> <li> Add one unit of sand to piles $1$ and $2$: $[\color{red}{3}, \color{red}{10}, 2, 4, 1]$. </li><li> Add one unit of sand to piles $4$ and $5$: $[3, 10, 2, \color{red}{5}, \color{red}{2}]$. </li><li> Add one unit of sand to piles $3$ and $4$: $[3, 10, \color{red}{3}, \color{red}{6}, 2]$. </li></ul> Now piles $2$ and $4$ are too tall, so in this case the answer is $2$. It can be shown that it is impossible to make more than $2$ piles too tall.<p>In the second test case, any operation will increase all piles by $1$ unit, so the number of too tall piles will always be $0$.</p><p>In the third test case, we can increase any pile by $1$ unit of sand. It can be shown that the maximum number of too tall piles is $1$.</p>
