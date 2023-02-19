## Description

<div><p><span class="tex-font-style-it">Kuznecov likes art, poetry, and music. And strings consisting of lowercase English letters.</span></p><p>Recently, Kuznecov has found two strings, $a$ and $b$, of lengths $n$ and $m$ respectively. They consist of lowercase English letters and <span class="tex-font-style-bf">no character is contained in both strings</span>. </p><p>Let another string $c$ be initially empty. Kuznecov can do the following two types of operations:</p><ul> <li> Choose any character from the string $a$, remove it from $a$, and add it to the end of $c$. </li><li> Choose any character from the string $b$, remove it from $b$, and add it to the end of $c$. </li></ul><p>But, he can not do more than $k$ operations of the same type in a row. He must perform operations until either $a$ or $b$ becomes empty. What is the lexicographically smallest possible value of $c$ after he finishes?</p><p>A string $x$ is lexicographically smaller than a string $y$ if and only if one of the following holds:</p><ul><li> $x$ is a prefix of $y$, but $x \neq y$; </li><li> in the first position where $x$ and $y$ differ, the string $x$ has a letter that appears earlier in the alphabet than the corresponding letter in $y$.</li></ul></div><div class="input-specification"><p>There are several test cases in the input data. The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($1\leq n,m,k \leq 100$)&nbsp;— parameters from the statement.</p><p>The second line of each test case contains the string $a$ of length $n$.</p><p>The third line of each test case contains the string $b$ of length $m$. </p><p>The strings contain only lowercase English letters. It is guaranteed that no symbol appears in $a$ and $b$ simultaneously.</p></div><div class="output-specification"><p>In each test case, output a single string $c$&nbsp;— the answer to the problem.</p></div>

## Input

<p>There are several test cases in the input data. The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($1\leq n,m,k \leq 100$)&nbsp;— parameters from the statement.</p><p>The second line of each test case contains the string $a$ of length $n$.</p><p>The third line of each test case contains the string $b$ of length $m$. </p><p>The strings contain only lowercase English letters. It is guaranteed that no symbol appears in $a$ and $b$ simultaneously.</p>

## Output

<p>In each test case, output a single string $c$&nbsp;— the answer to the problem.</p>





```input1
3
6 4 2
aaaaaa
bbbb
5 9 3
caaca
bedededeb
7 7 1
noskill
wxhtzdy
```




```output1
aabaabaa
aaabbcc
dihktlwlxnyoz
```



## Note

<p>In the first test case, it is optimal to take two '<span class="tex-font-style-tt">a</span>'s from the string $a$ and add them to the string $c$. Then it is forbidden to take more characters from $a$, hence one character '<span class="tex-font-style-tt">b</span>' from the string $b$ has to be taken. Following that logic, we end up with $c$ being '<span class="tex-font-style-tt">aabaabaa</span>' when string $a$ is emptied.</p><p>In the second test case it is optimal to take as many '<span class="tex-font-style-tt">a</span>'s from string $a$ as possible, then take as many '<span class="tex-font-style-tt">b</span>'s as possible from string $b$. In the end, we take two '<span class="tex-font-style-tt">c</span>'s from the string $a$ emptying it. </p>
