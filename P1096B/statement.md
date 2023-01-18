## Description

<div><p>You are given a string $s$ of length $n$ consisting only of lowercase Latin letters.</p><p>A substring of a string is a contiguous subsequence of that string. So, string "<span class="tex-font-style-tt">forces</span>" is substring of string "<span class="tex-font-style-tt">codeforces</span>", but string "<span class="tex-font-style-tt">coder</span>" is not.</p><p>Your task is to calculate the number of ways to remove <span class="tex-font-style-bf">exactly</span> one substring from this string in such a way that <span class="tex-font-style-bf">all</span> remaining characters are <span class="tex-font-style-bf">equal</span> (the number of distinct characters either zero or one).</p><p>It is guaranteed that there is <span class="tex-font-style-bf">at least two</span> different characters in $s$.</p><p>Note that you <span class="tex-font-style-bf">can</span> remove the whole string and it is correct. Also note that you should <span class="tex-font-style-bf">remove at least one character</span>.</p><p>Since the answer can be rather large (not very large though) print it modulo $998244353$.</p><p><span class="tex-font-style-bf">If you are Python programmer, consider using PyPy instead of Python when you submit your code.</span></p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of the string $s$.</p><p>The second line of the input contains the string $s$ of length $n$ consisting only of lowercase Latin letters.</p><p>It is guaranteed that there is <span class="tex-font-style-bf">at least two</span> different characters in $s$.</p></div><div class="output-specification"><p>Print one integer — the number of ways modulo $998244353$ to remove <span class="tex-font-style-bf">exactly</span> one substring from $s$ in such way that <span class="tex-font-style-bf">all</span> remaining characters are <span class="tex-font-style-bf">equal</span>.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of the string $s$.</p><p>The second line of the input contains the string $s$ of length $n$ consisting only of lowercase Latin letters.</p><p>It is guaranteed that there is <span class="tex-font-style-bf">at least two</span> different characters in $s$.</p>

## Output

<p>Print one integer — the number of ways modulo $998244353$ to remove <span class="tex-font-style-bf">exactly</span> one substring from $s$ in such way that <span class="tex-font-style-bf">all</span> remaining characters are <span class="tex-font-style-bf">equal</span>.</p>





```input1
4
abaa
```




```input2
7
aacdeee
```




```input3
2
az
```




```output1
6
```




```output2
6
```




```output3
3
```



## Note

<p>Let $s[l; r]$ be the substring of $s$ from the position $l$ to the position $r$ inclusive.</p><p>Then in the first example you can remove the following substrings: </p><ul> <li> $s[1; 2]$; </li><li> $s[1; 3]$; </li><li> $s[1; 4]$; </li><li> $s[2; 2]$; </li><li> $s[2; 3]$; </li><li> $s[2; 4]$. </li></ul><p>In the second example you can remove the following substrings: </p><ul> <li> $s[1; 4]$; </li><li> $s[1; 5]$; </li><li> $s[1; 6]$; </li><li> $s[1; 7]$; </li><li> $s[2; 7]$; </li><li> $s[3; 7]$. </li></ul><p>In the third example you can remove the following substrings: </p><ul> <li> $s[1; 1]$; </li><li> $s[1; 2]$; </li><li> $s[2; 2]$. </li></ul>
