## Description

<div><p>Two players play the following game. Initially, the players have a knife and a rectangular sheet of paper, divided into equal square grid cells of unit size. The players make moves in turn, the player who can't make a move loses. In one move, a player can take the knife and cut the paper along any segment of the grid line (not necessarily from border to border). The part of the paper, that touches the knife at least once, is considered cut. There is one limit not to turn the game into an infinite cycle: each move has to cut the paper, that is the knife has to touch the part of the paper that is not cut before.</p><p>Obviously, the game ends when the entire sheet is cut into <span class="tex-span">1 × 1</span> blocks. During the game, the pieces of the sheet are not allowed to move. It is also prohibited to cut along the border. The coordinates of the ends of each cut must be integers.</p><p>You are given an <span class="tex-span"><i>n</i> × <i>m</i></span> piece of paper, somebody has already made <span class="tex-span"><i>k</i></span> cuts there. Your task is to determine who will win if the players start to play on this sheet. You can consider that both players play optimally well. If the first player wins, you also need to find the winning first move.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the sizes of the piece of paper and the number of cuts. Then follow <span class="tex-span"><i>k</i></span> lines, each containing 4 integers <span class="tex-span"><i>xb</i><sub class="lower-index"><i>i</i></sub>, <i>yb</i><sub class="lower-index"><i>i</i></sub>, <i>xe</i><sub class="lower-index"><i>i</i></sub>, <i>ye</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>xb</i><sub class="lower-index"><i>i</i></sub>, <i>xe</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>yb</i><sub class="lower-index"><i>i</i></sub>, <i>ye</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the coordinates of the ends of the existing cuts. </p><p>It is guaranteed that each cut has a non-zero length, is either vertical or horizontal and doesn't go along the sheet border.</p><p>The cuts may intersect, overlap and even be the same. That is, it is not guaranteed that the cuts were obtained during any correct game.</p></div><div class="output-specification"><p>If the second player wins, print "<span class="tex-font-style-tt">SECOND</span>". Otherwise, in the first line print "<span class="tex-font-style-tt">FIRST</span>", and in the second line print any winning move of the first player (the coordinates of the cut ends, follow input format to print them).</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the sizes of the piece of paper and the number of cuts. Then follow <span class="tex-span"><i>k</i></span> lines, each containing 4 integers <span class="tex-span"><i>xb</i><sub class="lower-index"><i>i</i></sub>, <i>yb</i><sub class="lower-index"><i>i</i></sub>, <i>xe</i><sub class="lower-index"><i>i</i></sub>, <i>ye</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>xb</i><sub class="lower-index"><i>i</i></sub>, <i>xe</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 0 ≤ <i>yb</i><sub class="lower-index"><i>i</i></sub>, <i>ye</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the coordinates of the ends of the existing cuts. </p><p>It is guaranteed that each cut has a non-zero length, is either vertical or horizontal and doesn't go along the sheet border.</p><p>The cuts may intersect, overlap and even be the same. That is, it is not guaranteed that the cuts were obtained during any correct game.</p>

## Output

<p>If the second player wins, print "<span class="tex-font-style-tt">SECOND</span>". Otherwise, in the first line print "<span class="tex-font-style-tt">FIRST</span>", and in the second line print any winning move of the first player (the coordinates of the cut ends, follow input format to print them).</p>





```input1
2 1 0

```




```input2
2 2 4
0 1 2 1
0 1 2 1
1 2 1 0
1 1 1 2

```




```output1
FIRST
1 0 1 1

```




```output2
SECOND

```


