## Description

<div><p>You are given a description of a depot. It is a rectangular checkered field of <span class="tex-span"><i>n</i> × <i>m</i></span> size. Each cell in a field can be empty ("<span class="tex-font-style-tt">.</span>") or it can be occupied by a wall ("<span class="tex-font-style-tt">*</span>"). </p><p>You have one bomb. If you lay the bomb at the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, then after triggering it will wipe out all walls in the row <span class="tex-span"><i>x</i></span> and all walls in the column <span class="tex-span"><i>y</i></span>.</p><p>You are to determine if it is possible to wipe out all walls in the depot by placing and triggering <span class="tex-font-style-bf">exactly one bomb</span>. The bomb can be laid both in an empty cell or in a cell occupied by a wall.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— the number of rows and columns in the depot field. </p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> symbols "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">*</span>" each&nbsp;— the description of the field. <span class="tex-span"><i>j</i></span>-th symbol in <span class="tex-span"><i>i</i></span>-th of them stands for cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. If the symbol is equal to "<span class="tex-font-style-tt">.</span>", then the corresponding cell is empty, otherwise it equals "<span class="tex-font-style-tt">*</span>" and the corresponding cell is occupied by a wall.</p></div><div class="output-specification"><p>If it is impossible to wipe out all walls by placing and triggering exactly one bomb, then print "<span class="tex-font-style-tt">NO</span>" in the first line (without quotes).</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line and two integers in the second line&nbsp;— the coordinates of the cell at which the bomb should be laid. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>)&nbsp;— the number of rows and columns in the depot field. </p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> symbols "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">*</span>" each&nbsp;— the description of the field. <span class="tex-span"><i>j</i></span>-th symbol in <span class="tex-span"><i>i</i></span>-th of them stands for cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. If the symbol is equal to "<span class="tex-font-style-tt">.</span>", then the corresponding cell is empty, otherwise it equals "<span class="tex-font-style-tt">*</span>" and the corresponding cell is occupied by a wall.</p>

## Output

<p>If it is impossible to wipe out all walls by placing and triggering exactly one bomb, then print "<span class="tex-font-style-tt">NO</span>" in the first line (without quotes).</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line and two integers in the second line&nbsp;— the coordinates of the cell at which the bomb should be laid. If there are multiple answers, print any of them.</p>





```input1
3 4
.*..
....
.*..

```




```input2
3 3
..*
.*.
*..

```




```input3
6 5
..*..
..*..
*****
..*..
..*..
..*..

```




```output1
YES
1 2

```




```output2
NO

```




```output3
YES
3 3

```


