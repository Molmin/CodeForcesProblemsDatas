## Description

<div><p>You are given a string $s$ such that each its character is either <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span>, or <span class="tex-font-style-tt">3</span>. You have to choose the shortest contiguous substring of $s$ such that it contains each of these three characters at least once.</p><p>A contiguous substring of string $s$ is a string that can be obtained from $s$ by removing some (possibly zero) characters from the beginning of $s$ and some (possibly zero) characters from the end of $s$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 20000$) — the number of test cases.</p><p>Each test case consists of one line containing the string $s$ ($1 \le |s| \le 200000$). It is guaranteed that each character of $s$ is either <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span>, or <span class="tex-font-style-tt">3</span>.</p><p>The sum of lengths of all strings in all test cases does not exceed $200000$.</p></div><div class="output-specification"><p>For each test case, print one integer — the length of the shortest contiguous substring of $s$ containing all three types of characters at least once. If there is no such substring, print $0$ instead.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 20000$) — the number of test cases.</p><p>Each test case consists of one line containing the string $s$ ($1 \le |s| \le 200000$). It is guaranteed that each character of $s$ is either <span class="tex-font-style-tt">1</span>, <span class="tex-font-style-tt">2</span>, or <span class="tex-font-style-tt">3</span>.</p><p>The sum of lengths of all strings in all test cases does not exceed $200000$.</p>

## Output

<p>For each test case, print one integer — the length of the shortest contiguous substring of $s$ containing all three types of characters at least once. If there is no such substring, print $0$ instead.</p>





```input1
7
123
12222133333332
112233
332211
12121212
333333
31121
```




```output1
3
3
4
4
0
0
4
```



## Note

<p>Consider the example test:</p><p>In the first test case, the substring <span class="tex-font-style-tt">123</span> can be used.</p><p>In the second test case, the substring <span class="tex-font-style-tt">213</span> can be used.</p><p>In the third test case, the substring <span class="tex-font-style-tt">1223</span> can be used.</p><p>In the fourth test case, the substring <span class="tex-font-style-tt">3221</span> can be used.</p><p>In the fifth test case, there is no character <span class="tex-font-style-tt">3</span> in $s$.</p><p>In the sixth test case, there is no character <span class="tex-font-style-tt">1</span> in $s$.</p><p>In the seventh test case, the substring <span class="tex-font-style-tt">3112</span> can be used.</p>
