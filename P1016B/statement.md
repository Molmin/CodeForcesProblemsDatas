## Description

<div><p>You are given two strings $s$ and $t$, both consisting only of lowercase Latin letters.</p><p>The substring $s[l..r]$ is the string which is obtained by taking characters $s_l, s_{l + 1}, \dots, s_r$ without changing the order.</p><p>Each of the occurrences of string $a$ in a string $b$ is a position $i$ ($1 \le i \le |b| - |a| + 1$) such that $b[i..i + |a| - 1] = a$ ($|a|$ is the length of string $a$).</p><p>You are asked $q$ queries: for the $i$-th query you are required to calculate the number of occurrences of string $t$ in a substring $s[l_i..r_i]$.</p></div><div class="input-specification"><p>The first line contains three integer numbers $n$, $m$ and $q$ ($1 \le n, m \le 10^3$, $1 \le q \le 10^5$) — the length of string $s$, the length of string $t$ and the number of queries, respectively.</p><p>The second line is a string $s$ ($|s| = n$), consisting only of lowercase Latin letters.</p><p>The third line is a string $t$ ($|t| = m$), consisting only of lowercase Latin letters.</p><p>Each of the next $q$ lines contains two integer numbers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) — the arguments for the $i$-th query.</p></div><div class="output-specification"><p>Print $q$ lines — the $i$-th line should contain the answer to the $i$-th query, that is the number of occurrences of string $t$ in a substring $s[l_i..r_i]$.</p></div>

## Input

<p>The first line contains three integer numbers $n$, $m$ and $q$ ($1 \le n, m \le 10^3$, $1 \le q \le 10^5$) — the length of string $s$, the length of string $t$ and the number of queries, respectively.</p><p>The second line is a string $s$ ($|s| = n$), consisting only of lowercase Latin letters.</p><p>The third line is a string $t$ ($|t| = m$), consisting only of lowercase Latin letters.</p><p>Each of the next $q$ lines contains two integer numbers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) — the arguments for the $i$-th query.</p>

## Output

<p>Print $q$ lines — the $i$-th line should contain the answer to the $i$-th query, that is the number of occurrences of string $t$ in a substring $s[l_i..r_i]$.</p>





```input1
10 3 4
codeforces
for
1 3
3 10
5 6
5 7

```




```input2
15 2 3
abacabadabacaba
ba
1 15
3 4
2 14

```




```input3
3 5 2
aaa
baaab
1 3
1 1

```




```output1
0
1
0
1

```




```output2
4
0
3

```




```output3
0
0

```



## Note

<p>In the first example the queries are substrings: "<span class="tex-font-style-tt">cod</span>", "<span class="tex-font-style-tt">deforces</span>", "<span class="tex-font-style-tt">fo</span>" and "<span class="tex-font-style-tt">for</span>", respectively.</p>
