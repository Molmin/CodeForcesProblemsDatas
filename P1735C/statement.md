## Description

<div><p>There was a string $s$ which was supposed to be encrypted. For this reason, all $26$ lowercase English letters were arranged in a circle in some order, afterwards, each letter in $s$ was replaced with the one that follows in clockwise order, in that way the string $t$ was obtained. </p><p>You are given a string $t$. Determine the lexicographically smallest string $s$ that could be a prototype of the given string $t$.</p><p>A string $a$ is lexicographically smaller than a string $b$ of the same length if and only if: </p><ul> <li> in the first position where $a$ and $b$ differ, the string $a$ has a letter, that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul> </div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 3 \cdot 10^4$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10^5$) — the length of the string $t$.</p><p>The next line contains the string $t$ of the length $n$, containing lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single line containing the lexicographically smallest string $s$ which could be a prototype of $t$.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 3 \cdot 10^4$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10^5$) — the length of the string $t$.</p><p>The next line contains the string $t$ of the length $n$, containing lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single line containing the lexicographically smallest string $s$ which could be a prototype of $t$.</p>





```input1|2,3,6,7,10,11
5
1
a
2
ba
10
codeforces
26
abcdefghijklmnopqrstuvwxyz
26
abcdefghijklmnopqrstuvwxzy
```




```output1
b
ac
abcdebfadg
bcdefghijklmnopqrstuvwxyza
bcdefghijklmnopqrstuvwxyaz
```



## Note

<p>In the first test case, we couldn't have the string "<span class="tex-font-style-tt">a</span>", since the letter <span class="tex-font-style-tt">a</span> would transit to itself. Lexicographically the second string "<span class="tex-font-style-tt">b</span>" is suitable as an answer.</p><p>In the second test case, the string "<span class="tex-font-style-tt">aa</span>" is not suitable, since <span class="tex-font-style-tt">a</span> would transit to itself. "<span class="tex-font-style-tt">ab</span>" is not suitable, since the circle would be closed with $2$ letters, but it must contain all $26$. The next string "<span class="tex-font-style-tt">ac</span>" is suitable.</p><p>Below you can see the schemes for the first three test cases. The non-involved letters are skipped, they can be arbitrary placed in the gaps.</p><center> <img class="tex-graphics" src="file://1viN2kT6.png" style="max-width: 100.0%;max-height: 100.0%;" width="832px"> </center>
