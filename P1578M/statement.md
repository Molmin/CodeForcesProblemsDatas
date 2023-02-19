## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>In this problem, you need to come up with a strategy for a cooperative game. This game is played by two players. Each player receives 5 cards. Each card has a random integer between 1 and 100 on it. It is guaranteed that all numbers on cards are distinct.</p><p>The goal of the game is to play a card with a minimal number on it out of all 10 cards dealt to the players before any other card. The problem is that each player can only see their own cards and cannot communicate with another player in any way.</p><p>The game consists of 5 turns. During each turn, players simultaneously make a move. Each player can either play their smallest card or do nothing. If on some turn the smallest card is played, and no other card is played on or before that turn, players win. If two cards are played at the same turn or if after all 5 turns, no card is still played, players lose.</p><p>Players cannot communicate, so a strategy for the game should only be based on 5 cards that the player has. You can describe a strategy as five numbers $0.0 \le p_i \le 1.0, \sum_{i=1}^{5}p_i \le 1$, where $p_i$&nbsp;— the probability of playing the player's smallest card in their hand on $i$-th turn. If you know the cards dealt to the players, and the strategies that players choose, you can compute the probability of winning by a simple formula. </p><p>You will be given $n=1000$ randomly generated hands of 5 cards. You need to generate a strategy for each of the hands to maximize the probability of winning. After the judge program receives all $n$ strategies, it generates all possible valid pairs of those hands (pairs which have the same numbers are discarded), and computes a probability of winning based on two strategies provided by your program. </p><p><span class="tex-font-style-bf">To ensure that answers for different hands are independent, you must output a strategy for a hand and flush the standard output before reading information about the next hand.</span></p><p>If the average probability of winning a game is more than 85% over all valid pairs of hands, the test is considered passed. This problem contains the sample test and $20$ randomly generated tests with $n = 1000$.</p></div><div class="input-specification"><p>The first line contains one integer $n$&nbsp;— the number of hands. It is guaranteed that $n = 1000$ for all cases except the first sample case. </p><p>Each of the next $n$ lines contains 5 numbers $a_i$ ($1 \le a_i \le 100, a_i &lt; a_{i+1}$)&nbsp;— the cards in the hand. It is guaranteed that each possible set of 5 cards has an equal probability of being chosen. </p></div><div class="output-specification"><p>For each of the $n$ hands you need to output 5 numbers $0.0 \le p_i \le 1.0, \sum_{i=1}^{5}p_i \le 1$, where $p_i$&nbsp;— probability of playing the smallest card on $i$-th turn.</p></div>

## Input

<p>The first line contains one integer $n$&nbsp;— the number of hands. It is guaranteed that $n = 1000$ for all cases except the first sample case. </p><p>Each of the next $n$ lines contains 5 numbers $a_i$ ($1 \le a_i \le 100, a_i &lt; a_{i+1}$)&nbsp;— the cards in the hand. It is guaranteed that each possible set of 5 cards has an equal probability of being chosen. </p>

## Output

<p>For each of the $n$ hands you need to output 5 numbers $0.0 \le p_i \le 1.0, \sum_{i=1}^{5}p_i \le 1$, where $p_i$&nbsp;— probability of playing the smallest card on $i$-th turn.</p>





```input1
2
2 12 27 71 100

22 29 39 68 90
```




```output1
0.8 0.2 0.0 0.0 0.0 

0.0 0.2 0.2 0.2 0.3
```



## Note

<p>In the example test there is only one valid pair of hands. The winning probability for the example output is equal to $0.8 + 0.2 \cdot (1 - 0.2) = 0.96$. Also note that the second player will not play a card at all with probability 0.1.</p>
