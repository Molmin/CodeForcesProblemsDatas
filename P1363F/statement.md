## Description

<div><p>You are given two strings $s$ and $t$, each of length $n$ and consisting of lowercase Latin alphabets. You want to make $s$ equal to $t$. </p><p>You can perform the following operation on $s$ any number of times to achieve it&nbsp;— </p><ul> <li> Choose any substring of $s$ and rotate it clockwise once, that is, if the selected substring is $s[l,l+1...r]$, then it becomes $s[r,l,l + 1 ... r - 1]$. All the remaining characters of $s$ stay in their position. <p>For example, on rotating the substring $[2,4]$ , string "<span class="tex-font-style-tt">abcde</span>" becomes "<span class="tex-font-style-tt">adbce</span>". </p></li></ul><p>A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p><p>Find the minimum number of operations required to convert $s$ to $t$, or determine that it's impossible.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ $(1\leq t \leq 2000)$&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(1\leq n \leq 2000)$&nbsp;— the length of the strings. </p><p>The second and the third lines contain strings $s$ and $t$ respectively.</p><p>The sum of $n$ over all the test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, output the minimum number of operations to convert $s$ to $t$. If it is not possible to convert $s$ to $t$, output $-1$ instead.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ $(1\leq t \leq 2000)$&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(1\leq n \leq 2000)$&nbsp;— the length of the strings. </p><p>The second and the third lines contain strings $s$ and $t$ respectively.</p><p>The sum of $n$ over all the test cases does not exceed $2000$.</p>

## Output

<p>For each test case, output the minimum number of operations to convert $s$ to $t$. If it is not possible to convert $s$ to $t$, output $-1$ instead.</p>





```input1
6
1
a
a
2
ab
ba
3
abc
cab
3
abc
cba
4
abab
baba
4
abcc
aabc
```




```output1
0
1
1
2
1
-1
```



## Note

<p>For the $1$-st test case, since $s$ and $t$ are equal, you don't need to apply any operation.</p><p>For the $2$-nd test case, you only need to apply one operation on the entire string <span class="tex-font-style-tt">ab</span> to convert it to <span class="tex-font-style-tt">ba</span>.</p><p>For the $3$-rd test case, you only need to apply one operation on the entire string <span class="tex-font-style-tt">abc</span> to convert it to <span class="tex-font-style-tt">cab</span>.</p><p>For the $4$-th test case, you need to apply the operation twice: first on the entire string <span class="tex-font-style-tt">abc</span> to convert it to <span class="tex-font-style-tt">cab</span> and then on the substring of length $2$ beginning at the second character to convert it to <span class="tex-font-style-tt">cba</span>.</p><p>For the $5$-th test case, you only need to apply one operation on the entire string <span class="tex-font-style-tt">abab</span> to convert it to <span class="tex-font-style-tt">baba</span>.</p><p>For the $6$-th test case, it is not possible to convert string $s$ to $t$.</p>
