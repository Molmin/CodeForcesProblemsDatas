## Description

<div><p>You are given an integer $n$. Find any string $s$ of length $n$ consisting only of English lowercase letters such that each non-empty substring of $s$ occurs in $s$ an <span class="tex-font-style-bf">odd</span> number of times. If there are multiple such strings, output any. It can be shown that such string always exists under the given constraints.</p><p>A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 500$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line containing the string $s$. If there are multiple such strings, output any. It can be shown that such string always exists under the given constraints.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 500$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single line containing the string $s$. If there are multiple such strings, output any. It can be shown that such string always exists under the given constraints.</p>





```input1
4
3
5
9
19
```




```output1
abc
diane
bbcaabbba
youarethecutestuwuu
```



## Note

<p>In the first test case, each substring of "<span class="tex-font-style-tt">abc</span>" occurs exactly once.</p><p>In the third test case, each substring of "<span class="tex-font-style-tt">bbcaabbba</span>" occurs an odd number of times. In particular, "<span class="tex-font-style-tt">b</span>" occurs $5$ times, "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">bb</span>" occur $3$ times each, and each of the remaining substrings occurs exactly once.</p>
