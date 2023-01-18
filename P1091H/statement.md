## Description

<div><p>Alice and Bob play a game on a grid with $n$ rows and infinitely many columns. In each row, there are three tokens, blue, white and red one. <span class="tex-font-style-bf">Before</span> the game starts and <span class="tex-font-style-bf">after every move</span>, the following two conditions must hold: </p><ul> <li> Any two tokens are not in the same cell. </li><li> In each row, the blue token is to the left of the white token, and the red token is to the right of the white token. </li></ul><p>First, they pick a positive integer $f$, whose value is valid for the whole game. Second, the starting player is chosen and makes his or her first turn. Then players take alternating turns. The player who is unable to make a move loses. </p><p>During a move, a player first selects an integer $k$ that is either a prime number or a product of two (not necessarily distinct) primes. The smallest possible values of $k$ are thus $2, 3, 4, 5, 6, 7, 9, 10, 11, 13, 14, 15, 17, 19, \dots$. Furthermore, $k$ must not be equal to the previously picked integer $f$. Each turn, a move is performed in exactly one of the rows.</p><p>If it is Alice's turn, she chooses a single blue token and moves it $k$ cells to the right. Alternatively, she may move both the blue and the white token in the same row by the same amount $k$ to the right.</p><p>On the other hand, Bob selects a single red token and moves it $k$ cells to the left. Similarly, he may also move the white and the red token in the corresponding row by $k$ to the left.</p><p>Note that Alice may never move a red token, while Bob may never move a blue one. Remember that after a move, the two conditions on relative positions of the tokens must still hold. </p><p>Both players play optimally. Given the initial state of the board, determine who wins for two games: if Alice starts and if Bob starts. </p></div><div class="input-specification"><p>The first line contains a two integers $n$ and $f$&nbsp;($1 \leq n \leq 10^5$, $2 \leq f \leq 2 \cdot 10^5$)&nbsp;— the number of rows and the forbidden move, respectively.</p><p>Each of the next $n$ lines contains three integers $b_i$, $w_i$, $r_i$&nbsp;($-10^5 \leq b_i &lt; w_i &lt; r_i \leq 10^5$)&nbsp;— the number of column in which the blue, white and red token lies in the $i$-th row, respectively. </p></div><div class="output-specification"><p>Output two lines. </p><p>The first line should contain the name of the winner when Alice starts, and the second line should contain the name of the winner when Bob starts.</p></div>

## Input

<p>The first line contains a two integers $n$ and $f$&nbsp;($1 \leq n \leq 10^5$, $2 \leq f \leq 2 \cdot 10^5$)&nbsp;— the number of rows and the forbidden move, respectively.</p><p>Each of the next $n$ lines contains three integers $b_i$, $w_i$, $r_i$&nbsp;($-10^5 \leq b_i &lt; w_i &lt; r_i \leq 10^5$)&nbsp;— the number of column in which the blue, white and red token lies in the $i$-th row, respectively. </p>

## Output

<p>Output two lines. </p><p>The first line should contain the name of the winner when Alice starts, and the second line should contain the name of the winner when Bob starts.</p>





```input1
1 6
0 3 9
```




```input2
1 2
0 3 9
```




```input3
10 133
-248 -193 -187
97 101 202
-72 67 91
23 89 215
-129 -108 232
-223 -59 236
-99 86 242
-137 -109 -45
-105 173 246
-44 228 243
```




```output1
Alice
Bob
```




```output2
Alice
Bob
```




```output3
Bob
Alice
```



## Note

<p>The first example is as follows:</p><p>When Alice starts, she can win by moving the blue and white token to right by $2$ cells, getting into position $2~5~9$. Regardless of what Bob does, Alice will have one more move and then the game is over. For instance, he can move both the red and white token by $2$ cells to the left, reaching state $2~3~7$. Alice can then move blue and white token by $2$ to move into $4~5~7$, where no more moves are possible.</p><p>If Bob starts, he gains enough advantage to win. For instance, he may move the red token by $3$ to the left, getting into position $0~3~6$. Alice can, for example, move the blue token by $2$, which is countered by Bob by moving the red token by $2$. The game ends in position $2~3~4$. </p><p>In the second example, it is forbidden to move by $2$, but this doesn't stop Alice from winning! She can move the blue and white token by $4$, getting into position $4~7~9$. Now Bob has no move, since moving by $2$ is forbidden.</p>
