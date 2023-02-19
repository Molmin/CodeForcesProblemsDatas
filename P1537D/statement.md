## Description

<div><p>Alice and Bob are playing a game. </p><p>They start with a positive integer $n$ and take alternating turns doing operations on it. Each turn a player can subtract from $n$ one of its divisors that isn't $1$ or $n$. The player who cannot make a move on his/her turn loses. Alice always moves first.</p><p>Note that they subtract a divisor of the <span class="tex-font-style-bf">current</span> number in each turn.</p><p>You are asked to find out who will win the game if both players play optimally.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case contains a single integer $n$ ($1 \leq n \leq 10^9$) — the initial number.</p></div><div class="output-specification"><p>For each test case output "<span class="tex-font-style-tt">Alice</span>" if Alice will win the game or "<span class="tex-font-style-tt">Bob</span>" if Bob will win, if both players play optimally.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case contains a single integer $n$ ($1 \leq n \leq 10^9$) — the initial number.</p>

## Output

<p>For each test case output "<span class="tex-font-style-tt">Alice</span>" if Alice will win the game or "<span class="tex-font-style-tt">Bob</span>" if Bob will win, if both players play optimally.</p>





```input1
4
1
4
12
69
```




```output1
Bob
Alice
Alice
Bob
```



## Note

<p>In the first test case, the game ends immediately because Alice cannot make a move.</p><p>In the second test case, Alice can subtract $2$ making $n = 2$, then Bob cannot make a move so Alice wins.</p><p>In the third test case, Alice can subtract $3$ so that $n = 9$. Bob's only move is to subtract $3$ and make $n = 6$. Now, Alice can subtract $3$ again and $n = 3$. Then Bob cannot make a move, so Alice wins.</p>
