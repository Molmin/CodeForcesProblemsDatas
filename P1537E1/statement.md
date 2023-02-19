## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The only difference is the constraints on $n$ and $k$. You can make hacks only if all versions of the problem are solved.</span></p><p>You have a string $s$, and you can do two types of operations on it: </p><ul> <li> Delete the last character of the string. </li><li> Duplicate the string: $s:=s+s$, where $+$ denotes concatenation. </li></ul><p>You can use each operation any number of times (possibly none).</p><p>Your task is to find the lexicographically smallest string of length exactly $k$ that can be obtained by doing these operations on string $s$.</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds:</p><ul> <li> $a$ is a prefix of $b$, but $a\ne b$; </li><li> In the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$, $k$ ($1 \leq n, k \leq 5000$) — the length of the original string $s$ and the length of the desired string.</p><p>The second line contains the string $s$, consisting of $n$ lowercase English letters.</p></div><div class="output-specification"><p>Print the lexicographically smallest string of length $k$ that can be obtained by doing the operations on string $s$.</p></div>

## Input

<p>The first line contains two integers $n$, $k$ ($1 \leq n, k \leq 5000$) — the length of the original string $s$ and the length of the desired string.</p><p>The second line contains the string $s$, consisting of $n$ lowercase English letters.</p>

## Output

<p>Print the lexicographically smallest string of length $k$ that can be obtained by doing the operations on string $s$.</p>





```input1
8 16
dbcadabc
```




```input2
4 5
abcd
```




```output1
dbcadabcdbcadabc
```




```output2
aaaaa
```



## Note

<p>In the first test, it is optimal to make one duplication: "<span class="tex-font-style-tt">dbcadabc</span>" $\to$ "<span class="tex-font-style-tt">dbcadabcdbcadabc</span>".</p><p>In the second test it is optimal to delete the last $3$ characters, then duplicate the string $3$ times, then delete the last $3$ characters to make the string have length $k$.</p><p>"<span class="tex-font-style-tt">abcd</span>" $\to$ "<span class="tex-font-style-tt">abc</span>" $\to$ "<span class="tex-font-style-tt">ab</span>" $\to$ "<span class="tex-font-style-tt">a</span>" $\to$ "<span class="tex-font-style-tt">aa</span>" $\to$ "<span class="tex-font-style-tt">aaaa</span>" $\to$ "<span class="tex-font-style-tt">aaaaaaaa</span>" $\to$ "<span class="tex-font-style-tt">aaaaaaa</span>" $\to$ "<span class="tex-font-style-tt">aaaaaa</span>" $\to$ "<span class="tex-font-style-tt">aaaaa</span>".</p>
