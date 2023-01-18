## Description

<div><p>Sasha and Ira are two best friends. But they aren’t just friends, they are software engineers and experts in artificial intelligence. They are developing an algorithm for two bots playing a two-player game. The game is cooperative and turn based. In each turn, one of the players makes a move (it doesn’t matter which player, it's possible that players turns do not alternate). </p><p>Algorithm for bots that Sasha and Ira are developing works by keeping track of the state the game is in. Each time either bot makes a move, the state changes. And, since the game is very dynamic, it will never go back to the state it was already in at any point in the past.</p><p>Sasha and Ira are perfectionists and want their algorithm to have an optimal winning strategy. They have noticed that in the optimal winning strategy, both bots make exactly <span class="tex-span"><i>N</i></span> moves each. But, in order to find the optimal strategy, their algorithm needs to analyze all possible states of the game (they haven’t learned about alpha-beta pruning yet) and pick the best sequence of moves.</p><p>They are worried about the efficiency of their algorithm and are wondering what is the total number of states of the game that need to be analyzed? </p></div><div class="input-specification"><p>The first and only line contains integer N.</p><ul> <li> <span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">6</sup></span> </li></ul></div><div class="output-specification"><p>Output should contain a single integer – number of possible states modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first and only line contains integer N.</p><ul> <li> <span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">6</sup></span> </li></ul>

## Output

<p>Output should contain a single integer – number of possible states modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2

```




```output1
19

```



## Note

<p>Start: Game is in state A. </p><ul> <li> Turn 1: Either bot can make a move (first bot is red and second bot is blue), so there are two possible states after the first turn – B and C. </li><li> Turn 2: In both states B and C, either bot can again make a turn, so the list of possible states is expanded to include D, E, F and G. </li><li> Turn 3: Red bot already did N=2 moves when in state D, so it cannot make any more moves there. It can make moves when in state E, F and G, so states I, K and M are added to the list. Similarly, blue bot cannot make a move when in state G, but can when in D, E and F, so states H, J and L are added. </li><li> Turn 4: Red bot already did N=2 moves when in states H, I and K, so it can only make moves when in J, L and M, so states P, R and S are added. Blue bot cannot make a move when in states J, L and M, but only when in H, I and K, so states N, O and Q are added. </li></ul><p>Overall, there are 19 possible states of the game their algorithm needs to analyze.</p><p><img class="tex-graphics" src="file://8iaVcnMt.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
