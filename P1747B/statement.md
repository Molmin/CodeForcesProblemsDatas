## Description

<div><p>You are given an integer $n$.</p><p>Let's define $s(n)$ as the string "<span class="tex-font-style-tt">BAN</span>" concatenated $n$ times. For example, $s(1)$ = "<span class="tex-font-style-tt">BAN</span>", $s(3)$ = "<span class="tex-font-style-tt">BANBANBAN</span>". Note that the length of the string $s(n)$ is equal to $3n$.</p><p>Consider $s(n)$. You can perform the following operation on $s(n)$ any number of times (possibly zero):</p><ul><li> Select any two distinct indices $i$ and $j$ $(1 \leq i, j \leq 3n, i \ne j)$.</li><li> Then, swap $s(n)_i$ and $s(n)_j$. </li></ul><p>You want the string "<span class="tex-font-style-tt">BAN</span>" to <span class="tex-font-style-bf">not appear</span> in $s(n)$ as a <span class="tex-font-style-bf">subsequence</span>. What's the smallest number of operations you have to do to achieve this? Also, find one such shortest sequence of operations.</p><p>A string $a$ is a subsequence of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ $(1 \leq t \leq 100)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single integer $n$ $(1 \leq n \leq 100)$.</p></div><div class="output-specification"><p>For each test case, in the first line output $m$ ($0 \le m \le 10^5$)&nbsp;— the minimum number of operations required. It's guaranteed that the objective is always achievable in at most $10^5$ operations under the constraints of the problem. </p><p>Then, output $m$ lines. The $k$-th of these lines should contain two integers $i_k$, $j_k$ $(1\leq i_k, j_k \leq 3n, i_k \ne j_k)$ denoting that you want to swap characters at indices $i_k$ and $j_k$ at the $k$-th operation. </p><p>After all $m$ operations, "<span class="tex-font-style-tt">BAN</span>" must not appear in $s(n)$ as a subsequence. </p><p>If there are multiple possible answers, output any.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ $(1 \leq t \leq 100)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single integer $n$ $(1 \leq n \leq 100)$.</p>

## Output

<p>For each test case, in the first line output $m$ ($0 \le m \le 10^5$)&nbsp;— the minimum number of operations required. It's guaranteed that the objective is always achievable in at most $10^5$ operations under the constraints of the problem. </p><p>Then, output $m$ lines. The $k$-th of these lines should contain two integers $i_k$, $j_k$ $(1\leq i_k, j_k \leq 3n, i_k \ne j_k)$ denoting that you want to swap characters at indices $i_k$ and $j_k$ at the $k$-th operation. </p><p>After all $m$ operations, "<span class="tex-font-style-tt">BAN</span>" must not appear in $s(n)$ as a subsequence. </p><p>If there are multiple possible answers, output any.</p>





```input1
2
1
2
```




```output1
1
1 2
1
2 6
```



## Note

<p>In the <span class="tex-font-style-bf">first testcase</span>, $s(1) = $ "<span class="tex-font-style-tt">BAN</span>", we can swap $s(1)_1$ and $s(1)_2$, converting $s(1)$ to "<span class="tex-font-style-tt">ABN</span>", which does not contain "<span class="tex-font-style-tt">BAN</span>" as a subsequence.</p><p>In the <span class="tex-font-style-bf">second testcase</span>, $s(2) = $ "<span class="tex-font-style-tt">BANBAN</span>", we can swap $s(2)_2$ and $s(2)_6$, converting $s(2)$ to "<span class="tex-font-style-tt">BNNBAA</span>", which does not contain "<span class="tex-font-style-tt">BAN</span>" as a subsequence.</p>
