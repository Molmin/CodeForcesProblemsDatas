## Description

<div><p>Acacius is studying strings theory. Today he came with the following problem.</p><p>You are given a string $s$ of length $n$ consisting of lowercase English letters and question marks. It is possible to replace question marks with lowercase English letters in such a way that a string "<span class="tex-font-style-tt">abacaba</span>" occurs as a substring in a resulting string exactly once?</p><p>Each question mark should be replaced with <span class="tex-font-style-bf">exactly one</span> lowercase English letter. For example, string "<span class="tex-font-style-tt">a?b?c</span>" can be transformed into strings "<span class="tex-font-style-tt">aabbc</span>" and "<span class="tex-font-style-tt">azbzc</span>", but can't be transformed into strings "<span class="tex-font-style-tt">aabc</span>", "<span class="tex-font-style-tt">a?bbc</span>" and "<span class="tex-font-style-tt">babbc</span>".</p><p>Occurrence of a string $t$ of length $m$ in the string $s$ of length $n$ as a substring is a index $i$ ($1 \leq i \leq n - m + 1$) such that string $s[i..i+m-1]$ consisting of $m$ consecutive symbols of $s$ starting from $i$-th equals to string $t$. For example string "<span class="tex-font-style-tt">ababa</span>" has two occurrences of a string "<span class="tex-font-style-tt">aba</span>" as a substring with $i = 1$ and $i = 3$, but there are no occurrences of a string "<span class="tex-font-style-tt">aba</span>" in the string "<span class="tex-font-style-tt">acba</span>" as a substring.</p><p>Please help Acacius to check if it is possible to replace all question marks with lowercase English letters in such a way that a string "<span class="tex-font-style-tt">abacaba</span>" occurs as a substring in a resulting string <span class="tex-font-style-bf">exactly once</span>.</p></div><div class="input-specification"><p>First line of input contains an integer $T$ ($1 \leq T \leq 5000$), number of test cases. $T$ pairs of lines with test case descriptions follow.</p><p>The first line of a test case description contains a single integer $n$ ($7 \leq n \leq 50$), length of a string $s$.</p><p>The second line of a test case description contains string $s$ of length $n$ consisting of lowercase English letters and question marks.</p></div><div class="output-specification"><p>For each test case output an answer for it.</p><p>In case if there is no way to replace question marks in string $s$ with a lowercase English letters in such a way that there is exactly one occurrence of a string "<span class="tex-font-style-tt">abacaba</span>" in the resulting string as a substring output "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise output "<span class="tex-font-style-tt">Yes</span>" and in the next line output a resulting string consisting of $n$ lowercase English letters. If there are multiple possible strings, output any.</p><p>You may print every letter in "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span>, and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p></div>

## Input

<p>First line of input contains an integer $T$ ($1 \leq T \leq 5000$), number of test cases. $T$ pairs of lines with test case descriptions follow.</p><p>The first line of a test case description contains a single integer $n$ ($7 \leq n \leq 50$), length of a string $s$.</p><p>The second line of a test case description contains string $s$ of length $n$ consisting of lowercase English letters and question marks.</p>

## Output

<p>For each test case output an answer for it.</p><p>In case if there is no way to replace question marks in string $s$ with a lowercase English letters in such a way that there is exactly one occurrence of a string "<span class="tex-font-style-tt">abacaba</span>" in the resulting string as a substring output "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise output "<span class="tex-font-style-tt">Yes</span>" and in the next line output a resulting string consisting of $n$ lowercase English letters. If there are multiple possible strings, output any.</p><p>You may print every letter in "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span>, and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p>





```input1
6
7
abacaba
7
???????
11
aba?abacaba
11
abacaba?aba
15
asdf???f???qwer
11
abacabacaba
```




```output1
Yes
abacaba
Yes
abacaba
Yes
abadabacaba
Yes
abacabadaba
No
No
```



## Note

<p>In first example there is exactly one occurrence of a string "<span class="tex-font-style-tt">abacaba</span>" in the string "<span class="tex-font-style-tt">abacaba</span>" as a substring.</p><p>In second example seven question marks can be replaced with any seven lowercase English letters and with "<span class="tex-font-style-tt">abacaba</span>" in particular.</p><p>In sixth example there are two occurrences of a string "<span class="tex-font-style-tt">abacaba</span>" as a substring.</p>
