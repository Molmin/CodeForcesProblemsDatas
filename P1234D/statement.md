## Description

<div><p>You are given a string $s$ consisting of lowercase Latin letters and $q$ queries for this string.</p><p>Recall that the substring $s[l; r]$ of the string $s$ is the string $s_l s_{l + 1} \dots s_r$. For example, the substrings of "<span class="tex-font-style-tt">codeforces</span>" are "<span class="tex-font-style-tt">code</span>", "<span class="tex-font-style-tt">force</span>", "<span class="tex-font-style-tt">f</span>", "<span class="tex-font-style-tt">for</span>", but not "<span class="tex-font-style-tt">coder</span>" and "<span class="tex-font-style-tt">top</span>".</p><p>There are two types of queries: </p><ul> <li> $1~ pos~ c$ ($1 \le pos \le |s|$, $c$ is lowercase Latin letter): replace $s_{pos}$ with $c$ (set $s_{pos} := c$); </li><li> $2~ l~ r$ ($1 \le l \le r \le |s|$): calculate the number of distinct characters in the substring $s[l; r]$. </li></ul></div><div class="input-specification"><p>The first line of the input contains one string $s$ consisting of no more than $10^5$ lowercase Latin letters.</p><p>The second line of the input contains one integer $q$ ($1 \le q \le 10^5$) — the number of queries.</p><p>The next $q$ lines contain queries, one per line. Each query is given in the format described in the problem statement. It is guaranteed that there is at least one query of the second type.</p></div><div class="output-specification"><p>For each query of the second type print the answer for it — the number of distinct characters in the required substring in this query.</p></div>

## Input

<p>The first line of the input contains one string $s$ consisting of no more than $10^5$ lowercase Latin letters.</p><p>The second line of the input contains one integer $q$ ($1 \le q \le 10^5$) — the number of queries.</p><p>The next $q$ lines contain queries, one per line. Each query is given in the format described in the problem statement. It is guaranteed that there is at least one query of the second type.</p>

## Output

<p>For each query of the second type print the answer for it — the number of distinct characters in the required substring in this query.</p>





```input1
abacaba
5
2 1 4
1 4 b
1 5 b
2 4 6
2 1 7
```




```input2
dfcbbcfeeedbaea
15
1 6 e
1 4 b
2 6 14
1 7 b
1 12 c
2 6 8
2 1 6
1 7 c
1 2 f
1 10 a
2 7 9
1 10 a
1 14 b
1 1 f
2 1 11
```




```output1
3
1
2
```




```output2
5
2
5
2
6
```


