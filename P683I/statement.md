## Description

<div><p>A loader works in a warehouse, which is a rectangular field with size <span class="tex-span"><i>n</i> × <i>m</i></span>. Some cells of this field are free, others are occupied by pillars on which the roof of the warehouse rests. </p><p>There is a load in one of the free cells, and the loader in another. At any moment, the loader and the load can not be in the cells with columns, outside the warehouse or in the same cell.</p><p>The loader can move to the adjacent cell (two cells are considered adjacent if they have a common side), or move the load. To move the load, the loader should reach the cell adjacent to the load and push the load. In this case the load advances to the next cell in the direction in which the loader pushes it and the loader ends up in the cell in which the load was.</p><p>Your task is to determine a sequence of pushes and loader's movements after which the load will reach the given cell (it is guaranteed that this cell is free). The load is rather heavy, so you need to minimize first the number of pushes and second the number of loader's movements.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 40</span>, <span class="tex-span"><i>n</i>·<i>m</i> ≥ 3</span>) — the number of rows and columns in the rectangular field.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the warehouse. If there is a character in the next cell of the warehouse:</p><ul> <li> "<span class="tex-font-style-tt">X</span>", it means, that the current cell contains the column; </li><li> "<span class="tex-font-style-tt">.</span>", it means, that the current cell is free; </li><li> "<span class="tex-font-style-tt">Y</span>", it means, that the loader is in the current cell; </li><li> "<span class="tex-font-style-tt">B</span>", it means, that the load is in the current cell; </li><li> "<span class="tex-font-style-tt">T</span>", it means, that the load should be moved to this cell. </li></ul><p>It is guaranteed that there is exactly one load, one loader and one cell to which the load should be moved.</p></div><div class="output-specification"><p>If the loader is not able to move the load to the given cell, print "<span class="tex-font-style-tt">NO</span>" (without the quotes) in the first line of the output.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without the quotes) in the first line of the output, and in the second line — the sequence of characters that determines movements and pushes of the loader. Characters <span class="tex-font-style-tt">w</span>, <span class="tex-font-style-tt">e</span>, <span class="tex-font-style-tt">n</span>, <span class="tex-font-style-tt">s</span> shall denote loader's moves to the west, east, north and south, respectively. Characters <span class="tex-font-style-tt">W</span>, <span class="tex-font-style-tt">E</span>, <span class="tex-font-style-tt">N</span>, <span class="tex-font-style-tt">S</span> must denote loader's pushes in the corresponding directions. First of all you need to minimize the number of pushes of the load and second, the number of movements of the loader. If there are several answers, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 40</span>, <span class="tex-span"><i>n</i>·<i>m</i> ≥ 3</span>) — the number of rows and columns in the rectangular field.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the warehouse. If there is a character in the next cell of the warehouse:</p><ul> <li> "<span class="tex-font-style-tt">X</span>", it means, that the current cell contains the column; </li><li> "<span class="tex-font-style-tt">.</span>", it means, that the current cell is free; </li><li> "<span class="tex-font-style-tt">Y</span>", it means, that the loader is in the current cell; </li><li> "<span class="tex-font-style-tt">B</span>", it means, that the load is in the current cell; </li><li> "<span class="tex-font-style-tt">T</span>", it means, that the load should be moved to this cell. </li></ul><p>It is guaranteed that there is exactly one load, one loader and one cell to which the load should be moved.</p>

## Output

<p>If the loader is not able to move the load to the given cell, print "<span class="tex-font-style-tt">NO</span>" (without the quotes) in the first line of the output.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without the quotes) in the first line of the output, and in the second line — the sequence of characters that determines movements and pushes of the loader. Characters <span class="tex-font-style-tt">w</span>, <span class="tex-font-style-tt">e</span>, <span class="tex-font-style-tt">n</span>, <span class="tex-font-style-tt">s</span> shall denote loader's moves to the west, east, north and south, respectively. Characters <span class="tex-font-style-tt">W</span>, <span class="tex-font-style-tt">E</span>, <span class="tex-font-style-tt">N</span>, <span class="tex-font-style-tt">S</span> must denote loader's pushes in the corresponding directions. First of all you need to minimize the number of pushes of the load and second, the number of movements of the loader. If there are several answers, you are allowed to print any of them.</p>





```input1
3 3
..Y
.BX
..T

```




```input2
3 3
.BY
...
TXX

```




```output1
YES
wSwsE

```




```output2
NO

```


