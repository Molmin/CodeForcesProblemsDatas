## Description

<div><p>Burenka and Tonya are playing an old Buryat game with a chip on a board of $n \times m$ cells.</p><p>At the beginning of the game, the chip is located in the lower left corner of the board. In one move, the player can move the chip to the right or up by any <span class="tex-font-style-bf">odd</span> number of cells (but you cannot move the chip both to the right and up in one move). The one who cannot make a move loses.</p><p>Burenka makes the first move, the players take turns. Burenka really wants to win the game, but she is too lazy to come up with a strategy, so you are invited to solve the difficult task of finding it. Name the winner of the game (it is believed that Burenka and Tonya are masters of playing with chips, so they always move in the optimal way).</p><center> <img class="tex-graphics" src="file://p7Tsevzl.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Chip's starting cell is green, the only cell from which chip can't move is red. if the chip is in the yellow cell, then blue cells are all options to move the chip in one move.</span> </center></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The following is a description of the input data sets.</p><p>The only line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 10^9$) — the dimensions of the game board.</p></div><div class="output-specification"><p>For each test case print a single line — the name of the winner of the game ("<span class="tex-font-style-tt">Burenka</span>" or "<span class="tex-font-style-tt">Tonya</span>").</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The following is a description of the input data sets.</p><p>The only line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 10^9$) — the dimensions of the game board.</p>

## Output

<p>For each test case print a single line — the name of the winner of the game ("<span class="tex-font-style-tt">Burenka</span>" or "<span class="tex-font-style-tt">Tonya</span>").</p>





```input1|2,4,6
6
1 1
1 4
5 6
2 2
6 3
999999999 1000000000
```




```output1
Tonya
Burenka
Burenka
Tonya
Burenka
Burenka
```



## Note

<p>In the first case, Burenka has no move, so Tonya wins.</p><p>In the second case, Burenka can move $3$ cells to the right, after which Tony will not be able to make a move, which means that Burenka wins.</p><p>In the third case, Burenka can move $5$ squares to the right. Then we can say that we have a game on a board of $1 \times 5$ cells, and Tonya is the first player. In such game the second player wins, so in the original one Burenka will win.</p>
