## Description

<div><p>The string $t_1t_2 \dots t_k$ is good if each letter of this string belongs to at least one palindrome of length <span class="tex-font-style-bf">greater</span> than <span class="tex-font-style-tt">1</span>.</p><p>A palindrome is a string that reads the same backward as forward. For example, the strings <span class="tex-font-style-tt">A</span>, <span class="tex-font-style-tt">BAB</span>, <span class="tex-font-style-tt">ABBA</span>, <span class="tex-font-style-tt">BAABBBAAB</span> are palindromes, but the strings <span class="tex-font-style-tt">AB</span>, <span class="tex-font-style-tt">ABBBAA</span>, <span class="tex-font-style-tt">BBBA</span> are not.</p><p>Here are some examples of good strings: </p><ul> <li> $t$ = <span class="tex-font-style-tt">AABBB</span> (letters $t_1$, $t_2$ belong to palindrome $t_1 \dots t_2$ and letters $t_3$, $t_4$, $t_5$ belong to palindrome $t_3 \dots t_5$); </li><li> $t$ = <span class="tex-font-style-tt">ABAA</span> (letters $t_1$, $t_2$, $t_3$ belong to palindrome $t_1 \dots t_3$ and letter $t_4$ belongs to palindrome $t_3 \dots t_4$); </li><li> $t$ = <span class="tex-font-style-tt">AAAAA</span> (all letters belong to palindrome $t_1 \dots t_5$); </li></ul><p>You are given a string $s$ of length $n$, consisting of <span class="tex-font-style-bf">only</span> letters <span class="tex-font-style-tt">A</span> and <span class="tex-font-style-tt">B</span>.</p><p>You have to calculate the number of good substrings of string $s$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 3 \cdot 10^5$) — the length of the string $s$.</p><p>The second line contains the string $s$, consisting of letters <span class="tex-font-style-tt">A</span> and <span class="tex-font-style-tt">B</span>.</p></div><div class="output-specification"><p>Print one integer — the number of good substrings of string $s$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 3 \cdot 10^5$) — the length of the string $s$.</p><p>The second line contains the string $s$, consisting of letters <span class="tex-font-style-tt">A</span> and <span class="tex-font-style-tt">B</span>.</p>

## Output

<p>Print one integer — the number of good substrings of string $s$.</p>





```input1
5
AABBB
```




```input2
3
AAA
```




```input3
7
AAABABB
```




```output1
6
```




```output2
3
```




```output3
15
```



## Note

<p>In the first test case there are six good substrings: $s_1 \dots s_2$, $s_1 \dots s_4$, $s_1 \dots s_5$, $s_3 \dots s_4$, $s_3 \dots s_5$ and $s_4 \dots s_5$.</p><p>In the second test case there are three good substrings: $s_1 \dots s_2$, $s_1 \dots s_3$ and $s_2 \dots s_3$.</p>
