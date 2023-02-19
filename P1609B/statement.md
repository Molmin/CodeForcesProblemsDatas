## Description

<div><center> <img class="tex-graphics" height="302px" src="file://ePkiegjX.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>Before becoming a successful trader William got a university degree. During his education an interesting situation happened, after which William started to listen to homework assignments much more attentively. What follows is the correct formal description of the homework assignment:</p><p>You are given a string $s$ of length $n$ only consisting of characters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>". There are $q$ queries of format ($pos, c$), meaning replacing the element of string $s$ at position $pos$ with character $c$. After each query you must output the minimal number of characters in the string, which have to be replaced, so that the string doesn't contain string "<span class="tex-font-style-tt">abc</span>" as a <span class="tex-font-style-bf">substring</span>. A valid replacement of a character is replacing it with "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" or "<span class="tex-font-style-tt">c</span>".</p><p>A string $x$ is a substring of a string $y$ if $x$ can be obtained from $y$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ $(1 \le n, q \le 10^5)$, the length of the string and the number of queries, respectively.</p><p>The second line contains the string $s$, consisting of characters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>".</p><p>Each of the next $q$ lines contains an integer $i$ and character $c$ $(1 \le i \le n)$, index and the value of the new item in the string, respectively. It is guaranteed that character's $c$ value is "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" or "<span class="tex-font-style-tt">c</span>".</p></div><div class="output-specification"><p>For each query output the minimal number of characters that would have to be replaced so that the string doesn't contain "<span class="tex-font-style-tt">abc</span>" as a substring.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ $(1 \le n, q \le 10^5)$, the length of the string and the number of queries, respectively.</p><p>The second line contains the string $s$, consisting of characters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>".</p><p>Each of the next $q$ lines contains an integer $i$ and character $c$ $(1 \le i \le n)$, index and the value of the new item in the string, respectively. It is guaranteed that character's $c$ value is "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" or "<span class="tex-font-style-tt">c</span>".</p>

## Output

<p>For each query output the minimal number of characters that would have to be replaced so that the string doesn't contain "<span class="tex-font-style-tt">abc</span>" as a substring.</p>





```input1
9 10
abcabcabc
1 a
1 b
2 c
3 a
4 b
5 c
8 a
9 b
1 c
4 a
```




```output1
3
2
2
2
1
2
1
1
1
0
```



## Note

<p>Let's consider the state of the string after each query: </p><ol> <li> $s =$ "<span class="tex-font-style-tt">abcabcabc</span>". In this case $3$ replacements can be performed to get, for instance, string $s =$ "<span class="tex-font-style-tt">bbcaccabb</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a substring.</li><li> $s =$ "<span class="tex-font-style-tt">bbcabcabc</span>". In this case $2$ replacements can be performed to get, for instance, string $s =$ "<span class="tex-font-style-tt">bbcbbcbbc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a substring.</li><li> $s =$ "<span class="tex-font-style-tt">bccabcabc</span>". In this case $2$ replacements can be performed to get, for instance, string $s =$ "<span class="tex-font-style-tt">bccbbcbbc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a substring.</li><li> $s =$ "<span class="tex-font-style-tt">bcaabcabc</span>". In this case $2$ replacements can be performed to get, for instance, string $s =$ "<span class="tex-font-style-tt">bcabbcbbc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a substring.</li><li> $s =$ "<span class="tex-font-style-tt">bcabbcabc</span>". In this case $1$ replacements can be performed to get, for instance, string $s =$ "<span class="tex-font-style-tt">bcabbcabb</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a substring.</li><li> $s =$ "<span class="tex-font-style-tt">bcabccabc</span>". In this case $2$ replacements can be performed to get, for instance, string $s =$ "<span class="tex-font-style-tt">bcabbcabb</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a substring.</li><li> $s =$ "<span class="tex-font-style-tt">bcabccaac</span>". In this case $1$ replacements can be performed to get, for instance, string $s =$ "<span class="tex-font-style-tt">bcabbcaac</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a substring.</li><li> $s =$ "<span class="tex-font-style-tt">bcabccaab</span>". In this case $1$ replacements can be performed to get, for instance, string $s =$ "<span class="tex-font-style-tt">bcabbcaab</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a substring.</li><li> $s =$ "<span class="tex-font-style-tt">ccabccaab</span>". In this case $1$ replacements can be performed to get, for instance, string $s =$ "<span class="tex-font-style-tt">ccabbcaab</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a substring.</li><li> $s =$ "<span class="tex-font-style-tt">ccaaccaab</span>". In this case the string does not contain "<span class="tex-font-style-tt">abc</span>" as a substring and no replacements are needed.</li></ol>
