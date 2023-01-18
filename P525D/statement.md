## Description

<div><p>Finally it is a day when Arthur has enough money for buying an apartment. He found a great option close to the center of the city with a nice price.</p><p>Plan of the apartment found by Arthur looks like a rectangle <span class="tex-span"><i>n</i> × <i>m</i></span> consisting of squares of size <span class="tex-span">1 × 1</span>. Each of those squares contains either a wall (such square is denoted by a symbol "<span class="tex-font-style-tt">*</span>" on the plan) or a free space (such square is denoted on the plan by a symbol "<span class="tex-font-style-tt">.</span>").</p><p>Room in an apartment is a maximal connected area consisting of free squares. Squares are considered adjacent if they share a common side.</p><p>The old Arthur dream is to live in an apartment where all rooms are rectangles. He asks you to calculate minimum number of walls you need to remove in order to achieve this goal. After removing a wall from a square it becomes a free square. While removing the walls it is possible that some rooms unite into a single one.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>) denoting the size of the Arthur apartments.</p><p>Following <span class="tex-span"><i>n</i></span> lines each contain <span class="tex-span"><i>m</i></span> symbols — the plan of the apartment.</p><p>If the cell is denoted by a symbol "<span class="tex-font-style-tt">*</span>" then it contains a wall.</p><p>If the cell is denoted by a symbol "<span class="tex-font-style-tt">.</span>" then it this cell is free from walls and also this cell is contained in some of the rooms.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> rows each consisting of <span class="tex-span"><i>m</i></span> symbols that show how the Arthur apartment plan should look like after deleting the minimum number of walls in order to make each room (maximum connected area free from walls) be a rectangle. </p><p>If there are several possible answers, output any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>) denoting the size of the Arthur apartments.</p><p>Following <span class="tex-span"><i>n</i></span> lines each contain <span class="tex-span"><i>m</i></span> symbols — the plan of the apartment.</p><p>If the cell is denoted by a symbol "<span class="tex-font-style-tt">*</span>" then it contains a wall.</p><p>If the cell is denoted by a symbol "<span class="tex-font-style-tt">.</span>" then it this cell is free from walls and also this cell is contained in some of the rooms.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> rows each consisting of <span class="tex-span"><i>m</i></span> symbols that show how the Arthur apartment plan should look like after deleting the minimum number of walls in order to make each room (maximum connected area free from walls) be a rectangle. </p><p>If there are several possible answers, output any of them.</p>





```input1
5 5
.*.*.
*****
.*.*.
*****
.*.*.

```




```input2
6 7
***.*.*
..*.*.*
*.*.*.*
*.*.*.*
..*...*
*******

```




```input3
4 5
.....
.....
..***
..*..

```




```output1
.*.*.
*****
.*.*.
*****
.*.*.

```




```output2
***...*
..*...*
..*...*
..*...*
..*...*
*******

```




```output3
.....
.....
.....
.....

```


