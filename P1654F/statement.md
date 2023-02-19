## Description

<div><p>You are given an integer $n$ and a string $s$ consisting of $2^n$ lowercase letters of the English alphabet. The characters of the string $s$ are $s_0s_1s_2\cdots s_{2^n-1}$.</p><p>A string $t$ of length $2^n$ (whose characters are denoted by $t_0t_1t_2\cdots t_{2^n-1}$) is a <span class="tex-font-style-it">xoration</span> of $s$ if there exists an integer $j$ ($0\le j \leq 2^n-1$) such that, for each $0 \leq i \leq 2^n-1$, $t_i = s_{i \oplus j}$ (where $\oplus$ denotes the operation <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a>).</p><p>Find the lexicographically minimal <span class="tex-font-style-it">xoration</span> of $s$.</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds: </p><ul> <li> $a$ is a prefix of $b$, but $a \ne b$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul> </div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 18$).</p><p>The second line contains a string $s$ consisting of $2^n$ lowercase letters of the English alphabet.</p></div><div class="output-specification"><p>Print a single line containing the lexicographically minimal xoration of $s$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 18$).</p><p>The second line contains a string $s$ consisting of $2^n$ lowercase letters of the English alphabet.</p>

## Output

<p>Print a single line containing the lexicographically minimal xoration of $s$.</p>





```input1
2
acba
```




```input2
3
bcbaaabb
```




```input3
4
bdbcbccdbdbaaccd
```




```input4
5
ccfcffccccccffcfcfccfffffcccccff
```




```input5
1
zz
```




```output1
abca
```




```output2
aabbbcba
```




```output3
abdbdccacbdbdccb
```




```output4
cccccffffcccccffccfcffcccccfffff
```




```output5
zz
```



## Note

<p>In the first test, the lexicographically minimal xoration $t$ of $s =$"<span class="tex-font-style-tt">acba</span>" is "<span class="tex-font-style-tt">abca</span>". It's a xoration because, for $j = 3$, </p><ul> <li> $t_0 = s_{0 \oplus j} = s_3 =$ "<span class="tex-font-style-tt">a</span>"; </li><li> $t_1 = s_{1 \oplus j} = s_2 =$ "<span class="tex-font-style-tt">b</span>"; </li><li> $t_2 = s_{2 \oplus j} = s_1 =$ "<span class="tex-font-style-tt">c</span>"; </li><li> $t_3 = s_{3 \oplus j} = s_0 =$ "<span class="tex-font-style-tt">a</span>". </li></ul> There isn't any xoration of $s$ lexicographically smaller than "<span class="tex-font-style-tt">abca</span>".<p>In the second test, the minimal string xoration corresponds to choosing $j = 4$ in the definition of xoration.</p><p>In the third test, the minimal string xoration corresponds to choosing $j = 11$ in the definition of xoration.</p><p>In the fourth test, the minimal string xoration corresponds to choosing $j = 10$ in the definition of xoration.</p><p>In the fifth test, the minimal string xoration corresponds to choosing either $j = 0$ or $j = 1$ in the definition of xoration.</p>
