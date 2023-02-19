## Description

<div><p>You are given $n$ words of <span class="tex-font-style-bf">equal</span> length $m$, consisting of lowercase Latin alphabet letters. The $i$-th word is denoted $s_i$.</p><p>In one move you can choose <span class="tex-font-style-bf">any position in any single word</span> and change the letter at that position to the previous or next letter in alphabetical order. For example:</p><ul> <li> you can change '<span class="tex-font-style-tt">e</span>' to '<span class="tex-font-style-tt">d</span>' or to '<span class="tex-font-style-tt">f</span>'; </li><li> '<span class="tex-font-style-tt">a</span>' can only be changed to '<span class="tex-font-style-tt">b</span>'; </li><li> '<span class="tex-font-style-tt">z</span>' can only be changed to '<span class="tex-font-style-tt">y</span>'. </li></ul><p>The <span class="tex-font-style-it">difference</span> between two words is the <span class="tex-font-style-bf">minimum</span> number of moves required to make them equal. For example, the <span class="tex-font-style-it">difference</span> between "<span class="tex-font-style-tt">best</span>" and "<span class="tex-font-style-tt">cost</span>" is $1 + 10 + 0 + 0 = 11$.</p><p>Find the minimum <span class="tex-font-style-it">difference</span> of $s_i$ and $s_j$ such that $(i &lt; j)$. In other words, find the minimum <span class="tex-font-style-it">difference</span> over all possible pairs of the $n$ words.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains $2$ integers $n$ and $m$ ($2 \leq n \leq 50$, $1 \leq m \leq 8$) — the number of strings and their length respectively.</p><p>Then follows $n$ lines, the $i$-th of which containing a single string $s_i$ of length $m$, consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>For each test case, print a single integer — the minimum <span class="tex-font-style-it">difference</span> over all possible pairs of the given strings.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains $2$ integers $n$ and $m$ ($2 \leq n \leq 50$, $1 \leq m \leq 8$) — the number of strings and their length respectively.</p><p>Then follows $n$ lines, the $i$-th of which containing a single string $s_i$ of length $m$, consisting of lowercase Latin letters.</p>

## Output

<p>For each test case, print a single integer — the minimum <span class="tex-font-style-it">difference</span> over all possible pairs of the given strings.</p>





```input1
6
2 4
best
cost
6 3
abb
zba
bef
cdu
ooo
zzz
2 7
aaabbbc
bbaezfe
3 2
ab
ab
ab
2 8
aaaaaaaa
zzzzzzzz
3 1
a
u
y
```




```output1
11
8
35
0
200
4
```



## Note

<p>For the second test case, one can show that the best pair is ("<span class="tex-font-style-tt">abb</span>","<span class="tex-font-style-tt">bef</span>"), which has <span class="tex-font-style-it">difference</span> equal to $8$, which can be obtained in the following way: change the first character of the first string to '<span class="tex-font-style-tt">b</span>' in one move, change the second character of the second string to '<span class="tex-font-style-tt">b</span>' in $3$ moves and change the third character of the second string to '<span class="tex-font-style-tt">b</span>' in $4$ moves, thus making in total $1 + 3 + 4 = 8$ moves.</p><p>For the third test case, there is only one possible pair and it can be shown that the minimum amount of moves necessary to make the strings equal is $35$.</p><p>For the fourth test case, there is a pair of strings which is already equal, so the answer is $0$.</p>
