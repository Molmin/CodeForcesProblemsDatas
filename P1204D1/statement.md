## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is the length of the string. You can hack this problem only if you solve both problems.</span></p><p>Kirk has a binary string $s$ (a string which consists of zeroes and ones) of length $n$ and he is asking you to find a binary string $t$ of the same length which satisfies the following conditions:</p><ul><li> For any $l$ and $r$ ($1 \leq l \leq r \leq n$) the length of the longest non-decreasing subsequence of the substring $s_{l}s_{l+1} \ldots s_{r}$ is equal to the length of the longest non-decreasing subsequence of the substring $t_{l}t_{l+1} \ldots t_{r}$;</li><li> The number of zeroes in $t$ is the maximum possible.</li></ul><p>A non-decreasing subsequence of a string $p$ is a sequence of indices $i_1, i_2, \ldots, i_k$ such that $i_1 &lt; i_2 &lt; \ldots &lt; i_k$ and $p_{i_1} \leq p_{i_2} \leq \ldots \leq p_{i_k}$. The length of the subsequence is $k$.</p><p>If there are multiple substrings which satisfy the conditions, output any.</p></div><div class="input-specification"><p>The first line contains a binary string of length not more than $2\: 000$.</p></div><div class="output-specification"><p>Output a binary string which satisfied the above conditions. If there are many such strings, output any of them.</p></div>

## Input

<p>The first line contains a binary string of length not more than $2\: 000$.</p>

## Output

<p>Output a binary string which satisfied the above conditions. If there are many such strings, output any of them.</p>





```input1
110
```




```input2
010
```




```input3
0001111
```




```input4
0111001100111011101000
```




```output1
010
```




```output2
010
```




```output3
0000000
```




```output4
0011001100001011101000
```



## Note

<p>In the first example: </p><ul><li> For the substrings of the length $1$ the length of the longest non-decreasing subsequnce is $1$; </li><li> For $l = 1, r = 2$ the longest non-decreasing subsequnce of the substring $s_{1}s_{2}$ is $11$ and the longest non-decreasing subsequnce of the substring $t_{1}t_{2}$ is $01$; </li><li> For $l = 1, r = 3$ the longest non-decreasing subsequnce of the substring $s_{1}s_{3}$ is $11$ and the longest non-decreasing subsequnce of the substring $t_{1}t_{3}$ is $00$; </li><li> For $l = 2, r = 3$ the longest non-decreasing subsequnce of the substring $s_{2}s_{3}$ is $1$ and the longest non-decreasing subsequnce of the substring $t_{2}t_{3}$ is $1$; </li></ul><p>The second example is similar to the first one.</p>
