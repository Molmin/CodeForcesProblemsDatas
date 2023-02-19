## Description

<div><p>You are given a binary string (i. e. a string consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>) $s$ of length $n$. You can perform the following operation with the string $s$ <span class="tex-font-style-bf">at most once</span>: choose a substring (a contiguous subsequence) of $s$ having <span class="tex-font-style-bf">exactly</span> $k$ characters <span class="tex-font-style-tt">1</span> in it, and shuffle it (reorder the characters in the substring as you wish).</p><p>Calculate the number of different strings which can be obtained from $s$ by performing this operation at most once.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \le n \le 5000$; $0 \le k \le n$).</p><p>The second line contains the string $s$ of length $n$, consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>Print one integer — the number of different strings which can be obtained from $s$ by performing the described operation at most once. Since the answer can be large, output it modulo $998244353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \le n \le 5000$; $0 \le k \le n$).</p><p>The second line contains the string $s$ of length $n$, consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>Print one integer — the number of different strings which can be obtained from $s$ by performing the described operation at most once. Since the answer can be large, output it modulo $998244353$.</p>





```input1
7 2
1100110
```




```input2
5 0
10010
```




```input3
8 1
10001000
```




```input4
10 8
0010011000
```




```output1
16
```




```output2
1
```




```output3
10
```




```output4
1
```



## Note

<p>Some strings you can obtain in the first example:</p><ul> <li> to obtain <span class="tex-font-style-tt">0110110</span>, you can take the substring from the $1$-st character to the $4$-th character, which is <span class="tex-font-style-tt">1100</span>, and reorder its characters to get <span class="tex-font-style-tt">0110</span>; </li><li> to obtain <span class="tex-font-style-tt">1111000</span>, you can take the substring from the $3$-rd character to the $7$-th character, which is <span class="tex-font-style-tt">00110</span>, and reorder its characters to get <span class="tex-font-style-tt">11000</span>; </li><li> to obtain <span class="tex-font-style-tt">1100101</span>, you can take the substring from the $5$-th character to the $7$-th character, which is <span class="tex-font-style-tt">110</span>, and reorder its characters to get <span class="tex-font-style-tt">101</span>. </li></ul><p>In the second example, $k = 0$ so you can only choose the substrings consisting only of <span class="tex-font-style-tt">0</span> characters. Reordering them doesn't change the string at all, so the only string you can obtain is <span class="tex-font-style-tt">10010</span>.</p>
