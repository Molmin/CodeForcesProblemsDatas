## Description

<div><div class="epigraph"><div class="epigraph-text">Real stupidity beats artificial intelligence every time.</div><div class="epigraph-source">— Terry Pratchett, <span class="tex-font-style-it">Hogfather, Discworld</span></div></div><p>You are given a string $s$ of length $n$ and a number $k$. Let's denote by $rev(s)$ the reversed string $s$ (i.e. $rev(s) = s_n s_{n-1} ... s_1$). You can apply one of the two kinds of operations to the string:</p><ul><li> replace the string $s$ with $s + rev(s)$</li><li> replace the string $s$ with $rev(s) + s$</li></ul><p>How many different strings can you get as a result of performing <span class="tex-font-style-bf">exactly</span> $k$ operations (possibly of different kinds) on the original string $s$?</p><p>In this statement we denoted the concatenation of strings $s$ and $t$ as $s + t$. In other words, $s + t = s_1 s_2 ... s_n t_1 t_2 ... t_m$, where $n$ and $m$ are the lengths of strings $s$ and $t$ respectively.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$)&nbsp;— number of test cases. Next $2 \cdot t$ lines contain $t$ test cases:</p><p>The first line of a test case contains two integers $n$ and $k$ ($1 \le n \le 100$, $0 \le k \le 1000$)&nbsp;— the length of the string and the number of operations respectively.</p><p>The second string of a test case contains one string $s$ of length $n$ consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>For each test case, print the answer (that is, the number of different strings that you can get after exactly $k$ operations) on a separate line.</p><p>It can be shown that the answer does not exceed $10^9$ under the given constraints.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$)&nbsp;— number of test cases. Next $2 \cdot t$ lines contain $t$ test cases:</p><p>The first line of a test case contains two integers $n$ and $k$ ($1 \le n \le 100$, $0 \le k \le 1000$)&nbsp;— the length of the string and the number of operations respectively.</p><p>The second string of a test case contains one string $s$ of length $n$ consisting of lowercase Latin letters.</p>

## Output

<p>For each test case, print the answer (that is, the number of different strings that you can get after exactly $k$ operations) on a separate line.</p><p>It can be shown that the answer does not exceed $10^9$ under the given constraints.</p>





```input1
4
3 2
aab
3 3
aab
7 1
abacaba
2 0
ab
```




```output1
2
2
1
1
```



## Note

<p>In the first test case of the example:</p><p>After the first operation the string $s$ can become either <span class="tex-font-style-bf">aabbaa</span> or <span class="tex-font-style-bf">baaaab</span>. After the second operation there are 2 possibilities for $s$: <span class="tex-font-style-bf">aabbaaaabbaa</span> and <span class="tex-font-style-bf">baaaabbaaaab</span>.</p>
