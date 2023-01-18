## Description

<div><p>During the last 24 hours Hamed and Malek spent all their time playing "Sharti". Now they are too exhausted to finish the last round. So they asked you for help to determine the winner of this round. </p><p>"Sharti" is played on a <span class="tex-span"><i>n</i> × <i>n</i></span> board with some of cells colored white and others colored black. The rows of the board are numbered from top to bottom using number <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Also the columns of the board are numbered from left to right using numbers <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The cell located at the intersection of <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column is denoted by <span class="tex-span">(<i>i</i>, <i>j</i>)</span>.</p><p>The players alternatively take turns. In each turn the player must choose a square with side-length at most <span class="tex-span"><i>k</i></span> with its lower-right cell painted white. Then the colors of all the cells in this square are inversed (white cells become black and vice-versa). The player who cannot perform a move in his turn loses. </p><p>You know Hamed and Malek are very clever and they would have played their best moves at each turn. Knowing this and the fact that Hamed takes the first turn, given the initial board as described in the input, you must determine which one of them will be the winner.</p></div><div class="input-specification"><p>In this problem the initial board is specified as a set of <span class="tex-span"><i>m</i></span> rectangles. All cells that lie inside at least one of these rectangles are colored white and the rest are colored black.</p><p>In the first line of input three space-spereated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">4</sup></span>) follow, denoting size of the board, number of rectangles and maximum size of the turn square during the game, respectively.</p><p>In <span class="tex-span"><i>i</i></span>-th line of the next <span class="tex-span"><i>m</i></span> lines four space-seperated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) are given meaning that <span class="tex-span"><i>i</i></span>-th rectangle determining the initial board is a rectangle with upper-left cell at <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> and lower-right cell at <span class="tex-span">(<i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>)</span>.</p></div><div class="output-specification"><p>If Hamed wins, print "Hamed", otherwise print "Malek" (without the quotes).</p></div>

## Input

<p>In this problem the initial board is specified as a set of <span class="tex-span"><i>m</i></span> rectangles. All cells that lie inside at least one of these rectangles are colored white and the rest are colored black.</p><p>In the first line of input three space-spereated integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">4</sup></span>) follow, denoting size of the board, number of rectangles and maximum size of the turn square during the game, respectively.</p><p>In <span class="tex-span"><i>i</i></span>-th line of the next <span class="tex-span"><i>m</i></span> lines four space-seperated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) are given meaning that <span class="tex-span"><i>i</i></span>-th rectangle determining the initial board is a rectangle with upper-left cell at <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> and lower-right cell at <span class="tex-span">(<i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>)</span>.</p>

## Output

<p>If Hamed wins, print "Hamed", otherwise print "Malek" (without the quotes).</p>





```input1
5 2 1
1 1 3 3
2 2 4 4

```




```input2
12 5 7
3 4 5 6
1 2 1 2
4 5 9 9
8 6 12 10
12 4 12 4

```




```output1
Malek

```




```output2
Hamed

```


