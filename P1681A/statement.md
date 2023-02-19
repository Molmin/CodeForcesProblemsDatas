## Description

<div><p>Alice and Bob play a game. Alice has $n$ cards, the $i$-th of them has the integer $a_i$ written on it. Bob has $m$ cards, the $j$-th of them has the integer $b_j$ written on it.</p><p>On the first turn of the game, <span class="tex-font-style-bf">the first player</span> chooses one of his/her cards and puts it on the table (plays it). On the second turn, <span class="tex-font-style-bf">the second player</span> chooses one of his/her cards <span class="tex-font-style-bf">such that the integer on it is greater than the integer on the card played on the first turn</span>, and plays it. On the third turn, <span class="tex-font-style-bf">the first player</span> chooses one of his/her cards <span class="tex-font-style-bf">such that the integer on it is greater than the integer on the card played on the second turn</span>, and plays it, and so on — the players take turns, and each player has to choose one of his/her cards with greater integer than the card played by the other player on the last turn.</p><p>If some player cannot make a turn, he/she loses.</p><p>For example, if Alice has $4$ cards with numbers $[10, 5, 3, 8]$, and Bob has $3$ cards with numbers $[6, 11, 6]$, the game may go as follows:</p><ul> <li> Alice can choose any of her cards. She chooses the card with integer $5$ and plays it. </li><li> Bob can choose any of his cards with number greater than $5$. He chooses a card with integer $6$ and plays it. </li><li> Alice can choose any of her cards with number greater than $6$. She chooses the card with integer $10$ and plays it. </li><li> Bob can choose any of his cards with number greater than $10$. He chooses a card with integer $11$ and plays it. </li><li> Alice can choose any of her cards with number greater than $11$, but she has no such cards, so she loses. </li></ul><p>Both Alice and Bob play <span class="tex-font-style-bf">optimally (if a player is able to win the game no matter how the other player plays, the former player will definitely win the game)</span>.</p><p>You have to answer two questions:</p><ul> <li> who wins if Alice is the first player? </li><li> who wins if Bob is the first player? </li></ul></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases. Each test case consists of four lines.</p><p>The first line of a test case contains one integer $n$ ($1 \le n \le 50$) — the number of cards Alice has.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 50$) — the numbers written on the cards that Alice has.</p><p>The third line contains one integer $m$ ($1 \le m \le 50$) — the number of Bob's cards.</p><p>The fourth line contains $m$ integers $b_1, b_2, \dots, b_m$ ($1 \le b_i \le 50$) — the numbers on Bob's cards.</p></div><div class="output-specification"><p>For each test case, print two lines. The first line should be <span class="tex-font-style-tt">Alice</span> if Alice wins when she is the first player; otherwise, the first line should be <span class="tex-font-style-tt">Bob</span>. The second line should contain the name of the winner if Bob is the first player, in the same format.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases. Each test case consists of four lines.</p><p>The first line of a test case contains one integer $n$ ($1 \le n \le 50$) — the number of cards Alice has.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 50$) — the numbers written on the cards that Alice has.</p><p>The third line contains one integer $m$ ($1 \le m \le 50$) — the number of Bob's cards.</p><p>The fourth line contains $m$ integers $b_1, b_2, \dots, b_m$ ($1 \le b_i \le 50$) — the numbers on Bob's cards.</p>

## Output

<p>For each test case, print two lines. The first line should be <span class="tex-font-style-tt">Alice</span> if Alice wins when she is the first player; otherwise, the first line should be <span class="tex-font-style-tt">Bob</span>. The second line should contain the name of the winner if Bob is the first player, in the same format.</p>





```input1
4
1
6
2
6 8
4
1 3 3 7
2
4 2
1
50
2
25 50
10
1 2 3 4 5 6 7 8 9 10
2
5 15
```




```output1
Bob
Bob
Alice
Alice
Alice
Bob
Bob
Bob
```



## Note

<p>Let's consider the first test case of the example.</p><p>Alice has one card with integer $6$, Bob has two cards with numbers $[6, 8]$.</p><p>If Alice is the first player, she has to play the card with number $6$. Bob then has to play the card with number $8$. Alice has no cards left, so she loses.</p><p>If Bob is the first player, then no matter which of his cards he chooses on the first turn, Alice won't be able to play her card on the second turn, so she will lose.</p>
