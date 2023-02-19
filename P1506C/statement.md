## Description

<div><p>You are given the strings $a$ and $b$, consisting of lowercase Latin letters. You can do any number of the following operations in any order: </p><ul> <li> if $|a| &gt; 0$ (the length of the string $a$ is greater than zero), delete the first character of the string $a$, that is, replace $a$ with $a_2 a_3 \ldots a_n$; </li><li> if $|a| &gt; 0$, delete the last character of the string $a$, that is, replace $a$ with $a_1 a_2 \ldots a_{n-1}$; </li><li> if $|b| &gt; 0$ (the length of the string $b$ is greater than zero), delete the first character of the string $b$, that is, replace $b$ with $b_2 b_3 \ldots b_n$; </li><li> if $|b| &gt; 0$, delete the last character of the string $b$, that is, replace $b$ with $b_1 b_2 \ldots b_{n-1}$. </li></ul><p>Note that after each of the operations, the string $a$ or $b$ may become empty.</p><p>For example, if $a=$<span class="tex-font-style-tt">"hello"</span> and $b=$<span class="tex-font-style-tt">"icpc"</span>, then you can apply the following sequence of operations: </p><ul> <li> delete the first character of the string $a$ $\Rightarrow$ $a=$<span class="tex-font-style-tt">"ello"</span> and $b=$<span class="tex-font-style-tt">"icpc"</span>; </li><li> delete the first character of the string $b$ $\Rightarrow$ $a=$<span class="tex-font-style-tt">"ello"</span> and $b=$<span class="tex-font-style-tt">"cpc"</span>; </li><li> delete the first character of the string $b$ $\Rightarrow$ $a=$<span class="tex-font-style-tt">"ello"</span> and $b=$<span class="tex-font-style-tt">"pc"</span>; </li><li> delete the last character of the string $a$ $\Rightarrow$ $a=$<span class="tex-font-style-tt">"ell"</span> and $b=$<span class="tex-font-style-tt">"pc"</span>; </li><li> delete the last character of the string $b$ $\Rightarrow$ $a=$<span class="tex-font-style-tt">"ell"</span> and $b=$<span class="tex-font-style-tt">"p"</span>. </li></ul><p>For the given strings $a$ and $b$, find the minimum number of operations for which you can make the strings $a$ and $b$ equal. Note that empty strings are also equal.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$). Then $t$ test cases follow.</p><p>The first line of each test case contains the string $a$ ($1 \le |a| \le 20$), consisting of lowercase Latin letters.</p><p>The second line of each test case contains the string $b$ ($1 \le |b| \le 20$), consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>For each test case, output the minimum number of operations that can make the strings $a$ and $b$ equal.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$). Then $t$ test cases follow.</p><p>The first line of each test case contains the string $a$ ($1 \le |a| \le 20$), consisting of lowercase Latin letters.</p><p>The second line of each test case contains the string $b$ ($1 \le |b| \le 20$), consisting of lowercase Latin letters.</p>

## Output

<p>For each test case, output the minimum number of operations that can make the strings $a$ and $b$ equal.</p>





```input1
5
a
a
abcd
bc
hello
codeforces
hello
helo
dhjakjsnasjhfksafasd
adjsnasjhfksvdafdser
```




```output1
0
2
13
3
20
```


