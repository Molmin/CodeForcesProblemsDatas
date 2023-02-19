## Description

<div><p><span class="tex-font-style-bf">It is the hard version of the problem. The only difference is that in this version $a_i \le 10^9$.</span></p><p>You are given an array of $n$ integers $a_0, a_1, a_2, \ldots a_{n - 1}$. Bryap wants to find the longest <span class="tex-font-style-bf">beautiful</span> subsequence in the array.</p><p>An array $b = [b_0, b_1, \ldots, b_{m-1}]$, where $0 \le b_0 &lt; b_1 &lt; \ldots &lt; b_{m - 1} &lt; n$, is a subsequence of length $m$ of the array $a$.</p><p>Subsequence $b = [b_0, b_1, \ldots, b_{m-1}]$ of length $m$ is called <span class="tex-font-style-bf">beautiful</span>, if the following condition holds: </p><ul> <li> For any $p$ ($0 \le p &lt; m - 1$) holds: $a_{b_p} \oplus b_{p+1} &lt; a_{b_{p+1}} \oplus b_p$. </li></ul><p>Here $a \oplus b$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of $a$ and $b$. For example, $2 \oplus 4 = 6$ and $3 \oplus 1=2$.</p><p>Bryap is a simple person so he only wants to know the length of the longest such subsequence. Help Bryap and find the answer to his question.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 3 \cdot 10^5$) — the length of the array.</p><p>The second line of each test case contains $n$ integers $a_0,a_1,...,a_{n-1}$ ($0 \leq a_i \leq 10^9$) — the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print a single integer — the length of the longest <span class="tex-font-style-bf">beautiful</span> subsequence.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 3 \cdot 10^5$) — the length of the array.</p><p>The second line of each test case contains $n$ integers $a_0,a_1,...,a_{n-1}$ ($0 \leq a_i \leq 10^9$) — the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case print a single integer — the length of the longest <span class="tex-font-style-bf">beautiful</span> subsequence.</p>





```input1|2,3,6,7
3
2
1 2
5
5 2 4 3 1
10
3 8 8 2 9 1 6 2 8 3
```




```output1
2
3
6
```



## Note

<p>In the first test case, we can pick the whole array as a beautiful subsequence because $1 \oplus 1 &lt; 2 \oplus 0$.</p><p>In the second test case, we can pick elements with indexes $1$, $2$ and $4$ (in $0$ indexation). For this elements holds: $2 \oplus 2 &lt; 4 \oplus 1$ and $4 \oplus 4 &lt; 1 \oplus 2$.</p>
