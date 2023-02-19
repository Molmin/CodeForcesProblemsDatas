## Description

<div><p>You are given a string $s$, consisting of lowercase Latin letters. While there is at least one character in the string $s$ that is <span class="tex-font-style-bf">repeated at least twice</span>, you perform the following operation: </p><ul> <li> you choose the index $i$ ($1 \le i \le |s|$) such that the character at position $i$ occurs <span class="tex-font-style-bf">at least two</span> times in the string $s$, and delete the character at position $i$, that is, replace $s$ with $s_1 s_2 \ldots s_{i-1} s_{i+1} s_{i+2} \ldots s_n$. </li></ul><p>For example, if $s=$<span class="tex-font-style-tt">"codeforces"</span>, then you can apply the following sequence of operations: </p><ul> <li> $i=6 \Rightarrow s=$<span class="tex-font-style-tt">"codefrces"</span>; </li><li> $i=1 \Rightarrow s=$<span class="tex-font-style-tt">"odefrces"</span>; </li><li> $i=7 \Rightarrow s=$<span class="tex-font-style-tt">"odefrcs"</span>; </li></ul><p>Given a given string $s$, find the lexicographically maximum string that can be obtained after applying a certain sequence of operations after which all characters in the string <span class="tex-font-style-bf">become unique</span>.</p><p>A string $a$ of length $n$ is lexicographically less than a string $b$ of length $m$, if: </p><ul> <li> there is an index $i$ ($1 \le i \le \min(n, m)$) such that the first $i-1$ characters of the strings $a$ and $b$ are the same, and the $i$-th character of the string $a$ is less than $i$-th character of string $b$; </li><li> <span class="tex-font-style-bf">or</span> the first $\min(n, m)$ characters in the strings $a$ and $b$ are the same and $n &lt; m$. </li></ul><p>For example, the string $a=$<span class="tex-font-style-tt">"aezakmi"</span> is lexicographically less than the string $b=$<span class="tex-font-style-tt">"aezus"</span>.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>Each test case is characterized by a string $s$, consisting of lowercase Latin letters ($1 \le |s| \le 2 \cdot 10^5$).</p><p>It is guaranteed that the sum of the lengths of the strings in all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the lexicographically maximum string that can be obtained after applying a certain sequence of operations after which all characters in the string <span class="tex-font-style-bf">become unique</span>.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>Each test case is characterized by a string $s$, consisting of lowercase Latin letters ($1 \le |s| \le 2 \cdot 10^5$).</p><p>It is guaranteed that the sum of the lengths of the strings in all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the lexicographically maximum string that can be obtained after applying a certain sequence of operations after which all characters in the string <span class="tex-font-style-bf">become unique</span>.</p>





```input1
6
codeforces
aezakmi
abacaba
convexhull
swflldjgpaxs
myneeocktxpqjpz
```




```output1
odfrces
ezakmi
cba
convexhul
wfldjgpaxs
myneocktxqjpz
```


