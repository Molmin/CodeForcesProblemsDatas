## Description

<div><p>You are given a binary string $s$ of length $n$. We define a <span class="tex-font-style-it">maximal substring</span> as a substring that cannot be extended while keeping all elements equal. For example, in the string $11000111$ there are three maximal substrings: $11$, $000$ and $111$.</p><p>In one operation, you can select two maximal adjacent substrings. Since they are maximal and adjacent, it's easy to see their elements must have different values. Let $a$ be the length of the sequence of ones and $b$ be the length of the sequence of zeros. Then do the following:</p><ul><li> If $a \ge b$, then replace $b$ selected zeros with $b$ ones. </li><li> If $a &lt; b$, then replace $a$ selected ones with $a$ zeros.</li></ul><p>As an example, for $1110000$ we make it $0000000$, for $0011$ we make it $1111$. We call a string being <span class="tex-font-style-it">good</span> if it can be turned into $1111...1111$ using the aforementioned operation any number of times (possibly, zero). Find the number of good substrings among all $\frac{n(n+1)}{2}$ non-empty substrings of $s$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of the string $s$.</p><p>The second line of each test case contains the binary string $s$ of length $n$. </p><p>It is guaranteed that sum of $n$ across all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer — the number of good substrings.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of the string $s$.</p><p>The second line of each test case contains the binary string $s$ of length $n$. </p><p>It is guaranteed that sum of $n$ across all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer — the number of good substrings.</p>





```input1|2,3,6,7
4
6
100011
3
101
5
11111
6
010101
```




```output1
8
5
15
18
```



## Note

<p>Let's define a substring from index $l$ to index $r$ as $[l, r]$.</p><p>For the first test case, the good substrings are:</p><ul> <li> $[1,1]$, </li><li> $[1,2]$, </li><li> $[3,6]$, </li><li> $[4,5]$, </li><li> $[4,6]$, </li><li> $[5,5]$, </li><li> $[5,6]$, </li><li> $[6,6]$. </li></ul><p>In the second test case, all substrings are good except $[2,2]$.</p><p>In the third test case, all substrings are good.</p>
