## Description

<div><p>Igor is in the museum and he wants to see as many pictures as possible.</p><p>Museum can be represented as a rectangular field of <span class="tex-span"><i>n</i> × <i>m</i></span> cells. Each cell is either empty or impassable. Empty cells are marked with '<span class="tex-font-style-tt">.</span>', impassable cells are marked with '<span class="tex-font-style-tt">*</span>'. Every two adjacent cells of different types (one empty and one impassable) are divided by a wall containing one picture.</p><p>At the beginning Igor is in some empty cell. At every moment he can move to any empty cell that share a side with the current one.</p><p>For several starting positions you should calculate the maximum number of pictures that Igor can see. Igor is able to see the picture only if he is in the cell adjacent to the wall with this picture. Igor have a lot of time, so he will examine every picture he can see.</p></div><div class="input-specification"><p>First line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 1000, 1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 100 000)</span>)&nbsp;— the museum dimensions and the number of starting positions to process.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> symbols '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">*</span>' — the description of the museum. It is guaranteed that all border cells are impassable, so Igor can't go out from the museum.</p><p>Each of the last <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>)&nbsp;— the row and the column of one of Igor's starting positions respectively. Rows are numbered from top to bottom, columns — from left to right. It is guaranteed that all starting positions are empty cells.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> integers&nbsp;— the maximum number of pictures, that Igor can see if he starts in corresponding position.</p></div>

## Input

<p>First line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 1000, 1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 100 000)</span>)&nbsp;— the museum dimensions and the number of starting positions to process.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> symbols '<span class="tex-font-style-tt">.</span>', '<span class="tex-font-style-tt">*</span>' — the description of the museum. It is guaranteed that all border cells are impassable, so Igor can't go out from the museum.</p><p>Each of the last <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>)&nbsp;— the row and the column of one of Igor's starting positions respectively. Rows are numbered from top to bottom, columns — from left to right. It is guaranteed that all starting positions are empty cells.</p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> integers&nbsp;— the maximum number of pictures, that Igor can see if he starts in corresponding position.</p>





```input1
5 6 3
******
*..*.*
******
*....*
******
2 2
2 5
4 3

```




```input2
4 4 1
****
*..*
*.**
****
3 2

```




```output1
6
4
10

```




```output2
8

```


