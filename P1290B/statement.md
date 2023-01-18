## Description

<div><p>Let's call two strings $s$ and $t$ <span class="tex-font-style-it">anagrams</span> of each other if it is possible to rearrange symbols in the string $s$ to get a string, equal to $t$.</p><p>Let's consider two strings $s$ and $t$ <span class="tex-font-style-bf">which are anagrams of each other</span>. We say that $t$ is a <span class="tex-font-style-it">reducible anagram</span> of $s$ if there exists an integer $k \ge 2$ and $2k$ non-empty strings $s_1, t_1, s_2, t_2, \dots, s_k, t_k$ that satisfy the following conditions:</p><ol> <li> If we write the strings $s_1, s_2, \dots, s_k$ in order, the resulting string will be equal to $s$; </li><li> If we write the strings $t_1, t_2, \dots, t_k$ in order, the resulting string will be equal to $t$; </li><li> For all integers $i$ between $1$ and $k$ inclusive, $s_i$ and $t_i$ are anagrams of each other. </li></ol><p>If such strings don't exist, then $t$ is said to be an <span class="tex-font-style-it">irreducible anagram</span> of $s$. <span class="tex-font-style-bf">Note that these notions are only defined when $s$ and $t$ are anagrams of each other</span>.</p><p>For example, consider the string $s = $ "<span class="tex-font-style-tt">gamegame</span>". Then the string $t = $ "<span class="tex-font-style-tt">megamage</span>" is a reducible anagram of $s$, we may choose for example $s_1 = $ "<span class="tex-font-style-tt">game</span>", $s_2 = $ "<span class="tex-font-style-tt">gam</span>", $s_3 = $ "<span class="tex-font-style-tt">e</span>" and $t_1 = $ "<span class="tex-font-style-tt">mega</span>", $t_2 = $ "<span class="tex-font-style-tt">mag</span>", $t_3 = $ "<span class="tex-font-style-tt">e</span>":</p><center> <img class="tex-graphics" src="file://4ew8Y2Xx.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>On the other hand, we can prove that $t = $ "<span class="tex-font-style-tt">memegaga</span>" is an irreducible anagram of $s$.</p><p>You will be given a string $s$ and $q$ queries, represented by two integers $1 \le l \le r \le |s|$ (where $|s|$ is equal to the length of the string $s$). For each query, you should find if the substring of $s$ formed by characters from the $l$-th to the $r$-th has <span class="tex-font-style-underline">at least one</span> irreducible anagram.</p></div><div class="input-specification"><p>The first line contains a string $s$, consisting of lowercase English characters ($1 \le |s| \le 2 \cdot 10^5$).</p><p>The second line contains a single integer $q$ ($1 \le q \le 10^5$) &nbsp;— the number of queries.</p><p>Each of the following $q$ lines contain two integers $l$ and $r$ ($1 \le l \le r \le |s|$), representing a query for the substring of $s$ formed by characters from the $l$-th to the $r$-th.</p></div><div class="output-specification"><p>For each query, print a single line containing "<span class="tex-font-style-tt">Yes</span>" (without quotes) if the corresponding substring has at least one irreducible anagram, and a single line containing "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line contains a string $s$, consisting of lowercase English characters ($1 \le |s| \le 2 \cdot 10^5$).</p><p>The second line contains a single integer $q$ ($1 \le q \le 10^5$) &nbsp;— the number of queries.</p><p>Each of the following $q$ lines contain two integers $l$ and $r$ ($1 \le l \le r \le |s|$), representing a query for the substring of $s$ formed by characters from the $l$-th to the $r$-th.</p>

## Output

<p>For each query, print a single line containing "<span class="tex-font-style-tt">Yes</span>" (without quotes) if the corresponding substring has at least one irreducible anagram, and a single line containing "<span class="tex-font-style-tt">No</span>" (without quotes) otherwise.</p>





```input1
aaaaa
3
1 1
2 4
5 5
```




```input2
aabbbbbbc
6
1 2
2 4
2 2
1 9
5 7
3 5
```




```output1
Yes
No
Yes
```




```output2
No
Yes
Yes
Yes
No
No
```



## Note

<p>In the first sample, in the first and third queries, the substring is "<span class="tex-font-style-tt">a</span>", which has itself as an irreducible anagram since two or more non-empty strings cannot be put together to obtain "<span class="tex-font-style-tt">a</span>". On the other hand, in the second query, the substring is "<span class="tex-font-style-tt">aaa</span>", which has no irreducible anagrams: its only anagram is itself, and we may choose $s_1 = $ "<span class="tex-font-style-tt">a</span>", $s_2 = $ "<span class="tex-font-style-tt">aa</span>", $t_1 = $ "<span class="tex-font-style-tt">a</span>", $t_2 = $ "<span class="tex-font-style-tt">aa</span>" to show that it is a reducible anagram.</p><p>In the second query of the second sample, the substring is "<span class="tex-font-style-tt">abb</span>", which has, for example, "<span class="tex-font-style-tt">bba</span>" as an irreducible anagram.</p>
