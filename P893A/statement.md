## Description

<div><p>Alex, Bob and Carl will soon participate in a team chess tournament. Since they are all in the same team, they have decided to practise really hard before the tournament. But it's a bit difficult for them because chess is a game for two players, not three.</p><p>So they play with each other according to following rules:</p><ul> <li> Alex and Bob play the first game, and Carl is spectating; </li><li> When the game ends, the one who lost the game becomes the spectator in the next game, and the one who was spectating plays against the winner. </li></ul><p>Alex, Bob and Carl play in such a way that there are no draws.</p><p>Today they have played <span class="tex-span"><i>n</i></span> games, and for each of these games they remember who was the winner. They decided to make up a log of games describing who won each game. But now they doubt if the information in the log is correct, and they want to know if the situation described in the log they made up was possible (that is, no game is won by someone who is spectating if Alex, Bob and Carl play according to the rules). Help them to check it!</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of games Alex, Bob and Carl played.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, describing the game log. <span class="tex-span"><i>i</i></span>-th line contains one integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>) which is equal to <span class="tex-span">1</span> if Alex won <span class="tex-span"><i>i</i></span>-th game, to <span class="tex-span">2</span> if Bob won <span class="tex-span"><i>i</i></span>-th game and <span class="tex-span">3</span> if Carl won <span class="tex-span"><i>i</i></span>-th game.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">YES</span> if the situation described in the log was possible. Otherwise print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of games Alex, Bob and Carl played.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, describing the game log. <span class="tex-span"><i>i</i></span>-th line contains one integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>) which is equal to <span class="tex-span">1</span> if Alex won <span class="tex-span"><i>i</i></span>-th game, to <span class="tex-span">2</span> if Bob won <span class="tex-span"><i>i</i></span>-th game and <span class="tex-span">3</span> if Carl won <span class="tex-span"><i>i</i></span>-th game.</p>

## Output

<p>Print <span class="tex-font-style-tt">YES</span> if the situation described in the log was possible. Otherwise print <span class="tex-font-style-tt">NO</span>.</p>





```input1
3
1
1
2

```




```input2
2
1
2

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first example the possible situation is:</p><ol> <li> Alex wins, Carl starts playing instead of Bob; </li><li> Alex wins, Bob replaces Carl; </li><li> Bob wins. </li></ol><p>The situation in the second example is impossible because Bob loses the first game, so he cannot win the second one.</p>
