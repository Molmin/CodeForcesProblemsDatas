## Description

<div><p>Xenia likes puzzles very much. She is especially fond of the puzzles that consist of domino pieces. Look at the picture that shows one of such puzzles.</p><center> <img class="tex-graphics" src="file://ob14VUmS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A puzzle is a <span class="tex-span">3 × <i>n</i></span> table with forbidden cells (black squares) containing dominoes (colored rectangles on the picture). A puzzle is called <span class="tex-font-style-it">correct</span> if it meets the following conditions:</p><ul> <li> each domino occupies exactly two non-forbidden cells of the table; </li><li> no two dominoes occupy the same table cell; </li><li> exactly one non-forbidden cell of the table is unoccupied by any domino (it is marked by a circle in the picture). </li></ul><p>To solve the puzzle, you need multiple steps to transport an empty cell from the starting position to some specified position. A move is transporting a domino to the empty cell, provided that the puzzle stays correct. <span class="tex-font-style-bf">The horizontal dominoes can be moved only horizontally, and vertical dominoes can be moved only vertically. You can't rotate dominoes.</span> The picture shows a probable move.</p><p>Xenia has a <span class="tex-span">3 × <i>n</i></span> table with forbidden cells and a cell marked with a circle. Also, Xenia has very many identical dominoes. Now Xenia is wondering, how many distinct correct puzzles she can make if she puts dominoes on the existing table. Also, Xenia wants the circle-marked cell to be empty in the resulting puzzle. The puzzle must contain at least one move.</p><p>Help Xenia, count the described number of puzzles. As the described number can be rather large, print the remainder after dividing it by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>)</span> — the puzzle's size. Each of the following three lines contains <span class="tex-span"><i>n</i></span> characters — the description of the table. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals "<span class="tex-font-style-tt">X</span>" if the corresponding cell is forbidden; it equals "<span class="tex-font-style-tt">.</span>", if the corresponding cell is non-forbidden and "<span class="tex-font-style-tt">O</span>", if the corresponding cell is marked with a circle.</p><p>It is guaranteed that exactly one cell in the table is marked with a circle. It is guaranteed that all cells of a given table having at least one common point with the marked cell is non-forbidden.</p></div><div class="output-specification"><p>Print a single number — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>)</span> — the puzzle's size. Each of the following three lines contains <span class="tex-span"><i>n</i></span> characters — the description of the table. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals "<span class="tex-font-style-tt">X</span>" if the corresponding cell is forbidden; it equals "<span class="tex-font-style-tt">.</span>", if the corresponding cell is non-forbidden and "<span class="tex-font-style-tt">O</span>", if the corresponding cell is marked with a circle.</p><p>It is guaranteed that exactly one cell in the table is marked with a circle. It is guaranteed that all cells of a given table having at least one common point with the marked cell is non-forbidden.</p>

## Output

<p>Print a single number — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
5
....X
.O...
...X.

```




```input2
5
.....
.O...
.....

```




```input3
3
...
...
..O

```




```output1
1

```




```output2
2

```




```output3
4

```



## Note

<p>Two puzzles are considered distinct if there is a pair of cells that contain one domino in one puzzle and do not contain it in the other one.</p>
