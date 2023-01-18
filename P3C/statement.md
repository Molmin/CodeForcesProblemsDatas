## Description

<div><p>Certainly, everyone is familiar with tic-tac-toe game. The rules are very simple indeed. Two players take turns marking the cells in a <span class="tex-span">3 × 3</span> grid (one player always draws crosses, the other — noughts). The player who succeeds first in placing three of his marks in a horizontal, vertical or diagonal line wins, and the game is finished. The player who draws crosses goes first. If the grid is filled, but neither Xs, nor 0s form the required line, a draw is announced.</p><p>You are given a <span class="tex-span">3 × 3</span> grid, each grid cell is empty, or occupied by a cross or a nought. You have to find the player (first or second), whose turn is next, or print one of the verdicts below: </p><ul> <li> <span class="tex-font-style-tt">illegal</span> — if the given board layout can't appear during a valid game; </li><li> <span class="tex-font-style-tt">the first player won</span> — if in the given board layout the first player has just won; </li><li> <span class="tex-font-style-tt">the second player won</span> — if in the given board layout the second player has just won; </li><li> <span class="tex-font-style-tt">draw</span> — if the given board layout has just let to a draw. </li></ul></div><div class="input-specification"><p>The input consists of three lines, each of the lines contains characters "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">X</span>" or "<span class="tex-font-style-tt">0</span>" (a period, a capital letter X, or a digit zero).</p></div><div class="output-specification"><p>Print one of the six verdicts: <span class="tex-font-style-tt">first</span>, <span class="tex-font-style-tt">second</span>, <span class="tex-font-style-tt">illegal</span>, <span class="tex-font-style-tt">the first player won</span>, <span class="tex-font-style-tt">the second player won</span> or <span class="tex-font-style-tt">draw</span>.</p></div>

## Input

<p>The input consists of three lines, each of the lines contains characters "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">X</span>" or "<span class="tex-font-style-tt">0</span>" (a period, a capital letter X, or a digit zero).</p>

## Output

<p>Print one of the six verdicts: <span class="tex-font-style-tt">first</span>, <span class="tex-font-style-tt">second</span>, <span class="tex-font-style-tt">illegal</span>, <span class="tex-font-style-tt">the first player won</span>, <span class="tex-font-style-tt">the second player won</span> or <span class="tex-font-style-tt">draw</span>.</p>





```input1
X0X
.0.
.X.

```




```output1
second

```


