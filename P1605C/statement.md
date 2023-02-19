## Description

<div><p>Ashish has a string $s$ of length $n$ containing only characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>'.</p><p>He wants to find the length of the smallest substring, which satisfies the following conditions: </p><ul> <li> Length of the substring is <span class="tex-font-style-bf">at least</span> $2$ </li><li> '<span class="tex-font-style-tt">a</span>' occurs strictly more times in this substring than '<span class="tex-font-style-tt">b</span>' </li><li> '<span class="tex-font-style-tt">a</span>' occurs strictly more times in this substring than '<span class="tex-font-style-tt">c</span>' </li></ul> <p>Ashish is busy planning his next Codeforces round. Help him solve the problem.</p><p>A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \le t \le 10^{5})$ &nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2 \le n \le 10^{6})$ &nbsp;— the length of the string $s$.</p><p>The second line of each test case contains a string $s$ consisting only of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>'.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^{6}$.</p></div><div class="output-specification"><p>For each test case, output the length of the smallest substring which satisfies the given conditions or print $-1$ if there is no such substring.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \le t \le 10^{5})$ &nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2 \le n \le 10^{6})$ &nbsp;— the length of the string $s$.</p><p>The second line of each test case contains a string $s$ consisting only of characters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>'.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^{6}$.</p>

## Output

<p>For each test case, output the length of the smallest substring which satisfies the given conditions or print $-1$ if there is no such substring.</p>





```input1
3
2
aa
5
cbabb
8
cacabccc
```




```output1
2
-1
3
```



## Note

<p>Consider the first test case. In the substring "<span class="tex-font-style-tt">aa</span>", '<span class="tex-font-style-tt">a</span>' occurs twice, while '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>' occur zero times. Since '<span class="tex-font-style-tt">a</span>' occurs strictly more times than '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>', the substring "<span class="tex-font-style-tt">aa</span>" satisfies the condition and the answer is $2$. The substring "<span class="tex-font-style-tt">a</span>" also satisfies this condition, however its length is not at least $2$.</p><p>In the second test case, it can be shown that in none of the substrings of "<span class="tex-font-style-tt">cbabb</span>" does '<span class="tex-font-style-tt">a</span>' occur strictly more times than '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>' each.</p><p>In the third test case, "<span class="tex-font-style-tt">c<span class="tex-font-style-underline">aca</span>bccc</span>", the length of the smallest substring that satisfies the conditions is $3$.</p>
