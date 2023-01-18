## Description

<div><p>Okabe likes to be able to walk through his city on a path lit by street lamps. That way, he doesn't get beaten up by schoolchildren.</p><p>Okabe's city is represented by a 2D grid of cells. Rows are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom, and columns are numbered <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> from left to right. Exactly <span class="tex-span"><i>k</i></span> cells in the city are lit by a street lamp. It's guaranteed that the top-left cell is lit.</p><p>Okabe starts his walk from the top-left cell, and wants to reach the bottom-right cell. Of course, Okabe will only walk on lit cells, and he can only move to adjacent cells in the up, down, left, and right directions. However, Okabe can also temporarily light all the cells in any single row or column at a time if he pays <span class="tex-span">1</span> coin, allowing him to walk through some cells not lit initially. </p><p>Note that Okabe can only light a single row or column at a time, and has to pay a coin every time he lights a new row or column. To change the row or column that is temporarily lit, he must stand at a cell that is lit initially. Also, once he removes his temporary light from a row or column, all cells in that row/column not initially lit are now not lit.</p><p>Help Okabe find the minimum number of coins he needs to pay to complete his walk!</p></div><div class="input-specification"><p>The first line of input contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains two space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the row and the column of the <span class="tex-span"><i>i</i></span>-th lit cell.</p><p>It is guaranteed that all <span class="tex-span"><i>k</i></span> lit cells are distinct. It is guaranteed that the top-left cell is lit.</p></div><div class="output-specification"><p>Print the minimum number of coins Okabe needs to pay to complete his walk, or <span class="tex-font-style-tt">-1</span> if it's not possible.</p></div>

## Input

<p>The first line of input contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>).</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains two space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the row and the column of the <span class="tex-span"><i>i</i></span>-th lit cell.</p><p>It is guaranteed that all <span class="tex-span"><i>k</i></span> lit cells are distinct. It is guaranteed that the top-left cell is lit.</p>

## Output

<p>Print the minimum number of coins Okabe needs to pay to complete his walk, or <span class="tex-font-style-tt">-1</span> if it's not possible.</p>





```input1
4 4 5
1 1
2 1
2 3
3 3
4 3

```




```input2
5 5 4
1 1
2 1
3 1
3 2

```




```input3
2 2 4
1 1
1 2
2 1
2 2

```




```input4
5 5 4
1 1
2 2
3 3
4 4

```




```output1
2

```




```output2
-1

```




```output3
0

```




```output4
3

```



## Note

<p>In the first sample test, Okabe can take the path <img align="middle" class="tex-formula" src="file://pzmgJF05.png" style="max-width: 100.0%;max-height: 100.0%;">, paying only when moving to <span class="tex-span">(2, 3)</span> and <span class="tex-span">(4, 4)</span>.</p><p>In the fourth sample, Okabe can take the path <img align="middle" class="tex-formula" src="file://8m0geUTz.png" style="max-width: 100.0%;max-height: 100.0%;"> <img align="middle" class="tex-formula" src="file://8qY39RsH.png" style="max-width: 100.0%;max-height: 100.0%;">, paying when moving to <span class="tex-span">(1, 2)</span>, <span class="tex-span">(3, 4)</span>, and <span class="tex-span">(5, 4)</span>.</p>
