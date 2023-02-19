## Description

<div><p>You have two strings $s_1$ and $s_2$ of length $n$, consisting of lowercase English letters. You can perform the following operation any (possibly zero) number of times: </p><ul> <li> Choose a positive integer $1 \leq k \leq n$. </li><li> Swap the prefix of the string $s_1$ and the suffix of the string $s_2$ of length $k$. </li></ul><p>Is it possible to make these two strings equal by doing described operations?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then the test cases follow.</p><p>Each test case consists of three lines.</p><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$) — the length of the strings $s_1$ and $s_2$. </p><p>The second line contains the string $s_1$ of length $n$, consisting of lowercase English letters.</p><p>The third line contains the string $s_2$ of length $n$, consisting of lowercase English letters.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if it is possible to make the strings equal, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then the test cases follow.</p><p>Each test case consists of three lines.</p><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$) — the length of the strings $s_1$ and $s_2$. </p><p>The second line contains the string $s_1$ of length $n$, consisting of lowercase English letters.</p><p>The third line contains the string $s_2$ of length $n$, consisting of lowercase English letters.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if it is possible to make the strings equal, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22
7
3
cbc
aba
5
abcaa
cbabb
5
abcaa
cbabz
1
a
a
1
a
b
6
abadaa
adaaba
8
abcabdaa
adabcaba
```




```output1
YES
YES
NO
YES
NO
NO
YES
```



## Note

<p>In the first test case:</p><ul> <li> Initially $s_1 = \mathtt{cbc}$, $s_2 = \mathtt{aba}$. </li><li> Operation with $k = 1$, after the operation $s_1 = \mathtt{abc}$, $s_2 = \mathtt{abc}$. </li></ul><p>In the second test case:</p><ul> <li> Initially $s_1 = \mathtt{abcaa}$, $s_2 = \mathtt{cbabb}$. </li><li> Operation with $k = 2$, after the operation $s_1 = \mathtt{bbcaa}$, $s_2 = \mathtt{cbaab}$. </li><li> Operation with $k = 3$, after the operation $s_1 = \mathtt{aabaa}$, $s_2 = \mathtt{cbbbc}$. </li><li> Operation with $k = 1$, after the operation $s_1 = \mathtt{cabaa}$, $s_2 = \mathtt{cbbba}$. </li><li> Operation with $k = 2$, after the operation $s_1 = \mathtt{babaa}$, $s_2 = \mathtt{cbbca}$. </li><li> Operation with $k = 1$, after the operation $s_1 = \mathtt{aabaa}$, $s_2 = \mathtt{cbbcb}$. </li><li> Operation with $k = 2$, after the operation $s_1 = \mathtt{cbbaa}$, $s_2 = \mathtt{cbbaa}$. </li></ul><p>In the third test case, it's impossible to make strings equal.</p>
