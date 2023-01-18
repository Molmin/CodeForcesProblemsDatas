## Description

<div><p>Two pirates Polycarpus and Vasily play a very interesting game. They have <span class="tex-span"><i>n</i></span> chests with coins, the chests are numbered with integers from 1 to <span class="tex-span"><i>n</i></span>. Chest number <span class="tex-span"><i>i</i></span> has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> coins. </p><p>Polycarpus and Vasily move in turns. Polycarpus moves first. During a move a player is allowed to choose a positive integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(2·<i>x</i> + 1 ≤ <i>n</i>)</span> and take a coin from each chest with numbers <span class="tex-span"><i>x</i></span>, <span class="tex-span">2·<i>x</i></span>, <span class="tex-span">2·<i>x</i> + 1</span>. It may turn out that some chest has no coins, in this case the player doesn't take a coin from this chest. The game finishes when all chests get emptied.</p><p>Polycarpus isn't a greedy scrooge. Polycarpys is a lazy slob. So he wonders in what minimum number of moves the game can finish. Help Polycarpus, determine the minimum number of moves in which the game can finish. Note that Polycarpus counts not only his moves, he also counts Vasily's moves.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of chests with coins. The second line contains a sequence of space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of coins in the chest number <span class="tex-span"><i>i</i></span> at the beginning of the game.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of moves needed to finish the game. If no sequence of turns leads to finishing the game, print -1.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of chests with coins. The second line contains a sequence of space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of coins in the chest number <span class="tex-span"><i>i</i></span> at the beginning of the game.</p>

## Output

<p>Print a single integer — the minimum number of moves needed to finish the game. If no sequence of turns leads to finishing the game, print -1.</p>





```input1
1
1

```




```input2
3
1 2 3

```




```output1
-1

```




```output2
3

```



## Note

<p>In the first test case there isn't a single move that can be made. That's why the players won't be able to empty the chests.</p><p>In the second sample there is only one possible move <span class="tex-span"><i>x</i> = 1</span>. This move should be repeated at least 3 times to empty the third chest.</p>
