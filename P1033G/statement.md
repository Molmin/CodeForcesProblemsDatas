## Description

<div><p>Alice and Bob decided to play one ultimate game. They have $n$ piles, the $i$-th pile initially contain $v_i$ chips. Alice selects a positive integer $a$ from interval $[1, m]$, and Bob selects a number $b$ the same way. </p><p>Then the game starts. In her turn, Alice can select any pile containing at least $a$ chips, and remove exactly $a$ chips from it. Similarly, in his turn, Bob can choose any pile with at least $b$ chips, and remove exactly $b$ chips from it. If a player cannot make a move, he or she loses. </p><p>If both players play optimally, the outcome ultimately depends on the choice of $a$ and $b$, and on the starting player. Consider a fixed pair $(a,b)$. There are four types of games: </p><ul> <li> <span class="tex-font-style-bf">Alice</span> wins, regardless of who starts. </li><li> <span class="tex-font-style-bf">Bob</span> wins, regardless of who starts. </li><li> If Alice starts, she wins. If Bob starts, he wins. We say that the <span class="tex-font-style-bf">first</span> player wins. </li><li> If Alice starts, Bob wins. If Bob starts, Alice wins. We say that the <span class="tex-font-style-bf">second</span> player wins. </li></ul><p>Among all choices of $a$ and $b$ (i.e. for each pair $(a, b)$ such that $1\leq a, b\leq m$), determine how many games are won by Alice (regardless of who starts), how many are won by Bob (regardless of who starts), how many are won by the first player, and how many are won by the second player. </p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq n \leq 100, 1 \leq m \leq 10^5$)&nbsp;— the number of piles, and the upper bound on the number of chips allowed to be taken in one turn, respectively. </p><p>The second line contains $n$ integers $v_1, v_2, \dots, v_n$ ($1 \leq v_i \leq 10^{18}$)&nbsp;— the starting number of chips in each pile.</p></div><div class="output-specification"><p>Print a single line containing four integers $w_a$, $w_b$, $w_f$, $w_s$&nbsp;— the number of games won by Alice, Bob, the first player, the second player, respectively. </p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq n \leq 100, 1 \leq m \leq 10^5$)&nbsp;— the number of piles, and the upper bound on the number of chips allowed to be taken in one turn, respectively. </p><p>The second line contains $n$ integers $v_1, v_2, \dots, v_n$ ($1 \leq v_i \leq 10^{18}$)&nbsp;— the starting number of chips in each pile.</p>

## Output

<p>Print a single line containing four integers $w_a$, $w_b$, $w_f$, $w_s$&nbsp;— the number of games won by Alice, Bob, the first player, the second player, respectively. </p>





```input1
2 2
4 5

```




```input2
2 20
4 5

```




```output1
1 1 1 1

```




```output2
82 82 6 230

```



## Note

<p>In the first sample, there are a total of four choices for the tuple $(a,b)$.</p><ul> <li> $a = b = 1$: It does not matter from which pile the chips are removed&nbsp;— there are $9$ turns to be made, and the first player also makes the last, and hence he wins.</li><li> $a = b = 2$: The second player may win by always selecting the same pile as the first before there are $0$ and $1$ chips in the piles. Since it is impossible to remove $2$ chips from any of them, the first player loses.</li><li> $a = 1$ and $b = 2$: <ul> <li> Suppose Alice starts. She can win by removing a single chip from the pile with $5$ chips and then copying Bob's decision. After the next four turns, the game ends with $1$ chip in each pile and Bob unable to make a move. </li><li> Suppose Bob starts. If he removes two chips from second pile, Alice counters by removing a chip from the first pile. From then on, she can always copy Bob's decision and win. If Bob removes two chips from the first pile in his first turn, Alice can also remove one. As the first pile only has one chip left, Bob is forced to remove two chips from the second pile, leaving $3$. Regardless of what Alice does, she wins. </li></ul> Hence, Alice wins no matter who starts.</li><li> $a = 2$ and $b = 1$: This is symmetric with the previous case&nbsp;— hence Bob always wins. </li></ul><p>In the second sample, a lot of games, e.g. $a = 7$ and $b = 6$, end without anybody being able to remove single chip&nbsp;— which counts as a win for the second player. The games won for the first player are $(1, 1)$, $(1, 4)$, $(2, 3)$, $(3, 2)$, $(4, 1)$, and $(5, 5)$.</p>
