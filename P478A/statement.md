## Description

<div><p>There are five people playing a game called "Generosity". Each person gives some non-zero number of coins <span class="tex-span"><i>b</i></span> as an initial bet. After all players make their bets of <span class="tex-span"><i>b</i></span> coins, the following operation is repeated for several times: a coin is passed from one player to some other player.</p><p>Your task is to write a program that can, given the number of coins each player has at the end of the game, determine the size <span class="tex-span"><i>b</i></span> of the initial bet or find out that such outcome of the game cannot be obtained for any positive number of coins <span class="tex-span"><i>b</i></span> in the initial bet.</p></div><div class="input-specification"><p>The input consists of a single line containing five integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">3</sub>, <i>c</i><sub class="lower-index">4</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">5</sub></span> — the number of coins that the first, second, third, fourth and fifth players respectively have at the end of the game (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">3</sub>, <i>c</i><sub class="lower-index">4</sub>, <i>c</i><sub class="lower-index">5</sub> ≤ 100</span>).</p></div><div class="output-specification"><p>Print the only line containing a single positive integer <span class="tex-span"><i>b</i></span> — the number of coins in the initial bet of each player. If there is no such value of <span class="tex-span"><i>b</i></span>, then print the only value "<span class="tex-font-style-tt">-1</span>" (quotes for clarity).</p></div>

## Input

<p>The input consists of a single line containing five integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">3</sub>, <i>c</i><sub class="lower-index">4</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">5</sub></span> — the number of coins that the first, second, third, fourth and fifth players respectively have at the end of the game (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">3</sub>, <i>c</i><sub class="lower-index">4</sub>, <i>c</i><sub class="lower-index">5</sub> ≤ 100</span>).</p>

## Output

<p>Print the only line containing a single positive integer <span class="tex-span"><i>b</i></span> — the number of coins in the initial bet of each player. If there is no such value of <span class="tex-span"><i>b</i></span>, then print the only value "<span class="tex-font-style-tt">-1</span>" (quotes for clarity).</p>





```input1
2 5 4 0 4

```




```input2
4 5 9 2 1

```




```output1
3

```




```output2
-1

```



## Note

<p>In the first sample the following sequence of operations is possible:</p><ol> <li> One coin is passed from the fourth player to the second player; </li><li> One coin is passed from the fourth player to the fifth player; </li><li> One coin is passed from the first player to the third player; </li><li> One coin is passed from the fourth player to the second player. </li></ol>
