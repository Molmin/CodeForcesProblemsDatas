## Description

<div><p>Authors have come up with the string $s$ consisting of $n$ lowercase Latin letters.</p><p>You are given two permutations of its indices (not necessary equal) $p$ and $q$ (both of length $n$). Recall that the permutation is the array of length $n$ which contains each integer from $1$ to $n$ exactly once.</p><p>For all $i$ from $1$ to $n-1$ the following properties hold: $s[p_i] \le s[p_{i + 1}]$ and $s[q_i] \le s[q_{i + 1}]$. It means that if you will write down all characters of $s$ in order of permutation indices, the resulting string will be sorted in the non-decreasing order.</p><p>Your task is to restore <span class="tex-font-style-bf">any</span> such string $s$ of length $n$ consisting of <span class="tex-font-style-bf">at least $k$ distinct lowercase Latin letters</span> which suits the given permutations.</p><p>If there are multiple answers, you can print any of them.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5, 1 \le k \le 26$) — the length of the string and the number of distinct characters required.</p><p>The second line of the input contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$, all $p_i$ are distinct integers from $1$ to $n$) — the permutation $p$.</p><p>The third line of the input contains $n$ integers $q_1, q_2, \dots, q_n$ ($1 \le q_i \le n$, all $q_i$ are distinct integers from $1$ to $n$) — the permutation $q$.</p></div><div class="output-specification"><p>If it is impossible to find the suitable string, print "<span class="tex-font-style-tt">NO</span>" on the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" on the first line and string $s$ on the second line. It should consist of $n$ lowercase Latin letters, contain at least $k$ distinct characters and suit the given permutations.</p><p>If there are multiple answers, you can print any of them.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5, 1 \le k \le 26$) — the length of the string and the number of distinct characters required.</p><p>The second line of the input contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$, all $p_i$ are distinct integers from $1$ to $n$) — the permutation $p$.</p><p>The third line of the input contains $n$ integers $q_1, q_2, \dots, q_n$ ($1 \le q_i \le n$, all $q_i$ are distinct integers from $1$ to $n$) — the permutation $q$.</p>

## Output

<p>If it is impossible to find the suitable string, print "<span class="tex-font-style-tt">NO</span>" on the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" on the first line and string $s$ on the second line. It should consist of $n$ lowercase Latin letters, contain at least $k$ distinct characters and suit the given permutations.</p><p>If there are multiple answers, you can print any of them.</p>





```input1
3 2
1 2 3
1 3 2
```




```output1
YES
abb
```


