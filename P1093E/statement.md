## Description

<div><p>You are given two permutations $a$ and $b$, both consisting of $n$ elements. Permutation of $n$ elements is such a integer sequence that each value from $1$ to $n$ appears exactly once in it.</p><p>You are asked to perform two types of queries with them:</p><ul> <li> $1~l_a~r_a~l_b~r_b$ — calculate the number of values which appear in both segment $[l_a; r_a]$ of positions in permutation $a$ and segment $[l_b; r_b]$ of positions in permutation $b$; </li><li> $2~x~y$ — swap values on positions $x$ and $y$ in permutation $b$. </li></ul><p>Print the answer for each query of the first type.</p><p>It is guaranteed that there will be at least one query of the first type in the input.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m \le 2 \cdot 10^5$) — the number of elements in both permutations and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) — permutation $a$. It is guaranteed that each value from $1$ to $n$ appears in $a$ exactly once.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le n$) — permutation $b$. It is guaranteed that each value from $1$ to $n$ appears in $b$ exactly once.</p><p>Each of the next $m$ lines contains the description of a certain query. These are either:</p><ul> <li> $1~l_a~r_a~l_b~r_b$ ($1 \le l_a \le r_a \le n$, $1 \le l_b \le r_b \le n$); </li><li> $2~x~y$ ($1 \le x, y \le n$, $x \ne y$). </li></ul></div><div class="output-specification"><p>Print the answers for the queries of the first type, each answer in the new line — the number of values which appear in both segment $[l_a; r_a]$ of positions in permutation $a$ and segment $[l_b; r_b]$ of positions in permutation $b$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m \le 2 \cdot 10^5$) — the number of elements in both permutations and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$) — permutation $a$. It is guaranteed that each value from $1$ to $n$ appears in $a$ exactly once.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le n$) — permutation $b$. It is guaranteed that each value from $1$ to $n$ appears in $b$ exactly once.</p><p>Each of the next $m$ lines contains the description of a certain query. These are either:</p><ul> <li> $1~l_a~r_a~l_b~r_b$ ($1 \le l_a \le r_a \le n$, $1 \le l_b \le r_b \le n$); </li><li> $2~x~y$ ($1 \le x, y \le n$, $x \ne y$). </li></ul>

## Output

<p>Print the answers for the queries of the first type, each answer in the new line — the number of values which appear in both segment $[l_a; r_a]$ of positions in permutation $a$ and segment $[l_b; r_b]$ of positions in permutation $b$.</p>





```input1
6 7
5 1 4 2 3 6
2 5 3 1 4 6
1 1 2 4 5
2 2 4
1 1 2 4 5
1 2 3 3 5
1 1 6 1 2
2 4 1
1 4 4 1 3
```




```output1
1
1
1
2
0
```



## Note

<p>Consider the first query of the first example. Values on positions $[1; 2]$ of $a$ are $[5, 1]$ and values on positions $[4; 5]$ of $b$ are $[1, 4]$. Only value $1$ appears in both segments.</p><p>After the first swap (the second query) permutation $b$ becomes $[2, 1, 3, 5, 4, 6]$.</p><p>After the second swap (the sixth query) permutation $b$ becomes $[5, 1, 3, 2, 4, 6]$.</p>
