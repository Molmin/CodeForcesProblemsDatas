## Description

<div><p>Polycarp owns a shop in the capital of Berland. Recently the criminal activity in the capital increased, so Polycarp is thinking about establishing some better security in the storehouse of his shop.</p><p>The storehouse can be represented as a matrix with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Each element of the matrix is either <span class="tex-font-style-tt">.</span> (an empty space) or <span class="tex-font-style-tt">x</span> (a wall).</p><p>Polycarp wants to hire some guards (possibly zero) to watch for the storehouse. Each guard will be in some cell of matrix and will protect every cell to the right of his own cell and every cell to the bottom of his own cell, until the nearest wall. More formally, if the guard is standing in the cell <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>)</span>, then he protects cell <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> if all these conditions are met:</p><ul> <li> <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> is an empty cell; </li><li> either <span class="tex-span"><i>x</i><sub class="lower-index">0</sub> = <i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">0</sub> ≤ <i>y</i><sub class="lower-index">1</sub></span>, or <span class="tex-span"><i>x</i><sub class="lower-index">0</sub> ≤ <i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">0</sub> = <i>y</i><sub class="lower-index">1</sub></span>; </li><li> there are no walls between cells <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>. <span class="tex-font-style-bf">There can be a guard between these cells, guards can look through each other.</span> </li></ul><p>Guards can be placed only in empty cells (and can protect only empty cells). The <span class="tex-font-style-it">plan</span> of placing the guards is some set of cells where guards will be placed (of course, two plans are different if there exists at least one cell that is included in the first plan, but not included in the second plan, or vice versa). Polycarp calls a plan <span class="tex-font-style-it">suitable</span> if there is <span class="tex-font-style-bf">not more than one</span> empty cell that is not protected.</p><p>Polycarp wants to know the number of suitable plans. Since it can be very large, you have to output it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the length and the width of the storehouse (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 250</span>, <span class="tex-span">1 ≤ <i>nm</i> ≤ 250</span>).</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, <span class="tex-span"><i>i</i></span>th line contains a string consisting of <span class="tex-span"><i>m</i></span> characters — <span class="tex-span"><i>i</i></span>th row of the matrix representing the storehouse. Each character is either <span class="tex-font-style-tt">.</span> or <span class="tex-font-style-tt">x</span>.</p></div><div class="output-specification"><p>Output the number of suitable plans modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the length and the width of the storehouse (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 250</span>, <span class="tex-span">1 ≤ <i>nm</i> ≤ 250</span>).</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, <span class="tex-span"><i>i</i></span>th line contains a string consisting of <span class="tex-span"><i>m</i></span> characters — <span class="tex-span"><i>i</i></span>th row of the matrix representing the storehouse. Each character is either <span class="tex-font-style-tt">.</span> or <span class="tex-font-style-tt">x</span>.</p>

## Output

<p>Output the number of suitable plans modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
1 3
.x.

```




```input2
2 2
xx
xx

```




```input3
2 2
..
..

```




```input4
3 1
x
.
x

```




```output1
3

```




```output2
1

```




```output3
10

```




```output4
2

```



## Note

<p>In the first example you have to put at least one guard, so there are three possible arrangements: one guard in the cell <span class="tex-span">(1, 1)</span>, one guard in the cell <span class="tex-span">(1, 3)</span>, and two guards in both these cells.</p>
