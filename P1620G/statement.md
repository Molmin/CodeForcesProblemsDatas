## Description

<div><p>For a sequence of strings $[t_1, t_2, \dots, t_m]$, let's define the function $f([t_1, t_2, \dots, t_m])$ as the number of different strings (<span class="tex-font-style-bf">including the empty string</span>) that are subsequences of <span class="tex-font-style-bf">at least one</span> string $t_i$. $f([]) = 0$ (i. e. the number of such strings for an empty sequence is $0$).</p><p>You are given a sequence of strings $[s_1, s_2, \dots, s_n]$. Every string in this sequence consists of lowercase Latin letters and is <span class="tex-font-style-bf">sorted</span> (i. e., each string begins with several (maybe zero) characters <span class="tex-font-style-tt">a</span>, then several (maybe zero) characters <span class="tex-font-style-tt">b</span>, ..., ends with several (maybe zero) characters <span class="tex-font-style-tt">z</span>).</p><p>For each of $2^n$ subsequences of $[s_1, s_2, \dots, s_n]$, calculate the value of the function $f$ modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 23$) — the number of strings.</p><p>Then $n$ lines follow. The $i$-th line contains the string $s_i$ ($1 \le |s_i| \le 2 \cdot 10^4$), consisting of lowercase Latin letters. Each string $s_i$ is sorted.</p></div><div class="output-specification"><p>Since printing up to $2^{23}$ integers would be really slow, you should do the following:</p><p>For each of the $2^n$ subsequences (which we denote as $[s_{i_1}, s_{i_2}, \dots, s_{i_k}]$), calculate $f([s_{i_1}, s_{i_2}, \dots, s_{i_k}])$, take it modulo $998244353$, then multiply it by $k \cdot (i_1 + i_2 + \dots + i_k)$. Print the XOR of all $2^n$ integers you get.</p><p>The indices $i_1, i_2, \dots, i_k$ in the description of each subsequences are $1$-indexed (i. e. are from $1$ to $n$).</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 23$) — the number of strings.</p><p>Then $n$ lines follow. The $i$-th line contains the string $s_i$ ($1 \le |s_i| \le 2 \cdot 10^4$), consisting of lowercase Latin letters. Each string $s_i$ is sorted.</p>

## Output

<p>Since printing up to $2^{23}$ integers would be really slow, you should do the following:</p><p>For each of the $2^n$ subsequences (which we denote as $[s_{i_1}, s_{i_2}, \dots, s_{i_k}]$), calculate $f([s_{i_1}, s_{i_2}, \dots, s_{i_k}])$, take it modulo $998244353$, then multiply it by $k \cdot (i_1 + i_2 + \dots + i_k)$. Print the XOR of all $2^n$ integers you get.</p><p>The indices $i_1, i_2, \dots, i_k$ in the description of each subsequences are $1$-indexed (i. e. are from $1$ to $n$).</p>





```input1
3
a
b
c
```




```input2
2
aa
a
```




```input3
2
a
a
```




```input4
2
abcd
aabb
```




```input5
3
ddd
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaabbbbbbbbbbbcccccccccccciiiiiiiiiiiiiiiiiiiiiiooooooooooqqqqqqqqqqqqqqqqqqvvvvvzzzzzzzzzzzz
```




```output1
92
```




```output2
21
```




```output3
10
```




```output4
124
```




```output5
15706243380
```


