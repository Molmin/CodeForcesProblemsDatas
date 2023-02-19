## Description

<div><p>You are given an integer array $a$ of length $n$. </p><p>Does there exist an array $b$ consisting of $n+1$ positive integers such that $a_i=\gcd (b_i,b_{i+1})$ for all $i$ ($1 \leq i \leq n$)? </p><p>Note that $\gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $x$ and $y$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$) — the length of the array $a$.</p><p>The second line of each test case contains $n$ space-separated integers $a_1,a_2,\ldots,a_n$ representing the array $a$ ($1 \leq a_i \leq 10^4$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if such $b$ exists, otherwise output "<span class="tex-font-style-tt">NO</span>". You can print each letter in any case (upper or lower).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^5$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$) — the length of the array $a$.</p><p>The second line of each test case contains $n$ space-separated integers $a_1,a_2,\ldots,a_n$ representing the array $a$ ($1 \leq a_i \leq 10^4$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if such $b$ exists, otherwise output "<span class="tex-font-style-tt">NO</span>". You can print each letter in any case (upper or lower).</p>





```input1|2,3,6,7
4
1
343
2
4 2
3
4 2 4
4
1 1 1 1
```




```output1
YES
YES
NO
YES
```



## Note

<p>In the first test case, we can take $b=[343,343]$.</p><p>In the second test case, one possibility for $b$ is $b=[12,8,6]$.</p><p>In the third test case, it can be proved that there does not exist any array $b$ that fulfills all the conditions.</p>
