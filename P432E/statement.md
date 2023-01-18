## Description

<div><p>You have an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangle table, its cells are not initially painted. Your task is to paint all cells of the table. The resulting picture should be a tiling of the table with squares. More formally:</p><ul> <li> each cell must be painted some color (the colors are marked by uppercase Latin letters); </li><li> we will assume that two cells of the table are connected if they are of the same color and share a side; each connected region of the table must form a square. </li></ul><p>Given <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, find lexicographically minimum coloring of the table that meets the described properties.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>.</p></div><div class="output-specification"><p>Print lexicographically minimum coloring of the table that meets the described conditions. </p><p>One coloring (let's call it X) is considered lexicographically less than the other one (let's call it Y), if:</p><ul> <li> consider all the table cells from left to right and from top to bottom (first, the first cell in the first row, then the second cell in the first row and so on); </li><li> let's find in this order the first cell that has distinct colors in two colorings; </li><li> the letter that marks the color of the cell in X, goes alphabetically before the letter that marks the color of the cell in Y. </li></ul></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 100)</span>.</p>

## Output

<p>Print lexicographically minimum coloring of the table that meets the described conditions. </p><p>One coloring (let's call it X) is considered lexicographically less than the other one (let's call it Y), if:</p><ul> <li> consider all the table cells from left to right and from top to bottom (first, the first cell in the first row, then the second cell in the first row and so on); </li><li> let's find in this order the first cell that has distinct colors in two colorings; </li><li> the letter that marks the color of the cell in X, goes alphabetically before the letter that marks the color of the cell in Y. </li></ul>





```input1
1 3

```




```input2
2 2

```




```input3
3 4

```




```output1
ABA

```




```output2
AA
AA

```




```output3
AAAB
AAAC
AAAB

```


