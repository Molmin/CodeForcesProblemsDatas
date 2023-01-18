## Description

<div><p>Kris works in a large company "Blake Technologies". As a best engineer of the company he was assigned a task to develop a printer that will be able to print horizontal and vertical strips. First prototype is already built and Kris wants to tests it. He wants you to implement the program that checks the result of the printing.</p><p>Printer works with a rectangular sheet of paper of size <span class="tex-span"><i>n</i> × <i>m</i></span>. Consider the list as a table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Rows are numbered from top to bottom with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, while columns are numbered from left to right with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Initially, all cells are painted in color <span class="tex-span">0</span>.</p><p>Your program has to support two operations: </p><ol> <li> Paint all cells in row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> in color <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>; </li><li> Paint all cells in column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> in color <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </li></ol><p>If during some operation <span class="tex-span"><i>i</i></span> there is a cell that have already been painted, the color of this cell also changes to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Your program has to print the resulting table after <span class="tex-span"><i>k</i></span> operation.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1  ≤  <i>n</i>,  <i>m</i>  ≤ 5000</span>, <span class="tex-span"><i>n</i>·<i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100 000</span>)&nbsp;— the dimensions of the sheet and the number of operations, respectively.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains the description of exactly one query: </p><ul> <li> <span class="tex-span">1&nbsp;<i>r</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), means that row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is painted in color <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>; </li><li> <span class="tex-span">2&nbsp;<i>c</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), means that column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is painted in color <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> integers each&nbsp;— the resulting table after all operations are applied.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1  ≤  <i>n</i>,  <i>m</i>  ≤ 5000</span>, <span class="tex-span"><i>n</i>·<i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100 000</span>)&nbsp;— the dimensions of the sheet and the number of operations, respectively.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains the description of exactly one query: </p><ul> <li> <span class="tex-span">1&nbsp;<i>r</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), means that row <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is painted in color <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>; </li><li> <span class="tex-span">2&nbsp;<i>c</i><sub class="lower-index"><i>i</i></sub>&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), means that column <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is painted in color <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> integers each&nbsp;— the resulting table after all operations are applied.</p>





```input1
3 3 3
1 1 3
2 2 1
1 2 2

```




```input2
5 3 5
1 1 1
1 3 1
1 5 1
2 1 1
2 3 1

```




```output1
3 1 3 
2 2 2 
0 1 0 

```




```output2
1 1 1 
1 0 1 
1 1 1 
1 0 1 
1 1 1 

```



## Note

<p>The figure below shows all three operations for the first sample step by step. The cells that were painted on the corresponding step are marked gray. </p><center> <img class="tex-graphics" src="file://Rv8YJDdo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
