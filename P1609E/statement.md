## Description

<div><center> <img class="tex-graphics" height="302px" src="file://tEfHXRCg.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>Before becoming a successful trader William got a university degree. During his education an interesting situation happened, after which William started to listen to homework assignments much more attentively. What follows is a formal description of the homework assignment as William heard it:</p><p>You are given a string $s$ of length $n$ only consisting of characters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>". There are $q$ queries of format ($pos, c$), meaning replacing the element of string $s$ at position $pos$ with character $c$. After each query you must output the minimal number of characters in the string, which have to be replaced, so that the string doesn't contain string "<span class="tex-font-style-tt">abc</span>" as a <span class="tex-font-style-bf">subsequence</span>. A valid replacement of a character is replacing it with "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" or "<span class="tex-font-style-tt">c</span>".</p><p>A string $x$ is said to be a subsequence of string $y$ if $x$ can be obtained from $y$ by deleting some characters without changing the ordering of the remaining characters.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ $(1 \le n, q \le 10^5)$, the length of the string and the number of queries, respectively.</p><p>The second line contains the string $s$, consisting of characters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>".</p><p>Each of the next $q$ lines contains an integer $i$ and character $c$ $(1 \le i \le n)$, index and the value of the new item in the string, respectively. It is guaranteed that character's $c$ value is "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" or "<span class="tex-font-style-tt">c</span>".</p></div><div class="output-specification"><p>For each query output the minimal number of characters that would have to be replaced so that the string doesn't contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ $(1 \le n, q \le 10^5)$, the length of the string and the number of queries, respectively.</p><p>The second line contains the string $s$, consisting of characters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>".</p><p>Each of the next $q$ lines contains an integer $i$ and character $c$ $(1 \le i \le n)$, index and the value of the new item in the string, respectively. It is guaranteed that character's $c$ value is "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>" or "<span class="tex-font-style-tt">c</span>".</p>

## Output

<p>For each query output the minimal number of characters that would have to be replaced so that the string doesn't contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</p>





```input1
9 12
aaabccccc
4 a
4 b
2 b
5 a
1 b
6 b
5 c
2 a
1 a
5 a
6 b
7 b
```




```output1
0
1
2
2
1
2
1
2
2
2
2
2
```



## Note

<p>Let's consider the state of the string after each query: </p><ol> <li> $s = $"<span class="tex-font-style-tt">aaaaccccc</span>". In this case the string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence and no replacements are needed.</li><li> $s = $"<span class="tex-font-style-tt">aaabccccc</span>". In this case 1 replacements can be performed to get, for instance, string $s = $"<span class="tex-font-style-tt">aaaaccccc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li><li> $s = $"<span class="tex-font-style-tt">ababccccc</span>". In this case 2 replacements can be performed to get, for instance, string $s = $<span class="tex-font-style-tt">aaaaccccc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li><li> $s = $"<span class="tex-font-style-tt">ababacccc</span>". In this case 2 replacements can be performed to get, for instance, string $s = $"<span class="tex-font-style-tt">aaaaacccc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li><li> $s = $"<span class="tex-font-style-tt">bbabacccc</span>". In this case 1 replacements can be performed to get, for instance, string $s = $"<span class="tex-font-style-tt">bbacacccc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li><li> $s = $"<span class="tex-font-style-tt">bbababccc</span>". In this case 2 replacements can be performed to get, for instance, string $s = $"<span class="tex-font-style-tt">bbacacccc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li><li> $s = $"<span class="tex-font-style-tt">bbabcbccc</span>". In this case 1 replacements can be performed to get, for instance, string $s = $"<span class="tex-font-style-tt">bbcbcbccc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li><li> $s = $"<span class="tex-font-style-tt">baabcbccc</span>". In this case 2 replacements can be performed to get, for instance, string $s = $"<span class="tex-font-style-tt">bbbbcbccc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li><li> $s = $"<span class="tex-font-style-tt">aaabcbccc</span>". In this case 2 replacements can be performed to get, for instance, string $s = $"<span class="tex-font-style-tt">aaacccccc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li><li> $s = $"<span class="tex-font-style-tt">aaababccc</span>". In this case 2 replacements can be performed to get, for instance, string $s = $"<span class="tex-font-style-tt">aaacacccc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li><li> $s = $"<span class="tex-font-style-tt">aaababccc</span>". In this case 2 replacements can be performed to get, for instance, string $s = $"<span class="tex-font-style-tt">aaacacccc</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li><li> $s = $"<span class="tex-font-style-tt">aaababbcc</span>". In this case 2 replacements can be performed to get, for instance, string $s = $"<span class="tex-font-style-tt">aaababbbb</span>". This string does not contain "<span class="tex-font-style-tt">abc</span>" as a subsequence.</li></ol>
