## Description

<div><p>Let's call a string $t$ consisting of characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span> <span class="tex-font-style-it">beautiful</span>, if either the number of occurrences of character <span class="tex-font-style-tt">0</span> in this string does not exceed $k$, or the number of occurrences of characters <span class="tex-font-style-tt">1</span> in this string does not exceed $k$ (or both). For example, if $k = 3$, the strings <span class="tex-font-style-tt">101010</span>, <span class="tex-font-style-tt">111</span>, <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">00000</span>, <span class="tex-font-style-tt">1111111000</span> are <span class="tex-font-style-it">beautiful</span>, and the strings <span class="tex-font-style-tt">1111110000</span>, <span class="tex-font-style-tt">01010101</span> are not <span class="tex-font-style-it">beautiful</span>.</p><p>You are given a string $s$. You have to divide it into the minimum possible number of <span class="tex-font-style-it">beautiful</span> strings, i. e., find a sequence of strings $t_1, t_2, \dots, t_m$ such that every $t_i$ is <span class="tex-font-style-it">beautiful</span>, $t_1 + t_2 + \dots + t_m = s$ (where $+$ is the concatenation operator), and $m$ is minimum possible.</p><p>For every $k$ from $1$ to $|s|$, find the minimum possible number of strings such that $s$ can be divided into them (i. e. the minimum possible $m$ in the partition).</p></div><div class="input-specification"><p>The only line contains one string $s$ ($1 \le |s| \le 2 \cdot 10^5$). Each character of $s$ is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>Print $|s|$ integers. The $i$-th integer should be equal to the minimum number of strings in the partition of $s$, when $k = i$.</p></div>

## Input

<p>The only line contains one string $s$ ($1 \le |s| \le 2 \cdot 10^5$). Each character of $s$ is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>Print $|s|$ integers. The $i$-th integer should be equal to the minimum number of strings in the partition of $s$, when $k = i$.</p>





```input1
00100010
```




```input2
1001011100
```




```output1
2 1 1 1 1 1 1 1
```




```output2
3 2 2 2 1 1 1 1 1 1
```


