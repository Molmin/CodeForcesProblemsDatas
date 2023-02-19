## Description

<div><p>You are given an array $a$ consisting of $n$ positive integers, and an array $b$, with length $n$. Initially $b_i=0$ for each $1 \leq i \leq n$.</p><p>In one move you can choose an integer $i$ ($1 \leq i \leq n$), and add $a_i$ to $b_i$ or subtract $a_i$ from $b_i$. What is the minimum number of moves needed to make $b$ increasing (that is, every element is strictly greater than every element before it)?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \leq n \leq 5000$).</p><p>The second line contains $n$ integers, $a_1$, $a_2$, ..., $a_n$ ($1 \leq a_i \leq 10^9$) — the elements of the array $a$.</p></div><div class="output-specification"><p>Print a single integer, the minimum number of moves to make $b$ increasing.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \leq n \leq 5000$).</p><p>The second line contains $n$ integers, $a_1$, $a_2$, ..., $a_n$ ($1 \leq a_i \leq 10^9$) — the elements of the array $a$.</p>

## Output

<p>Print a single integer, the minimum number of moves to make $b$ increasing.</p>





```input1
5
1 2 3 4 5
```




```input2
7
1 2 1 2 1 2 1
```




```input3
8
1 8 2 7 3 6 4 5
```




```output1
4
```




```output2
10
```




```output3
16
```



## Note

<p>Example $1$: you can subtract $a_1$ from $b_1$, and add $a_3$, $a_4$, and $a_5$ to $b_3$, $b_4$, and $b_5$ respectively. The final array will be [$-1$, $0$, $3$, $4$, $5$] after $4$ moves.</p><p>Example $2$: you can reach [$-3$, $-2$, $-1$, $0$, $1$, $2$, $3$] in $10$ moves.</p>
