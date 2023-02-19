## Description

<div><p>A regular bracket sequence is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">1</span>" and "<span class="tex-font-style-tt">+</span>" between the original characters of the sequence. For example:</p><ul> <li> bracket sequences "<span class="tex-font-style-tt">()()</span>" and "<span class="tex-font-style-tt">(())</span>" are regular (the resulting expressions are: "<span class="tex-font-style-tt">(1)+(1)</span>" and "<span class="tex-font-style-tt">((1+1)+1)</span>"); </li><li> bracket sequences "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" are not. </li></ul><p>You are given two strings $s$ and $a$, the string $s$ has length $n$, the string $a$ has length $n - 3$. The string $s$ is a bracket sequence (i. e. each element of this string is either an opening bracket character or a closing bracket character). The string $a$ is a binary string (i. e. each element of this string is either <span class="tex-font-style-tt">1</span> or <span class="tex-font-style-tt">0</span>).</p><p>The string $a$ imposes some constraints on the string $s$: for every $i$ such that $a_i$ is <span class="tex-font-style-tt">1</span>, the string $s_i s_{i+1} s_{i+2} s_{i+3}$ should be a regular bracket sequence. Characters of $a$ equal to <span class="tex-font-style-tt">0</span> don't impose any constraints.</p><p>Initially, the string $s$ may or may not meet these constraints. You can perform the following operation any number of times: replace some character of $s$ with its inverse (i. e. you can replace an opening bracket with a closing bracket, or vice versa).</p><p>Determine if it is possible to change some characters in $s$ so that it meets all of the constraints, and if it is possible, calculate the minimum number of characters to be changed.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of three lines. The first line contains one integer $n$ ($4 \le n \le 2 \cdot 10^5$). The second line contains the string $s$, consisting of exactly $n$ characters; each character of $s$ is either '<span class="tex-font-style-tt">(</span>' or '<span class="tex-font-style-tt">)</span>'. The third line contains the string $a$, consisting of exactly $n - 3$ characters; each character of $a$ is either '<span class="tex-font-style-tt">1</span>' or '<span class="tex-font-style-tt">0</span>'.</p><p>Additional constraint on the input: the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer: the minimum number of characters that need to be changed in $s$, or $-1$ if it is impossible.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of three lines. The first line contains one integer $n$ ($4 \le n \le 2 \cdot 10^5$). The second line contains the string $s$, consisting of exactly $n$ characters; each character of $s$ is either '<span class="tex-font-style-tt">(</span>' or '<span class="tex-font-style-tt">)</span>'. The third line contains the string $a$, consisting of exactly $n - 3$ characters; each character of $a$ is either '<span class="tex-font-style-tt">1</span>' or '<span class="tex-font-style-tt">0</span>'.</p><p>Additional constraint on the input: the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer: the minimum number of characters that need to be changed in $s$, or $-1$ if it is impossible.</p>





```input1
6
4
))((
1
4
))((
0
4
()()
0
6
))(()(
101
6
))(()(
001
5
(((((
11
```




```output1
2
0
0
4
1
-1
```


