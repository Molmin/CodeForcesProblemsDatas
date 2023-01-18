## Description

<div><p>We guessed some integer number $x$. You are given a list of <span class="tex-font-style-bf">almost all</span> its divisors. <span class="tex-font-style-bf">Almost all</span> means that there are <span class="tex-font-style-bf">all divisors except $1$ and $x$</span> in the list.</p><p>Your task is to find the minimum possible integer $x$ that can be the guessed number, or say that the input data is contradictory and it is impossible to find such number.</p><p>You have to answer $t$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 25$) — the number of queries. Then $t$ queries follow.</p><p>The first line of the query contains one integer $n$ ($1 \le n \le 300$) — the number of divisors in the list.</p><p>The second line of the query contains $n$ integers $d_1, d_2, \dots, d_n$ ($2 \le d_i \le 10^6$), where $d_i$ is the $i$-th divisor of the guessed number. It is guaranteed that all values $d_i$ are <span class="tex-font-style-bf">distinct</span>.</p></div><div class="output-specification"><p>For each query print the answer to it.</p><p>If the input data in the query is contradictory and it is impossible to find such number $x$ that the given list of divisors is the list of <span class="tex-font-style-bf">almost all</span> its divisors, print <span class="tex-font-style-tt">-1</span>. Otherwise print the minimum possible $x$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 25$) — the number of queries. Then $t$ queries follow.</p><p>The first line of the query contains one integer $n$ ($1 \le n \le 300$) — the number of divisors in the list.</p><p>The second line of the query contains $n$ integers $d_1, d_2, \dots, d_n$ ($2 \le d_i \le 10^6$), where $d_i$ is the $i$-th divisor of the guessed number. It is guaranteed that all values $d_i$ are <span class="tex-font-style-bf">distinct</span>.</p>

## Output

<p>For each query print the answer to it.</p><p>If the input data in the query is contradictory and it is impossible to find such number $x$ that the given list of divisors is the list of <span class="tex-font-style-bf">almost all</span> its divisors, print <span class="tex-font-style-tt">-1</span>. Otherwise print the minimum possible $x$.</p>





```input1
2
8
8 2 12 6 4 24 16 3
1
2
```




```output1
48
4
```


