## Description

<div><p>Consider a game with $n$ cards ($n$ is even). Each card has a number written on it, between $1$ and $n$. All numbers on the cards are different. We say that a card with number $x$ is stronger than a card with number $y$ if $x &gt; y$.</p><p>Two players, Alex and Boris, play this game. In the beginning, each of them receives exactly $\frac{n}{2}$ cards, so each card belongs to exactly one player. Then, they take turns. Alex goes first, then Boris, then Alex again, and so on.</p><p>On a player's turn, he must play <span class="tex-font-style-bf">exactly one</span> of his cards. Then, if the opponent doesn't have any cards <span class="tex-font-style-bf">stronger</span> than the card played, the opponent loses, and the game ends. Otherwise, the opponent has to play a stronger card (exactly one card as well). These two cards are removed from the game, and the turn ends. If there are no cards left, the game ends in a draw; otherwise it's the opponent's turn.</p><p>Consider all possible ways to distribute the cards between two players, so that each of them receives exactly half of the cards. You have to calculate three numbers:</p><ul> <li> the number of ways to distribute the cards so that Alex wins; </li><li> the number of ways to distribute the cards so that Boris wins; </li><li> the number of ways to distribute the cards so that the game ends in a draw. </li></ul><p>You may assume that both players play optimally (i. e. if a player can win no matter how his opponent plays, he wins). Two ways to distribute the cards are different if there is at least one card such that, in one of these ways, it is given to Alex, and in the other way, it is given to Boris.</p><p>For example, suppose $n = 4$, Alex receives the cards $[2, 3]$, and Boris receives the cards $[1, 4]$. Then the game may go as follows:</p><ul> <li> if Alex plays the card $2$, then Boris has to respond with the card $4$. Then, Alex's turn ends, and Boris' turn starts. Boris has only one card left, which is $1$; he plays it, and Alex responds with the card $3$. So, the game ends in a draw; </li><li> if Alex plays the card $3$, then Boris has to respond with the card $4$. Then, Alex's turn ends, and Boris' turn starts. Boris has only one card left, which is $1$; he plays it, and Alex responds with the card $2$. So, the game ends in a draw. </li></ul><p>So, in this case, the game ends in a draw.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 30$)&nbsp;— the number of test cases.</p><p>Then, $t$ lines follow. The $i$-th line contains one <span class="tex-font-style-bf">even</span> integer $n$ ($2 \le n \le 60$).</p></div><div class="output-specification"><p>For each test case, print three integers:</p><ul> <li> the number of ways to distribute the cards so that Alex wins; </li><li> the number of ways to distribute the cards so that Boris wins; </li><li> the number of ways to distribute the cards so that the game ends in a draw. </li></ul><p><span class="tex-font-style-bf">Since the answers can be large, print them modulo $998244353$</span>.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 30$)&nbsp;— the number of test cases.</p><p>Then, $t$ lines follow. The $i$-th line contains one <span class="tex-font-style-bf">even</span> integer $n$ ($2 \le n \le 60$).</p>

## Output

<p>For each test case, print three integers:</p><ul> <li> the number of ways to distribute the cards so that Alex wins; </li><li> the number of ways to distribute the cards so that Boris wins; </li><li> the number of ways to distribute the cards so that the game ends in a draw. </li></ul><p><span class="tex-font-style-bf">Since the answers can be large, print them modulo $998244353$</span>.</p>





```input1|2,4,6
5
2
4
6
8
60
```




```output1
1 0 1
3 2 1
12 7 1
42 27 1
341102826 248150916 1
```



## Note

<p>In the first test case, Alex wins if he receives the card $2$ (he plays it, and Boris cannot respond). If Alex receives the card $1$, the game ends in a draw.</p><p>In the second test case: </p><ul> <li> Alex wins if he receives the cards $[3, 4]$, $[2, 4]$ or $[1, 4]$; </li><li> Boris wins if Alex receives the cards $[1, 2]$ or $[1, 3]$; </li><li> the game ends in a draw if Alex receives the cards $[2, 3]$. </li></ul>
