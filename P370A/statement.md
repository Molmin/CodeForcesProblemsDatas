## Description

<div><p>Little Petya is learning to play chess. He has already learned how to move a king, a rook and a bishop. Let us remind you the rules of moving chess pieces. A chessboard is 64 square fields organized into an <span class="tex-span">8 × 8</span> table. A field is represented by a pair of integers <span class="tex-span">(<i>r</i>, <i>c</i>)</span> — the number of the row and the number of the column (in a classical game the columns are traditionally indexed by letters). Each chess piece takes up exactly one field. To make a move is to move a chess piece, the pieces move by the following rules:</p><ul> <li> A rook moves any number of fields horizontally or vertically. </li><li> A bishop moves any number of fields diagonally. </li><li> A king moves one field in any direction — horizontally, vertically or diagonally. </li></ul><center> <img class="tex-graphics" src="file://x8PFFUPA.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The pieces move like that</span> </center><p>Petya is thinking about the following problem: what minimum number of moves is needed for each of these pieces to move from field <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> to field <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>? At that, we assume that there are no more pieces besides this one on the board. Help him solve this problem.</p></div><div class="input-specification"><p>The input contains four integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub> ≤ 8</span>) — the coordinates of the starting and the final field. The starting field doesn't coincide with the final one.</p><p>You can assume that the chessboard rows are numbered from top to bottom 1 through 8, and the columns are numbered from left to right 1 through 8.</p></div><div class="output-specification"><p>Print three space-separated integers: the minimum number of moves the rook, the bishop and the king (in this order) is needed to move from field <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> to field <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>. If a piece cannot make such a move, print a 0 instead of the corresponding number.</p></div>

## Input

<p>The input contains four integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub> ≤ 8</span>) — the coordinates of the starting and the final field. The starting field doesn't coincide with the final one.</p><p>You can assume that the chessboard rows are numbered from top to bottom 1 through 8, and the columns are numbered from left to right 1 through 8.</p>

## Output

<p>Print three space-separated integers: the minimum number of moves the rook, the bishop and the king (in this order) is needed to move from field <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> to field <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>. If a piece cannot make such a move, print a 0 instead of the corresponding number.</p>





```input1
4 3 1 6

```




```input2
5 5 5 6

```




```output1
2 1 3

```




```output2
1 0 1

```


