## Description

<div><p>You are given $n$ patterns $p_1, p_2, \dots, p_n$ and $m$ strings $s_1, s_2, \dots, s_m$. Each pattern $p_i$ consists of $k$ characters that are either lowercase Latin letters or wildcard characters (denoted by underscores). All patterns are pairwise distinct. Each string $s_j$ consists of $k$ lowercase Latin letters.</p><p>A string $a$ matches a pattern $b$ if for each $i$ from $1$ to $k$ either $b_i$ is a wildcard character or $b_i=a_i$.</p><p>You are asked to rearrange the patterns in such a way that the first pattern the $j$-th string matches is $p[mt_j]$. You are allowed to leave the order of the patterns unchanged.</p><p>Can you perform such a rearrangement? If you can, then print any valid order.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $k$ ($1 \le n, m \le 10^5$, $1 \le k \le 4$)&nbsp;— the number of patterns, the number of strings and the length of each pattern and string.</p><p>Each of the next $n$ lines contains a pattern&nbsp;— $k$ characters that are either lowercase Latin letters or underscores. All patterns are pairwise distinct.</p><p>Each of the next $m$ lines contains a string&nbsp;— $k$ lowercase Latin letters, and an integer $mt$ ($1 \le mt \le n$)&nbsp;— the index of the first pattern the corresponding string should match.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" if there is no way to rearrange the patterns in such a way that the first pattern that the $j$-th string matches is $p[mt_j]$.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line. The second line should contain $n$ distinct integers from $1$ to $n$&nbsp;— the order of the patterns. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $k$ ($1 \le n, m \le 10^5$, $1 \le k \le 4$)&nbsp;— the number of patterns, the number of strings and the length of each pattern and string.</p><p>Each of the next $n$ lines contains a pattern&nbsp;— $k$ characters that are either lowercase Latin letters or underscores. All patterns are pairwise distinct.</p><p>Each of the next $m$ lines contains a string&nbsp;— $k$ lowercase Latin letters, and an integer $mt$ ($1 \le mt \le n$)&nbsp;— the index of the first pattern the corresponding string should match.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" if there is no way to rearrange the patterns in such a way that the first pattern that the $j$-th string matches is $p[mt_j]$.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" in the first line. The second line should contain $n$ distinct integers from $1$ to $n$&nbsp;— the order of the patterns. If there are multiple answers, print any of them.</p>





```input1
5 3 4
_b_d
__b_
aaaa
ab__
_bcd
abcd 4
abba 2
dbcd 5
```




```input2
1 1 3
__c
cba 1
```




```input3
2 2 2
a_
_b
ab 1
ab 2
```




```output1
YES
3 2 4 5 1
```




```output2
NO
```




```output3
NO
```



## Note

<p>The order of patterns after the rearrangement in the first example is the following: </p><ul> <li> <span class="tex-font-style-tt">aaaa</span> </li><li> <span class="tex-font-style-tt">__b_</span> </li><li> <span class="tex-font-style-tt">ab__</span> </li><li> <span class="tex-font-style-tt">_bcd</span> </li><li> <span class="tex-font-style-tt">_b_d</span> </li></ul><p>Thus, the first string matches patterns <span class="tex-font-style-tt">ab__</span>, <span class="tex-font-style-tt">_bcd</span>, <span class="tex-font-style-tt">_b_d</span> in that order, the first of them is <span class="tex-font-style-tt">ab__</span>, that is indeed $p[4]$. The second string matches <span class="tex-font-style-tt">__b_</span> and <span class="tex-font-style-tt">ab__</span>, the first of them is <span class="tex-font-style-tt">__b_</span>, that is $p[2]$. The last string matches <span class="tex-font-style-tt">_bcd</span> and <span class="tex-font-style-tt">_b_d</span>, the first of them is <span class="tex-font-style-tt">_bcd</span>, that is $p[5]$.</p><p>The answer to that test is not unique, other valid orders also exist.</p><p>In the second example <span class="tex-font-style-tt">cba</span> doesn't match <span class="tex-font-style-tt">__c</span>, thus, no valid order exists.</p><p>In the third example the order (<span class="tex-font-style-tt">a_</span>, <span class="tex-font-style-tt">_b</span>) makes both strings match pattern $1$ first and the order (<span class="tex-font-style-tt">_b</span>, <span class="tex-font-style-tt">a_</span>) makes both strings match pattern $2$ first. Thus, there is no order that produces the result $1$ and $2$.</p>
