## Description

<div><p><span class="tex-font-style-bf">Note that the memory limit is unusual.</span></p><p>Let's define the sequence of Fibonacci strings as follows: $f_0$ is <span class="tex-font-style-tt">0</span>, $f_1$ is <span class="tex-font-style-tt">1</span>, $f_i$ is $f_{i-1} + f_{i-2}$ for $i&gt;1$ ($+$ denotes the concatenation of two strings). So, for example, $f_2$ is <span class="tex-font-style-tt">10</span>, $f_3$ is <span class="tex-font-style-tt">101</span>, $f_4$ is <span class="tex-font-style-tt">10110</span>.</p><p>For a given string $s$, let's define $g(s)$ as the number of ways to cut it into several (any number, possibly even just one) strings such that none of these strings are Fibonacci strings. For example, if $s$ is <span class="tex-font-style-tt">10110101</span>, $g(s) = 3$ since there are three ways to cut it:</p><ul> <li> <span class="tex-font-style-tt">101101</span> $+$ <span class="tex-font-style-tt">01</span>; </li><li> <span class="tex-font-style-tt">1011</span> $+$ <span class="tex-font-style-tt">0101</span>; </li><li> <span class="tex-font-style-tt">1011</span> $+$ <span class="tex-font-style-tt">01</span> $+$ <span class="tex-font-style-tt">01</span>. </li></ul><p>You are given a sequence of strings $s_1, s_2, \dots, s_n$. Calculate $g(s_1), g(s_1 + s_2), \dots, g(s_1 + s_2 + \ldots + s_n)$. Since these values can be huge, print them modulo $998244353$.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 3 \cdot 10^3$).</p><p>Then, $n$ lines follow. The $i$-th line contains the string $s_i$ ($1 \le |s_i| \le 10^3$), consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>Print $n$ integers, where the $i$-th integer is $g(s_1 + s_2 + \ldots + s_i) \bmod 998244353$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 3 \cdot 10^3$).</p><p>Then, $n$ lines follow. The $i$-th line contains the string $s_i$ ($1 \le |s_i| \le 10^3$), consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>Print $n$ integers, where the $i$-th integer is $g(s_1 + s_2 + \ldots + s_i) \bmod 998244353$.</p>





```input1
1
10110101
```




```input2
3
1111
1
0
```




```input3
6
10110101
100100001110
0000001100010001
1111
1001010100101010101001
000100000010101111
```




```output1
3
```




```output2
2
3
3
```




```output3
3
561
1466229
9887505
972227653
52128355
```


