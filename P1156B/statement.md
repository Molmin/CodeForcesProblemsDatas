## Description

<div><p>You are given a string, consisting of lowercase Latin letters.</p><p>A pair of <span class="tex-font-style-bf">neighbouring</span> letters in a string is considered ugly if these letters are also <span class="tex-font-style-bf">neighbouring</span> in a alphabet. For example, string "<span class="tex-font-style-tt">abaca</span>" contains ugly pairs at positions $(1, 2)$ — "<span class="tex-font-style-tt">ab</span>" and $(2, 3)$ — "<span class="tex-font-style-tt">ba</span>". Letters '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">z</span>' aren't considered neighbouring in a alphabet.</p><p>Can you rearrange the letters of a given string so that there are no ugly pairs? You can choose any order of the letters of the given string but you can't add any new letters or remove the existing ones. You can also leave the order the same.</p><p>If there are multiple answers, print any of them.</p><p>You also have to answer $T$ separate queries.</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 100$) — the number of queries.</p><p>Each of the next $T$ lines contains string $s$ $(1 \le |s| \le 100)$ — the string for the next query. It is guaranteed that it contains only lowercase Latin letters.</p><p><span class="tex-font-style-bf">Note that in hacks you have to set $T = 1$</span>.</p></div><div class="output-specification"><p>Print $T$ lines. The $i$-th line should contain the answer to the $i$-th query.</p><p>If the answer for the $i$-th query exists, then print such a rearrangment of letters of the given string that it contains no ugly pairs. You can choose any order of the letters of the given string but you can't add any new letters or remove the existing ones. You can also leave the order the same.</p><p>If there are multiple answers, print any of them.</p><p>Otherwise print "<span class="tex-font-style-tt">No answer</span>" for that query.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 100$) — the number of queries.</p><p>Each of the next $T$ lines contains string $s$ $(1 \le |s| \le 100)$ — the string for the next query. It is guaranteed that it contains only lowercase Latin letters.</p><p><span class="tex-font-style-bf">Note that in hacks you have to set $T = 1$</span>.</p>

## Output

<p>Print $T$ lines. The $i$-th line should contain the answer to the $i$-th query.</p><p>If the answer for the $i$-th query exists, then print such a rearrangment of letters of the given string that it contains no ugly pairs. You can choose any order of the letters of the given string but you can't add any new letters or remove the existing ones. You can also leave the order the same.</p><p>If there are multiple answers, print any of them.</p><p>Otherwise print "<span class="tex-font-style-tt">No answer</span>" for that query.</p>





```input1
4
abcd
gg
codeforces
abaca
```




```output1
cadb
gg
codfoerces
No answer
```



## Note

<p>In the first example answer "<span class="tex-font-style-tt">bdac</span>" is also correct.</p><p>The second example showcases the fact that only neighbouring in alphabet letters are not allowed. The same letter is ok.</p><p>There are lots of valid answers for the third example.</p>
