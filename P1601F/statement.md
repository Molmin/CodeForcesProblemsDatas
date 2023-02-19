## Description

<div><p>Integers from $1$ to $n$ (inclusive) were sorted lexicographically (considering integers as strings). As a result, array $a_1, a_2, \dots, a_n$ was obtained.</p><p>Calculate value of $(\sum_{i = 1}^n ((i - a_i) \mod 998244353)) \mod 10^9 + 7$.</p><p>$x \mod y$ here means the remainder after division $x$ by $y$. This remainder is always non-negative and doesn't exceed $y - 1$. For example, $5 \mod 3 = 2$, $(-1) \mod 6 = 5$. </p></div><div class="input-specification"><p>The first line contains the single integer $n$ ($1 \leq n \leq 10^{12}$).</p></div><div class="output-specification"><p>Print one integer&nbsp;— the required sum.</p></div>

## Input

<p>The first line contains the single integer $n$ ($1 \leq n \leq 10^{12}$).</p>

## Output

<p>Print one integer&nbsp;— the required sum.</p>





```input1
3
```




```input2
12
```




```input3
21
```




```input4
1000000000000
```




```output1
0
```




```output2
994733045
```




```output3
978932159
```




```output4
289817887
```



## Note

<p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds:</p><ul> <li> $a$ is a prefix of $b$, but $a \ne b$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul><p>For example, $42$ is lexicographically smaller than $6$, because they differ in the first digit, and $4 &lt; 6$; $42 &lt; 420$, because $42$ is a prefix of $420$.</p><p>Let's denote $998244353$ as $M$.</p><p>In the first example, array $a$ is equal to $[1, 2, 3]$. </p><ul> <li> $(1 - 1) \mod M = 0 \mod M = 0$ </li><li> $(2 - 2) \mod M = 0 \mod M = 0$ </li><li> $(3 - 3) \mod M = 0 \mod M = 0$ </li></ul><p>As a result, $(0 + 0 + 0) \mod 10^9 + 7 = 0$</p><p>In the second example, array $a$ is equal to $[1, 10, 11, 12, 2, 3, 4, 5, 6, 7, 8, 9]$. </p><ul> <li> $(1 - 1) \mod M = 0 \mod M = 0$ </li><li> $(2 - 10) \mod M = (-8) \mod M = 998244345$ </li><li> $(3 - 11) \mod M = (-8) \mod M = 998244345$ </li><li> $(4 - 12) \mod M = (-8) \mod M = 998244345$ </li><li> $(5 - 2) \mod M = 3 \mod M = 3$ </li><li> $(6 - 3) \mod M = 3 \mod M = 3$ </li><li> $(7 - 4) \mod M = 3 \mod M = 3$ </li><li> $(8 - 5) \mod M = 3 \mod M = 3$ </li><li> $(9 - 6) \mod M = 3 \mod M = 3$ </li><li> $(10 - 7) \mod M = 3 \mod M = 3$ </li><li> $(11 - 8) \mod M = 3 \mod M = 3$ </li><li> $(12 - 9) \mod M = 3 \mod M = 3$ </li></ul><p>As a result, $(0 + 998244345 + 998244345 + 998244345 + 3 + 3 + 3 + 3 + 3 + 3 + 3 + 3) \mod 10^9 + 7$ $=$ $2994733059 \mod 10^9 + 7$ $=$ $994733045$</p>
