## Description

<div><p>Hossam has an unweighted tree $G$ with letters in vertices.</p><p>Hossam defines $s(v, \, u)$ as a string that is obtained by writing down all the letters on the unique simple path from the vertex $v$ to the vertex $u$ in the tree $G$.</p><p>A string $a$ is a <span class="tex-font-style-it">subsequence</span> of a string $s$ if $a$ can be obtained from $s$ by deletion of several (possibly, zero) letters. For example, "<span class="tex-font-style-tt">dores</span>", "<span class="tex-font-style-tt">cf</span>", and "<span class="tex-font-style-tt">for</span>" are subsequences of "<span class="tex-font-style-tt">codeforces</span>", while "<span class="tex-font-style-tt">decor</span>" and "<span class="tex-font-style-tt">fork</span>" are not.</p><p>A <span class="tex-font-style-it">palindrome</span> is a string that reads the same from left to right and from right to left. For example, "<span class="tex-font-style-tt">abacaba</span>" is a palindrome, but "<span class="tex-font-style-tt">abac</span>" is not.</p><p>Hossam defines a <span class="tex-font-style-it">sub-palindrome</span> of a string $s$ as a subsequence of $s$, that is a palindrome. For example, "<span class="tex-font-style-tt">k</span>", "<span class="tex-font-style-tt">abba</span>" and "<span class="tex-font-style-tt">abhba</span>" are sub-palindromes of the string "<span class="tex-font-style-tt">abhbka</span>", but "<span class="tex-font-style-tt">abka</span>" and "<span class="tex-font-style-tt">cat</span>" are not.</p><p>Hossam defines a <span class="tex-font-style-it">maximal sub-palindrome</span> of a string $s$ as a sub-palindrome of $s$, which has the maximal length among all sub-palindromes of $s$. For example, "<span class="tex-font-style-tt">abhbka</span>" has only one maximal sub-palindrome — "<span class="tex-font-style-tt">abhba</span>". But it may also be that the string has several maximum sub-palindromes: the string "<span class="tex-font-style-tt">abcd</span>" has $4$ maximum sub-palindromes.</p><p>Help Hossam find the length of the longest maximal sub-palindrome among all $s(v, \, u)$ in the tree $G$.</p><p><span class="tex-font-style-bf">Note that the sub-palindrome is a subsequence, not a substring.</span></p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 200$) — the number of test cases.</p><p>The first line of each test case has one integer number $n$ ($1 \le n \le 2 \cdot 10^3$) — the number of vertices in the graph.</p><p>The second line contains a string $s$ of length $n$, the $i$-th symbol of which denotes the letter on the vertex $i$. It is guaranteed that all characters in this string are lowercase English letters.</p><p>The next $n - 1$ lines describe the edges of the tree. Each edge is given by two integers $v$ and $u$ ($1 \le v, \, u \le n$, $v \neq u$). These two numbers mean that there is an edge $(v, \, u)$ in the tree. It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that sum of all $n$ doesn't exceed $2 \cdot 10^3$.</p></div><div class="output-specification"><p>For each test case output one integer — the length of the longest maximal sub-palindrome among all $s(v, \, u)$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 200$) — the number of test cases.</p><p>The first line of each test case has one integer number $n$ ($1 \le n \le 2 \cdot 10^3$) — the number of vertices in the graph.</p><p>The second line contains a string $s$ of length $n$, the $i$-th symbol of which denotes the letter on the vertex $i$. It is guaranteed that all characters in this string are lowercase English letters.</p><p>The next $n - 1$ lines describe the edges of the tree. Each edge is given by two integers $v$ and $u$ ($1 \le v, \, u \le n$, $v \neq u$). These two numbers mean that there is an edge $(v, \, u)$ in the tree. It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that sum of all $n$ doesn't exceed $2 \cdot 10^3$.</p>

## Output

<p>For each test case output one integer — the length of the longest maximal sub-palindrome among all $s(v, \, u)$.</p>





```input1|2,3,4,5,6,7
2
5
abaca
1 2
1 3
3 4
4 5
9
caabadedb
1 2
2 3
2 4
1 5
5 6
5 7
5 8
8 9
```




```output1
3
5
```



## Note

<p>In the first example the maximal subpalindromes are "<span class="tex-font-style-tt">aaa</span>" with letters in vertices $1, \, 3, \, 5$, or "<span class="tex-font-style-tt">aca</span>" with letters in vertices $1, \, 4, \, 5$.</p><center> <img class="tex-graphics" src="file://7zvMlF1k.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The tree from the first example.</span> </center><p>In the second example there is only one maximal palindrome "<span class="tex-font-style-tt">bacab</span>" with letters in vertices $4, \, 2, \, 1, \, 5, \, 9$.</p><center> <img class="tex-graphics" src="file://5noctGB4.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The tree from the second example.</span> </center>
