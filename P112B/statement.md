## Description

<div><p>Little Petya loves playing with squares. Mum bought him a square <span class="tex-span">2<i>n</i> × 2<i>n</i></span> in size. Petya marked a cell inside the square and now he is solving the following task.</p><p>The task is to draw a broken line that would go along the grid lines and that would cut the square into two equal parts. The cutting line should not have any common points with the marked cell and the resulting two parts should be equal <span class="tex-font-style-bf">up to rotation</span>.</p><p>Petya wants to determine whether it is possible to cut the square in the required manner given the sizes of the square side and the coordinates of the marked cell. Help him.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span">2<i>n</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">2 ≤ 2<i>n</i> ≤ 100, 1 ≤ <i>x</i>, <i>y</i> ≤ 2<i>n</i></span>), representing the length of a square's side and the coordinates of the marked cell. It is guaranteed that <span class="tex-span">2<i>n</i></span> is even.</p><p>The coordinates of the marked cell are represented by a pair of numbers <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>, where <span class="tex-span"><i>x</i></span> represents the number of the row and <span class="tex-span"><i>y</i></span> represents the number of the column. The rows and columns are numbered by consecutive integers from <span class="tex-span">1</span> to <span class="tex-span">2<i>n</i></span>. The rows are numbered from top to bottom and the columns are numbered from the left to the right.</p></div><div class="output-specification"><p>If the square is possible to cut, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span">2<i>n</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">2 ≤ 2<i>n</i> ≤ 100, 1 ≤ <i>x</i>, <i>y</i> ≤ 2<i>n</i></span>), representing the length of a square's side and the coordinates of the marked cell. It is guaranteed that <span class="tex-span">2<i>n</i></span> is even.</p><p>The coordinates of the marked cell are represented by a pair of numbers <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>, where <span class="tex-span"><i>x</i></span> represents the number of the row and <span class="tex-span"><i>y</i></span> represents the number of the column. The rows and columns are numbered by consecutive integers from <span class="tex-span">1</span> to <span class="tex-span">2<i>n</i></span>. The rows are numbered from top to bottom and the columns are numbered from the left to the right.</p>

## Output

<p>If the square is possible to cut, print "<span class="tex-font-style-tt">YES</span>", otherwise print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
4 1 1

```




```input2
2 2 2

```




```output1
YES

```




```output2
NO

```



## Note

<p>A sample test from the statement and one of the possible ways of cutting the square are shown in the picture: </p><center> <img class="tex-graphics" src="file://wqC0IsvL.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
