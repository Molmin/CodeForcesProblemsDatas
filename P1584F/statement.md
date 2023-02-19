## Description

<div><p>You are given $n$ strings $s_1, s_2, \ldots, s_n$, each consisting of lowercase and uppercase English letters. In addition, it's guaranteed that each character occurs in each string <span class="tex-font-style-bf">at most twice</span>. Find the longest common subsequence of these strings.</p><p>A string $t$ is a subsequence of a string $s$ if $t$ can be obtained from $s$ by deletion of several (possibly, zero or all) symbols.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 5$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 10$) — the number of strings.</p><p>Each of the next $n$ lines contains the corresponding string $s_i$. Each $s_i$ is non-empty, consists only of uppercase and lowercase English letters, and no character appears more than twice in each string.</p></div><div class="output-specification"><p>For each test case print the answer in two lines:</p><p>In the first line print the length of the longest common subsequence. </p><p>In the second line print the longest common subsequence. If there are multiple such subsequences, print any of them.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 5$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 10$) — the number of strings.</p><p>Each of the next $n$ lines contains the corresponding string $s_i$. Each $s_i$ is non-empty, consists only of uppercase and lowercase English letters, and no character appears more than twice in each string.</p>

## Output

<p>For each test case print the answer in two lines:</p><p>In the first line print the length of the longest common subsequence. </p><p>In the second line print the longest common subsequence. If there are multiple such subsequences, print any of them.</p>





```input1
4
2
ABC
CBA
2
bacab
defed
3
abcde
aBcDe
ace
2
codeforces
technocup
```




```output1
1
A
0

3
ace
3
coc
```



## Note

<p>In the first test case, the longest common subsequence is "<span class="tex-font-style-tt">A</span>". There are no common subsequences of length $2$.</p><p>In the second test case, sets of characters of strings don't intersect, so any non-empty string can't be a common subsequence.</p>
