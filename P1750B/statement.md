## Description

<div><p>A binary string is a string consisting only of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. You are given a binary string $s$.</p><p>For some non-empty substring$^\dagger$ $t$ of string $s$ containing $x$ characters <span class="tex-font-style-tt">0</span> and $y$ characters <span class="tex-font-style-tt">1</span>, define its <span class="tex-font-style-it">cost</span> as:</p><ul> <li> $x \cdot y$, if $x &gt; 0$ and $y &gt; 0$; </li><li> $x^2$, if $x &gt; 0$ and $y = 0$; </li><li> $y^2$, if $x = 0$ and $y &gt; 0$. </li></ul><p>Given a binary string $s$ of length $n$, find the maximum cost across all its non-empty substrings.</p><p>$^\dagger$ A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of the string $s$.</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer — the maximum cost across all substrings.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of the string $s$.</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer — the maximum cost across all substrings.</p>





```input1|2,3,6,7,10,11
6
5
11100
7
1100110
6
011110
7
1001010
4
1000
1
0
```




```output1
9
12
16
12
9
1
```



## Note

<p>In the first test case, we can take a substring $111$. It contains $3$ characters <span class="tex-font-style-tt">1</span> and $0$ characters <span class="tex-font-style-tt">0</span>. So $a = 3$, $b = 0$ and its cost is $3^2 = 9$.</p><p>In the second test case, we can take the whole string. It contains $4$ characters <span class="tex-font-style-tt">1</span> and $3$ characters <span class="tex-font-style-tt">0</span>. So $a = 4$, $b = 3$ and its cost is $4 \cdot 3 = 12$.</p><p>In the third test case, we can can take a substring $1111$ and its cost is $4^2 = 16$.</p><p>In the fourth test case, we can take the whole string and cost is $4 \cdot 3 = 12$.</p><p>In the fifth test case, we can take a substring $000$ and its cost is $3 \cdot 3 = 9$.</p><p>In the sixth test case, we can only take the substring $0$ and its cost is $1 \cdot 1 = 1$.</p>
