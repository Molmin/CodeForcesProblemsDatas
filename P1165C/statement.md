## Description

<div><p>Let's call (yet again) a string <span class="tex-font-style-bf">good</span> if its length is even, and every character in odd position of this string is different from the next character (the first character is different from the second, the third is different from the fourth, and so on). For example, the strings <span class="tex-font-style-tt">good</span>, <span class="tex-font-style-tt">string</span> and <span class="tex-font-style-tt">xyyx</span> are good strings, and the strings <span class="tex-font-style-tt">bad</span>, <span class="tex-font-style-tt">aa</span> and <span class="tex-font-style-tt">aabc</span> are not good. <span class="tex-font-style-bf">Note that the empty string is considered good</span>.</p><p>You are given a string $s$, you have to delete minimum number of characters from this string so that it becomes good.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of characters in $s$.</p><p>The second line contains the string $s$, consisting of exactly $n$ lowercase Latin letters.</p></div><div class="output-specification"><p>In the first line, print one integer $k$ ($0 \le k \le n$) — the minimum number of characters you have to delete from $s$ to make it good.</p><p>In the second line, print the resulting string $s$. <span class="tex-font-style-bf">If it is empty, you may leave the second line blank, or not print it at all</span>.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of characters in $s$.</p><p>The second line contains the string $s$, consisting of exactly $n$ lowercase Latin letters.</p>

## Output

<p>In the first line, print one integer $k$ ($0 \le k \le n$) — the minimum number of characters you have to delete from $s$ to make it good.</p><p>In the second line, print the resulting string $s$. <span class="tex-font-style-bf">If it is empty, you may leave the second line blank, or not print it at all</span>.</p>





```input1
4
good
```




```input2
4
aabc
```




```input3
3
aaa
```




```output1
0
good
```




```output2
2
ab
```




```output3
3
```


