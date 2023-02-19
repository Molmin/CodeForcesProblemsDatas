## Description

<div><p>You are given a <span class="tex-font-style-bf">palindromic</span> string $s$ of length $n$.</p><p>You have to count the number of indices $i$ $(1 \le i \le n)$ such that the string after removing $s_i$ from $s$ still remains a palindrome. </p><p>For example, consider $s$ = "<span class="tex-font-style-tt">aba</span>"</p><ol> <li> If we remove $s_1$ from $s$, the string becomes "<span class="tex-font-style-tt">ba</span>" which is not a palindrome. </li><li> If we remove $s_2$ from $s$, the string becomes "<span class="tex-font-style-tt">aa</span>" which is a palindrome. </li><li> If we remove $s_3$ from $s$, the string becomes "<span class="tex-font-style-tt">ab</span>" which is not a palindrome. </li></ol><p>A palindrome is a string that reads the same backward as forward. For example, "<span class="tex-font-style-tt">abba</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">fef</span>" are palindromes whereas "<span class="tex-font-style-tt">codeforces</span>", "<span class="tex-font-style-tt">acd</span>", "<span class="tex-font-style-tt">xy</span>" are not.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line of the input contains a single integer $t$ $(1 \leq t \leq 10^3)$ &nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each testcase contains a single integer $n$ $(2 \leq n \leq 10^5)$ &nbsp;— the length of string $s$.</p><p>The second line of each test case contains a string $s$ consisting of lowercase English letters. <span class="tex-font-style-bf">It is guaranteed that $s$ is a palindrome</span>.</p><p>It is guaranteed that sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer &nbsp;— the number of indices $i$ $(1 \le i \le n)$ such that the string after removing $s_i$ from $s$ still remains a palindrome. </p></div>

## Input

<p>The input consists of multiple test cases. The first line of the input contains a single integer $t$ $(1 \leq t \leq 10^3)$ &nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each testcase contains a single integer $n$ $(2 \leq n \leq 10^5)$ &nbsp;— the length of string $s$.</p><p>The second line of each test case contains a string $s$ consisting of lowercase English letters. <span class="tex-font-style-bf">It is guaranteed that $s$ is a palindrome</span>.</p><p>It is guaranteed that sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer &nbsp;— the number of indices $i$ $(1 \le i \le n)$ such that the string after removing $s_i$ from $s$ still remains a palindrome. </p>





```input1
3
3
aba
8
acaaaaca
2
dd
```




```output1
1
4
2
```



## Note

<p>The first test case is described in the statement.</p><p>In the second test case, the indices $i$ that result in palindrome after removing $s_i$ are $3, 4, 5, 6$. Hence the answer is $4$. </p><p>In the third test case, removal of any of the indices results in "<span class="tex-font-style-tt">d</span>" which is a palindrome. Hence the answer is $2$.</p>
