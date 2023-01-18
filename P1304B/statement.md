## Description

<div><p>Returning back to problem solving, Gildong is now studying about palindromes. He learned that a <span class="tex-font-style-it">palindrome</span> is a string that is the same as its reverse. For example, strings "<span class="tex-font-style-tt">pop</span>", "<span class="tex-font-style-tt">noon</span>", "<span class="tex-font-style-tt">x</span>", and "<span class="tex-font-style-tt">kkkkkk</span>" are palindromes, while strings "<span class="tex-font-style-tt">moon</span>", "<span class="tex-font-style-tt">tv</span>", and "<span class="tex-font-style-tt">abab</span>" are not. <span class="tex-font-style-bf">An empty string is also a palindrome.</span></p><p>Gildong loves this concept so much, so he wants to play with it. He has $n$ <span class="tex-font-style-it">distinct</span> strings of equal length $m$. He wants to discard some of the strings (possibly none or all) and reorder the remaining strings so that the concatenation becomes a palindrome. He also wants the palindrome to be as long as possible. Please help him find one.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 100$, $1 \le m \le 50$) — the number of strings and the length of each string.</p><p>Next $n$ lines contain a string of length $m$ each, consisting of lowercase Latin letters only. All strings are <span class="tex-font-style-it">distinct</span>.</p></div><div class="output-specification"><p>In the first line, print the length of the longest palindrome string you made.</p><p>In the second line, print that palindrome. If there are multiple answers, print any one of them. If the palindrome is empty, print an empty line or don't print this line at all.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 100$, $1 \le m \le 50$) — the number of strings and the length of each string.</p><p>Next $n$ lines contain a string of length $m$ each, consisting of lowercase Latin letters only. All strings are <span class="tex-font-style-it">distinct</span>.</p>

## Output

<p>In the first line, print the length of the longest palindrome string you made.</p><p>In the second line, print that palindrome. If there are multiple answers, print any one of them. If the palindrome is empty, print an empty line or don't print this line at all.</p>





```input1
3 3
tab
one
bat
```




```input2
4 2
oo
ox
xo
xx
```




```input3
3 5
hello
codef
orces
```




```input4
9 4
abab
baba
abcd
bcde
cdef
defg
wxyz
zyxw
ijji
```




```output1
6
tabbat
```




```output2
6
oxxxxo
```




```output3
0
```




```output4
20
ababwxyzijjizyxwbaba
```



## Note

<p>In the first example, "<span class="tex-font-style-tt">battab</span>" is also a valid answer.</p><p>In the second example, there can be 4 different valid answers including the sample output. We are not going to provide any hints for what the others are.</p><p>In the third example, the empty string is the only valid palindrome string.</p>
