## Description

<div><p>Mio has an array $a$ consisting of $n$ integers, and an array $b$ consisting of $m$ integers. </p><p>Mio can do the following operation to $a$:</p><ul> <li> Choose an integer $i$ ($1 \leq i \leq n$) that has <span class="tex-font-style-bf">not</span> been chosen before, then add $1$ to $a_i$, subtract $2$ from $a_{i+1}$, add $3$ to $a_{i+2}$ an so on. Formally, the operation is to add $(-1)^{j-i} \cdot (j-i+1) $ to $a_j$ for $i \leq j \leq n$.</li></ul><p>Mio wants to transform $a$ so that it will contain $b$ as a <span class="tex-font-style-bf">subarray</span>. Could you answer her question, and provide a sequence of operations to do so, if it is possible?</p><p>An array $b$ is a <span class="tex-font-style-bf">subarray</span> of an array $a$ if $b$ can be obtained from $a$ by deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 2 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the test case contains $n$ integers $a_1, a_2, \cdots, a_n$ ($-10^5 \leq a_i \leq 10^5$), where $a_i$ is the $i$-th element of $a$.</p><p>The third line of the test case contains one integer $m$ ($2 \leq m \leq n$) — the number of elements in $b$.</p><p>The fourth line of the test case contains $m$ integers $b_1, b_2, \cdots, b_m$ ($-10^{12} \leq b_i \leq 10^{12}$), where $b_i$ is the $i$-th element of $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>If it is impossible to transform $a$ so that it contains $b$ as a subarray, output $-1$.</p><p>Otherwise, the first line of output should contain an integer $k$ ($0 \leq k \leq n$), the number of operations to be done.</p><p>The second line should contain $k$ distinct integers, representing the operations done in order.</p><p>If there are multiple solutions, you can output any.</p><p>Notice that you do <span class="tex-font-style-bf">not</span> need to minimize the number of operations.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 2 \cdot 10^5$) — the number of elements in $a$.</p><p>The second line of the test case contains $n$ integers $a_1, a_2, \cdots, a_n$ ($-10^5 \leq a_i \leq 10^5$), where $a_i$ is the $i$-th element of $a$.</p><p>The third line of the test case contains one integer $m$ ($2 \leq m \leq n$) — the number of elements in $b$.</p><p>The fourth line of the test case contains $m$ integers $b_1, b_2, \cdots, b_m$ ($-10^{12} \leq b_i \leq 10^{12}$), where $b_i$ is the $i$-th element of $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>If it is impossible to transform $a$ so that it contains $b$ as a subarray, output $-1$.</p><p>Otherwise, the first line of output should contain an integer $k$ ($0 \leq k \leq n$), the number of operations to be done.</p><p>The second line should contain $k$ distinct integers, representing the operations done in order.</p><p>If there are multiple solutions, you can output any.</p><p>Notice that you do <span class="tex-font-style-bf">not</span> need to minimize the number of operations.</p>





```input1
5
5
1 2 3 4 5
5
2 0 6 0 10
5
1 2 3 4 5
3
3 5 3
8
-3 2 -3 -4 4 0 1 -2
4
10 -6 7 -7
5
1 2 3 4 5
4
1 10 1 1
5
0 0 0 0 0
2
10 12
```




```output1
1
1 
1
4 
5
1 3 4 6 8 
-1
-1
```



## Note

<p>In the first test case, the sequence $a$ = $[1,2,3,4,5]$. One of the possible solutions is doing one operation at $i = 1$ (add $1$ to $a_1$, subtract $2$ from $a_2$, add $3$ to $a_3$, subtract $4$ from $a_4$, add $5$ to $a_5$). Then array $a$ is transformed to $a$ = $[2,0,6,0,10]$, which contains $b$ = $[2, 0, 6, 0, 10]$ as a subarray.</p><p>In the second test case, the sequence $a$ = $[1,2,3,4,5]$. One of the possible solutions is doing one operation at $i = 4$ (add $1$ to $a_4$, subtract $2$ from $a_5$). Then array $a$ is transformed to $a$ = $[1,2,3,5,3]$, which contains $b$ = $[3,5,3]$ as a subarray.</p><p>In the third test case, the sequence $a$ = $[-3, 2, -3, -4, 4, 0, 1, -2]$. One of the possible solutions is the following. </p><ul> <li> Choose an integer $i=8$ to do the operation. Then array $a$ is transformed to $a$ = $[-3, 2, -3, -4, 4, 0, 1, -1]$. </li><li> Choose an integer $i=6$ to do the operation. Then array $a$ is transformed to $a$ = $[-3, 2, -3, -4, 4, 1, -1, 2]$. </li><li> Choose an integer $i=4$ to do the operation. Then array $a$ is transformed to $a$ = $[-3, 2, -3, -3, 2, 4, -5, 7]$. </li><li> Choose an integer $i=3$ to do the operation. Then array $a$ is transformed to $a$ = $[-3, 2, -2, -5, 5, 0, 0, 1]$. </li><li> Choose an integer $i=1$ to do the operation. Then array $a$ is transformed to $a$ = $[-2, 0, 1, -9, 10, -6, 7, -7]$. </li></ul><p>The resulting $a$ is $[-2, 0, 1, -9, 10, -6, 7, -7]$, which contains $b$ = $[10, -6, 7, -7]$ as a subarray.</p><p>In the fourth test case, it is impossible to transform $a$ so that it contains $b$ as a subarray.</p><p>In the fifth test case, it is impossible to transform $a$ so that it contains $b$ as a subarray.</p>
