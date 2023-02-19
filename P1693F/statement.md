## Description

<div><p>You are given a binary string $S$ of length $n$ indexed from $1$ to $n$. You can perform the following operation any number of times (possibly zero):</p><ul><li><p>Choose two integers $l$ and $r$ ($1 \le l \le r \le n$). Let $cnt_0$ be the number of times <span class="tex-font-style-tt">0</span> occurs in $S[l \ldots r]$ and $cnt_1$ be the number of times <span class="tex-font-style-tt">1</span> occurs in $S[l \ldots r]$. You can pay $|cnt_0 - cnt_1| + 1$ coins and sort the $S[l \ldots r]$. (by $S[l \ldots r]$ we mean the substring of $S$ starting at position $l$ and ending at position $r$)</p><p>For example if $S = $ <span class="tex-font-style-tt">11001</span>, we can perform the operation on $S[2 \ldots 4]$, paying $|2 - 1| + 1 = 2$ coins, and obtain $S = $ <span class="tex-font-style-tt">10011</span> as a new string.</p></li></ul><p>Find the minimum total number of coins required to sort $S$ in increasing order.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the size of $S$.</p><p>The second line of each test case contains a binary string $S$ of $n$ characters $S_1S_2 \ldots S_n$. ($S_i = $ <span class="tex-font-style-tt">0</span> or $S_i = $ <span class="tex-font-style-tt">1</span> for each $1 \le i \le n$)</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the minimum total number of coins required to sort $S$ in increasing order.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the size of $S$.</p><p>The second line of each test case contains a binary string $S$ of $n$ characters $S_1S_2 \ldots S_n$. ($S_i = $ <span class="tex-font-style-tt">0</span> or $S_i = $ <span class="tex-font-style-tt">1</span> for each $1 \le i \le n$)</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the minimum total number of coins required to sort $S$ in increasing order.</p>





```input1|2,3,6,7,10,11,14,15
7
1
1
2
10
3
101
4
1000
5
11010
6
110000
20
01000010001010011000
```




```output1
0
1
1
3
2
2
5
```



## Note

<p>In the first test case, $S$ is already sorted.</p><p>In the second test case, it's enough to apply the operation with $l = 1, r = 2$.</p><p>In the third test case, it's enough to apply the operation with $l = 1, r = 2$.</p>
