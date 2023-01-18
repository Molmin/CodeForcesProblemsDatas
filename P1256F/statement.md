## Description

<div><p>You are given two strings $s$ and $t$ both of length $n$ and both consisting of lowercase Latin letters.</p><p>In one move, you can choose any length $len$ from $1$ to $n$ and perform the following operation: </p><ul> <li> Choose any contiguous substring of the string $s$ of length $len$ and reverse it; </li><li> <span class="tex-font-style-bf">at the same time</span> choose any contiguous substring of the string $t$ of length $len$ and reverse it as well. </li></ul><p>Note that during one move you reverse <span class="tex-font-style-bf">exactly one</span> substring of the string $s$ and <span class="tex-font-style-bf">exactly one</span> substring of the string $t$.</p><p>Also note that borders of substrings you reverse in $s$ and in $t$ <span class="tex-font-style-bf">can be different</span>, the only restriction is that you reverse the substrings of equal length. For example, if $len=3$ and $n=5$, you can reverse $s[1 \dots 3]$ and $t[3 \dots 5]$, $s[2 \dots 4]$ and $t[2 \dots 4]$, but not $s[1 \dots 3]$ and $t[1 \dots 2]$.</p><p>Your task is to say if it is possible to make strings $s$ and $t$ equal after some (possibly, empty) sequence of moves.</p><p>You have to answer $q$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 10^4$) — the number of test cases. Then $q$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of $s$ and $t$.</p><p>The second line of the test case contains one string $s$ consisting of $n$ lowercase Latin letters.</p><p>The third line of the test case contains one string $t$ consisting of $n$ lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer on it — "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to make strings $s$ and $t$ equal after some (possibly, empty) sequence of moves and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 10^4$) — the number of test cases. Then $q$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the length of $s$ and $t$.</p><p>The second line of the test case contains one string $s$ consisting of $n$ lowercase Latin letters.</p><p>The third line of the test case contains one string $t$ consisting of $n$ lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer on it — "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to make strings $s$ and $t$ equal after some (possibly, empty) sequence of moves and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
4
4
abcd
abdc
5
ababa
baaba
4
asdf
asdg
4
abcd
badc
```




```output1
NO
YES
NO
YES
```


