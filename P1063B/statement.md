## Description

<div><p>You are playing some computer game. One of its levels puts you in a maze consisting of <span class="tex-span"><i>n</i></span> lines, each of which contains <span class="tex-span"><i>m</i></span> cells. Each cell either is free or is occupied by an obstacle. The starting cell is in the row <span class="tex-span"><i>r</i></span> and column <span class="tex-span"><i>c</i></span>. In one step you can move one square up, left, down or right, if the target cell is not occupied by an obstacle. You can't move beyond the boundaries of the labyrinth.</p><p>Unfortunately, your keyboard is about to break, so you can move left no more than <span class="tex-span"><i>x</i></span> times and move right no more than <span class="tex-span"><i>y</i></span> times. There are no restrictions on the number of moves up and down since the keys used to move up and down are in perfect condition.</p><p>Now you would like to determine for each cell whether there exists a sequence of moves that will put you from the starting cell to this particular one. How many cells of the board have this property?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>)&nbsp;— the number of rows and the number columns in the labyrinth respectively.</p><p>The second line contains two integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ <i>m</i></span>)&nbsp;— index of the row and index of the column that define the starting cell.</p><p>The third line contains two integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the maximum allowed number of movements to the left and to the right respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe the labyrinth. Each of them has length of <span class="tex-span"><i>m</i></span> and consists only of symbols '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">*</span>'. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line corresponds to the cell of labyrinth at row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span>. Symbol '<span class="tex-font-style-tt">.</span>' denotes the free cell, while symbol '<span class="tex-font-style-tt">*</span>' denotes the cell with an obstacle.</p><p>It is guaranteed, that the starting cell contains no obstacles.</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— the number of cells in the labyrinth, which are reachable from starting cell, including the starting cell itself.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>)&nbsp;— the number of rows and the number columns in the labyrinth respectively.</p><p>The second line contains two integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ <i>m</i></span>)&nbsp;— index of the row and index of the column that define the starting cell.</p><p>The third line contains two integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">0 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the maximum allowed number of movements to the left and to the right respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe the labyrinth. Each of them has length of <span class="tex-span"><i>m</i></span> and consists only of symbols '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">*</span>'. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line corresponds to the cell of labyrinth at row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span>. Symbol '<span class="tex-font-style-tt">.</span>' denotes the free cell, while symbol '<span class="tex-font-style-tt">*</span>' denotes the cell with an obstacle.</p><p>It is guaranteed, that the starting cell contains no obstacles.</p>

## Output

<p>Print exactly one integer&nbsp;— the number of cells in the labyrinth, which are reachable from starting cell, including the starting cell itself.</p>





```input1
4 5
3 2
1 2
.....
.***.
...**
*....

```




```input2
4 4
2 2
0 1
....
..*.
....
....

```




```output1
10

```




```output2
7

```



## Note

<p>Cells, reachable in the corresponding example, are marked with '<span class="tex-font-style-tt">+</span>'.</p><p>First example: </p><center> <pre class="verbatim"><br>+++..<br>+***.<br>+++**<br>*+++.<br></pre> </center><p>Second example: </p><center> <pre class="verbatim"><br>.++.<br>.+*.<br>.++.<br>.++.<br></pre> </center>
