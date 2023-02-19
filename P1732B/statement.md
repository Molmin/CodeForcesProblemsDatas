## Description

<div><p>A binary string is a string consisting only of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. You are given a binary string $s_1 s_2 \ldots s_n$. It is necessary to make this string non-decreasing in the least number of operations. In other words, each character should be not less than the previous. In one operation, you can do the following:</p><ul><li> Select an arbitrary index $1 \leq i \leq n$ in the string;</li><li> For all $j \geq i$, change the value in the $j$-th position to the opposite, that is, if $s_j = 1$, then make $s_j = 0$, and vice versa.</li></ul><p>What is the minimum number of operations needed to make the string non-decreasing?</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test cases a single integer $n$ ($1 \leq n \leq 10^5$) — the length of the string.</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer — the minimum number of operations that are needed to make the string non-decreasing.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test cases a single integer $n$ ($1 \leq n \leq 10^5$) — the length of the string.</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer — the minimum number of operations that are needed to make the string non-decreasing.</p>





```input1|2,3,6,7,10,11,14,15
8
1
1
2
10
3
101
4
1100
5
11001
6
100010
10
0000110000
7
0101010
```




```output1
0
1
2
1
2
3
1
5
```



## Note

<p>In the first test case, the string is already non-decreasing.</p><p>In the second test case, you can select $i = 1$ and then $s = \mathtt{01}$.</p><p>In the third test case, you can select $i = 1$ and get $s = \mathtt{010}$, and then select $i = 2$. As a result, we get $s = \mathtt{001}$, that is, a non-decreasing string.</p><p>In the sixth test case, you can select $i = 5$ at the first iteration and get $s = \mathtt{100001}$. Then choose $i = 2$, then $s = \mathtt{111110}$. Then we select $i = 1$, getting the non-decreasing string $s = \mathtt{000001}$.</p>
