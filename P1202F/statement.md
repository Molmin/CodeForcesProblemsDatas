## Description

<div><p>You are given $a$ uppercase Latin letters 'A' and $b$ letters 'B'.</p><p>The period of the string is the smallest such positive integer $k$ that $s_i = s_{i~mod~k}$ ($0$-indexed) for each $i$. Note that this implies that $k$ won't always divide $a+b = |s|$.</p><p>For example, the period of string "ABAABAA" is $3$, the period of "AAAA" is $1$, and the period of "AABBB" is $5$.</p><p>Find the number of different periods over all possible strings with $a$ letters 'A' and $b$ letters 'B'.</p></div><div class="input-specification"><p>The first line contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$) — the number of letters 'A' and 'B', respectively.</p></div><div class="output-specification"><p>Print the number of different periods over all possible strings with $a$ letters 'A' and $b$ letters 'B'.</p></div>

## Input

<p>The first line contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$) — the number of letters 'A' and 'B', respectively.</p>

## Output

<p>Print the number of different periods over all possible strings with $a$ letters 'A' and $b$ letters 'B'.</p>





```input1
2 4
```




```input2
5 3
```




```output1
4
```




```output2
5
```



## Note

<p>All the possible periods for the first example: </p><ul> <li> $3$ "BBABBA" </li><li> $4$ "BBAABB" </li><li> $5$ "BBBAAB" </li><li> $6$ "AABBBB" </li></ul><p>All the possible periods for the second example: </p><ul> <li> $3$ "BAABAABA" </li><li> $5$ "BAABABAA" </li><li> $6$ "BABAAABA" </li><li> $7$ "BAABAAAB" </li><li> $8$ "AAAAABBB" </li></ul><p>Note that these are not the only possible strings for the given periods.</p>
