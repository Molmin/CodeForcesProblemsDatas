## Description

<div><p>Let's call a string <span class="tex-font-style-it">balanced</span> if all characters that are present in it appear the same number of times. For example, "<span class="tex-font-style-tt">coder</span>", "<span class="tex-font-style-tt">appall</span>", and "<span class="tex-font-style-tt">ttttttt</span>" are balanced, while "<span class="tex-font-style-tt">wowwow</span>" and "<span class="tex-font-style-tt">codeforces</span>" are not.</p><p>You are given a string $s$ of length $n$ consisting of lowercase English letters. Find a balanced string $t$ of the same length $n$ consisting of lowercase English letters that is different from the string $s$ in as few positions as possible. In other words, the number of indices $i$ such that $s_i \ne t_i$ should be as small as possible.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>Each test case consists of two lines. The first line contains a single integer $n$&nbsp;($1 \le n \le 10^5$)&nbsp;— the length of the string $s$.</p><p>The second line contains the string $s$ of length $n$ consisting of lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print the smallest number of positions where string $s$ and a balanced string $t$ can differ, followed by such a string $t$.</p><p>If there are multiple solutions, print any. It can be shown that at least one balanced string always exists.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>Each test case consists of two lines. The first line contains a single integer $n$&nbsp;($1 \le n \le 10^5$)&nbsp;— the length of the string $s$.</p><p>The second line contains the string $s$ of length $n$ consisting of lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print the smallest number of positions where string $s$ and a balanced string $t$ can differ, followed by such a string $t$.</p><p>If there are multiple solutions, print any. It can be shown that at least one balanced string always exists.</p>





```input1|2,3,6,7
4
5
hello
10
codeforces
5
eevee
6
appall
```




```output1
1
helno
2
codefofced
1
eeeee
0
appall
```



## Note

<p>In the first test case, the given string "<span class="tex-font-style-tt">hello</span>" is not balanced: letters '<span class="tex-font-style-tt">h</span>', '<span class="tex-font-style-tt">e</span>', and '<span class="tex-font-style-tt">o</span>' appear in it once, while letter '<span class="tex-font-style-tt">l</span>' appears twice. On the other hand, string "<span class="tex-font-style-tt">helno</span>" is balanced: five distinct letters are present in it, and each of them appears exactly once. Strings "<span class="tex-font-style-tt">hello</span>" and "<span class="tex-font-style-tt">helno</span>" differ in just one position: the fourth character. Other solutions are possible too.</p><p>In the second test case, string "<span class="tex-font-style-tt">codefofced</span>" is balanced since only letters '<span class="tex-font-style-tt">c</span>', '<span class="tex-font-style-tt">o</span>', '<span class="tex-font-style-tt">d</span>', '<span class="tex-font-style-tt">e</span>', and '<span class="tex-font-style-tt">f</span>' are present in it, and each of them appears exactly twice.</p><p>In the third test case, string "<span class="tex-font-style-tt">eeeee</span>" is balanced since only letter '<span class="tex-font-style-tt">e</span>' is present in it.</p><p>In the fourth test case, the given string "<span class="tex-font-style-tt">appall</span>" is already balanced.</p>
