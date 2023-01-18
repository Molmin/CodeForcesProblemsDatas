## Description

<div><p>Door's family is going celebrate Famil Doors's birthday party. They love Famil Door so they are planning to make his birthday cake weird!</p><p>The cake is a <span class="tex-span"><i>n</i> × <i>n</i></span> square consisting of equal squares with side length <span class="tex-span">1</span>. Each square is either empty or consists of a single chocolate. They bought the cake and randomly started to put the chocolates on the cake. The value of Famil Door's happiness will be equal to the number of pairs of cells with chocolates that are in the same row or in the same column of the cake. Famil Doors's family is wondering what is the amount of happiness of Famil going to be?</p><p>Please, note that any pair can be counted no more than once, as two different cells can't share both the same row and the same column.</p></div><div class="input-specification"><p>In the first line of the input, you are given a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the length of the side of the cake.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each containing <span class="tex-span"><i>n</i></span> characters. Empty cells are denoted with '<span class="tex-font-style-tt">.</span>', while cells that contain chocolates are denoted by '<span class="tex-font-style-tt">C</span>'.</p></div><div class="output-specification"><p>Print the value of Famil Door's happiness, i.e. the number of pairs of chocolate pieces that share the same row or the same column.</p></div>

## Input

<p>In the first line of the input, you are given a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the length of the side of the cake.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each containing <span class="tex-span"><i>n</i></span> characters. Empty cells are denoted with '<span class="tex-font-style-tt">.</span>', while cells that contain chocolates are denoted by '<span class="tex-font-style-tt">C</span>'.</p>

## Output

<p>Print the value of Famil Door's happiness, i.e. the number of pairs of chocolate pieces that share the same row or the same column.</p>





```input1
3
.CC
C..
C.C

```




```input2
4
CC..
C..C
.CC.
.CC.

```




```output1
4

```




```output2
9

```



## Note

<p>If we number rows from top to bottom and columns from left to right, then, pieces that share the same row in the first sample are: </p><ol> <li> <span class="tex-span">(1, 2)</span> and <span class="tex-span">(1, 3)</span> </li><li> <span class="tex-span">(3, 1)</span> and <span class="tex-span">(3, 3)</span> </li></ol> Pieces that share the same column are: <ol> <li> <span class="tex-span">(2, 1)</span> and <span class="tex-span">(3, 1)</span> </li><li> <span class="tex-span">(1, 3)</span> and <span class="tex-span">(3, 3)</span> </li></ol>
