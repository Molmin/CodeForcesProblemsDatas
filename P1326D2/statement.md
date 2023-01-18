## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The difference is the constraint on the sum of lengths of strings and the number of test cases. You can make hacks only if you solve all versions of this task.</span></p><p>You are given a string $s$, consisting of lowercase English letters. Find the longest string, $t$, which satisfies the following conditions: </p><ul> <li> The length of $t$ does not exceed the length of $s$. </li><li> $t$ is a palindrome. </li><li> There exists two strings $a$ and $b$ (possibly empty), such that $t = a + b$ ( "<span class="tex-font-style-tt">$+$</span>" represents concatenation), and $a$ is prefix of $s$ while $b$ is suffix of $s$. </li></ul></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$), the number of test cases. The next $t$ lines each describe a test case.</p><p>Each test case is a non-empty string $s$, consisting of lowercase English letters.</p><p>It is guaranteed that the sum of lengths of strings over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print the longest string which satisfies the conditions described above. If there exists multiple possible solutions, print any of them.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$), the number of test cases. The next $t$ lines each describe a test case.</p><p>Each test case is a non-empty string $s$, consisting of lowercase English letters.</p><p>It is guaranteed that the sum of lengths of strings over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, print the longest string which satisfies the conditions described above. If there exists multiple possible solutions, print any of them.</p>





```input1
5
a
abcdfdcecba
abbaxyzyx
codeforces
acbba
```




```output1
a
abcdfdcba
xyzyx
c
abba
```



## Note

<p>In the first test, the string $s = $"<span class="tex-font-style-tt">a</span>" satisfies all conditions.</p><p>In the second test, the string "<span class="tex-font-style-tt">abcdfdcba</span>" satisfies all conditions, because:</p><ul> <li> Its length is $9$, which does not exceed the length of the string $s$, which equals $11$. </li><li> It is a palindrome. </li><li> "<span class="tex-font-style-tt">abcdfdcba</span>" $=$ "<span class="tex-font-style-tt">abcdfdc</span>" $+$ "<span class="tex-font-style-tt">ba</span>", and "<span class="tex-font-style-tt">abcdfdc</span>" is a prefix of $s$ while "<span class="tex-font-style-tt">ba</span>" is a suffix of $s$. </li></ul><p>It can be proven that there does not exist a longer string which satisfies the conditions.</p><p>In the fourth test, the string "<span class="tex-font-style-tt">c</span>" is correct, because "<span class="tex-font-style-tt">c</span>" $=$ "<span class="tex-font-style-tt">c</span>" $+$ "<span class="tex-font-style-tt"></span>" and $a$ or $b$ can be empty. The other possible solution for this test is "<span class="tex-font-style-tt">s</span>".</p>
