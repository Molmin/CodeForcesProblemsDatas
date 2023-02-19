## Description

<div><p>Everool has a binary string $s$ of length $2n$. Note that a binary string is a string consisting of only characters $0$ and $1$. He wants to partition $s$ into two <span class="tex-font-style-bf">disjoint equal</span> subsequences. He needs your help to do it.</p><p>You are allowed to do the following operation <span class="tex-font-style-bf">exactly</span> once. </p><ul> <li> You can choose any subsequence (<span class="tex-font-style-bf">possibly empty</span>) of $s$ and rotate it right by one position. </li></ul><p>In other words, you can select a sequence of indices $b_1, b_2, \ldots, b_m$, where $1 \le b_1 &lt; b_2 &lt; \ldots &lt; b_m \le 2n$. After that you <span class="tex-font-style-bf">simultaneously</span> set $$s_{b_1} := s_{b_m},$$ $$s_{b_2} := s_{b_1},$$ $$\ldots,$$ $$s_{b_m} := s_{b_{m-1}}.$$</p><p>Can you partition $s$ into two <span class="tex-font-style-bf">disjoint equal</span> subsequences after performing the allowed operation <span class="tex-font-style-bf">exactly</span> once?</p><p>A partition of $s$ into two disjoint equal subsequences $s^p$ and $s^q$ is two <span class="tex-font-style-bf">increasing</span> arrays of indices $p_1, p_2, \ldots, p_n$ and $q_1, q_2, \ldots, q_n$, such that each integer from $1$ to $2n$ is encountered in either $p$ or $q$ exactly once, $s^p = s_{p_1} s_{p_2} \ldots s_{p_n}$, $s^q = s_{q_1} s_{q_2} \ldots s_{q_n}$, and $s^p = s^q$.</p><p>If it is not possible to partition after performing any kind of operation, report $-1$. </p><p>If it is possible to do the operation and partition $s$ into two disjoint subsequences $s^p$ and $s^q$, such that $s^p = s^q$, print elements of $b$ and indices of $s^p$, i.&nbsp;e. the values $p_1, p_2, \ldots, p_n$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$), where $2n$ is the length of the binary string.</p><p>The second line of each test case contains the binary string $s$ of length $2n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, follow the following output format.</p><p>If there is no solution, print $-1$. </p><p>Otherwise,</p><ul> <li> In the first line, print an integer $m$ ($0 \leq m \leq 2n$), followed by $m$ distinct indices $b_1$, $b_2$, ..., $b_m$(in <span class="tex-font-style-bf">increasing</span> order). </li><li> In the second line, print $n$ distinct indices $p_1$, $p_2$, ..., $p_n$ (in <span class="tex-font-style-bf">increasing</span> order). </li></ul><p>If there are multiple solutions, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$), where $2n$ is the length of the binary string.</p><p>The second line of each test case contains the binary string $s$ of length $2n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, follow the following output format.</p><p>If there is no solution, print $-1$. </p><p>Otherwise,</p><ul> <li> In the first line, print an integer $m$ ($0 \leq m \leq 2n$), followed by $m$ distinct indices $b_1$, $b_2$, ..., $b_m$(in <span class="tex-font-style-bf">increasing</span> order). </li><li> In the second line, print $n$ distinct indices $p_1$, $p_2$, ..., $p_n$ (in <span class="tex-font-style-bf">increasing</span> order). </li></ul><p>If there are multiple solutions, print any.</p>





```input1
4
2
1010
3
100010
2
1111
2
1110
```




```output1
0
1 2
2 3 5
1 2 5
3 2 3 4
1 4
-1
```



## Note

<p>In the first test case, $b$ is empty. So string $s$ is not changed. Now $s^p = s_1 s_2 = \mathtt{10}$, and $s^q = s_3s_4 = \mathtt{10}$.</p><p>In the second test case, $b=[3,5]$. Initially $s_3=\mathtt{0}$, and $s_5=\mathtt{1}$. On performing the operation, we simultaneously set $s_3=\mathtt{1}$, and $s_5=\mathtt{0}$.</p><p>So $s$ is updated to <span class="tex-font-style-tt">101000</span> on performing the operation.</p><p>Now if we take characters at indices $[1,2,5]$ in $s^p$, we get $s_1=\mathtt{100}$. Also characters at indices $[3,4,6]$ are in $s^q$. Thus $s^q=100$. We are done as $s^p=s^q$.</p><p>In fourth test case, it can be proved that it is not possible to partition the string after performing any operation.</p>
