## Description

<div><p>You are given two strings $s$ and $t$. The string $s$ consists of lowercase Latin letters and <span class="tex-font-style-bf">at most one</span> wildcard character '<span class="tex-font-style-tt">*</span>', the string $t$ consists only of lowercase Latin letters. The length of the string $s$ equals $n$, the length of the string $t$ equals $m$.</p><p>The wildcard character '<span class="tex-font-style-tt">*</span>' in the string $s$ (if any) can be replaced with an arbitrary sequence (possibly empty) of lowercase Latin letters. No other character of $s$ can be replaced with anything. If it is possible to replace a wildcard character '<span class="tex-font-style-tt">*</span>' in $s$ to obtain a string $t$, then the string $t$ matches the pattern $s$.</p><p>For example, if $s=$"<span class="tex-font-style-tt">aba*aba</span>" then the following strings match it "<span class="tex-font-style-tt">abaaba</span>", "<span class="tex-font-style-tt">abacaba</span>" and "<span class="tex-font-style-tt">abazzzaba</span>", but the following strings do not match: "<span class="tex-font-style-tt">ababa</span>", "<span class="tex-font-style-tt">abcaaba</span>", "<span class="tex-font-style-tt">codeforces</span>", "<span class="tex-font-style-tt">aba1aba</span>", "<span class="tex-font-style-tt">aba?aba</span>".</p><p>If the given string $t$ matches the given string $s$, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) — the length of the string $s$ and the length of the string $t$, respectively.</p><p>The second line contains string $s$ of length $n$, which consists of lowercase Latin letters and <span class="tex-font-style-bf">at most one</span> wildcard character '<span class="tex-font-style-tt">*</span>'.</p><p>The third line contains string $t$ of length $m$, which consists only of lowercase Latin letters.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes), if you can obtain the string $t$ from the string $s$. Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) — the length of the string $s$ and the length of the string $t$, respectively.</p><p>The second line contains string $s$ of length $n$, which consists of lowercase Latin letters and <span class="tex-font-style-bf">at most one</span> wildcard character '<span class="tex-font-style-tt">*</span>'.</p><p>The third line contains string $t$ of length $m$, which consists only of lowercase Latin letters.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes), if you can obtain the string $t$ from the string $s$. Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
6 10
code*s
codeforces

```




```input2
6 5
vk*cup
vkcup

```




```input3
1 1
v
k

```




```input4
9 6
gfgf*gfgf
gfgfgf

```




```output1
YES

```




```output2
YES

```




```output3
NO

```




```output4
NO

```



## Note

<p>In the first example a wildcard character '<span class="tex-font-style-tt">*</span>' can be replaced with a string "<span class="tex-font-style-tt">force</span>". So the string $s$ after this replacement is "<span class="tex-font-style-tt">codeforces</span>" and the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>In the second example a wildcard character '<span class="tex-font-style-tt">*</span>' can be replaced with an empty string. So the string $s$ after this replacement is "<span class="tex-font-style-tt">vkcup</span>" and the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>There is no wildcard character '<span class="tex-font-style-tt">*</span>' in the third example and the strings "<span class="tex-font-style-tt">v</span>" and "<span class="tex-font-style-tt">k</span>" are different so the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>In the fourth example there is no such replacement of a wildcard character '<span class="tex-font-style-tt">*</span>' that you can obtain the string $t$ so the answer is "<span class="tex-font-style-tt">NO</span>".</p>
