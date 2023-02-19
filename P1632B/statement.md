## Description

<div><p>It has finally been decided to build a roof over the football field in School 179. Its construction will require placing $n$ consecutive vertical pillars. Furthermore, the headmaster wants the heights of all the pillars to form a permutation $p$ of integers from $0$ to $n - 1$, where $p_i$ is the height of the $i$-th pillar from the left $(1 \le i \le n)$.</p><p>As the chief, you know that the cost of construction of consecutive pillars is equal to <span class="tex-font-style-bf">the maximum value of the bitwise XOR</span> of heights of all pairs of adjacent pillars. In other words, the cost of construction is equal to $\max\limits_{1 \le i \le n - 1}{p_i \oplus p_{i + 1}}$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>Find any sequence of pillar heights $p$ of length $n$ with the smallest construction cost.</p><p>In this problem, a permutation is an array consisting of $n$ distinct integers from $0$ to $n - 1$ in arbitrary order. For example, $[2,3,1,0,4]$ is a permutation, but $[1,0,1]$ is not a permutation ($1$ appears twice in the array) and $[1,0,3]$ is also not a permutation ($n=3$, but $3$ is in the array).</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The only line for each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of pillars for the construction of the roof.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print $n$ integers $p_1$, $p_2$, $\ldots$, $p_n$ — the sequence of pillar heights with the smallest construction cost.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The only line for each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the number of pillars for the construction of the roof.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print $n$ integers $p_1$, $p_2$, $\ldots$, $p_n$ — the sequence of pillar heights with the smallest construction cost.</p><p>If there are multiple answers, print any of them.</p>





```input1|2,4
4
2
3
5
10
```




```output1
0 1
2 0 1
3 2 1 0 4
4 6 3 2 0 8 9 1 7 5
```



## Note

<p>For $n = 2$ there are $2$ sequences of pillar heights: </p><ul> <li> $[0, 1]$ — cost of construction is $0 \oplus 1 = 1$. </li><li> $[1, 0]$ — cost of construction is $1 \oplus 0 = 1$. </li></ul><p>For $n = 3$ there are $6$ sequences of pillar heights: </p><ul> <li> $[0, 1, 2]$ — cost of construction is $\max(0 \oplus 1, 1 \oplus 2) = \max(1, 3) = 3$. </li><li> $[0, 2, 1]$ — cost of construction is $\max(0 \oplus 2, 2 \oplus 1) = \max(2, 3) = 3$. </li><li> $[1, 0, 2]$ — cost of construction is $\max(1 \oplus 0, 0 \oplus 2) = \max(1, 2) = 2$. </li><li> $[1, 2, 0]$ — cost of construction is $\max(1 \oplus 2, 2 \oplus 0) = \max(3, 2) = 3$. </li><li> $[2, 0, 1]$ — cost of construction is $\max(2 \oplus 0, 0 \oplus 1) = \max(2, 1) = 2$. </li><li> $[2, 1, 0]$ — cost of construction is $\max(2 \oplus 1, 1 \oplus 0) = \max(3, 1) = 3$. </li></ul>
