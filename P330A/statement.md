## Description

<div><p>You are given a rectangular cake, represented as an <span class="tex-span"><i>r</i> × <i>c</i></span> grid. Each cell either has an evil strawberry, or is empty. For example, a <span class="tex-span">3 × 4</span> cake may look as follows:</p><center> <img class="tex-graphics" src="file://ewFopZFI.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The cakeminator is going to eat the cake! Each time he eats, he chooses a row or a column that does not contain any evil strawberries and contains at least one cake cell that has not been eaten before, and eats all the cake cells there. He may decide to eat any number of times.</p><p>Please output the maximum number of cake cells that the cakeminator can eat.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">2 ≤ <i>r</i>, <i>c</i> ≤ 10</span>), denoting the number of rows and the number of columns of the cake. The next <span class="tex-span"><i>r</i></span> lines each contains <span class="tex-span"><i>c</i></span> characters — the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line denotes the content of the cell at row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span>, and is either one of these: </p><ul> <li> '<span class="tex-font-style-tt">.</span>' character denotes a cake cell with no evil strawberry; </li><li> '<span class="tex-font-style-tt">S</span>' character denotes a cake cell with an evil strawberry. </li></ul></div><div class="output-specification"><p>Output the maximum number of cake cells that the cakeminator can eat.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">2 ≤ <i>r</i>, <i>c</i> ≤ 10</span>), denoting the number of rows and the number of columns of the cake. The next <span class="tex-span"><i>r</i></span> lines each contains <span class="tex-span"><i>c</i></span> characters — the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line denotes the content of the cell at row <span class="tex-span"><i>i</i></span> and column <span class="tex-span"><i>j</i></span>, and is either one of these: </p><ul> <li> '<span class="tex-font-style-tt">.</span>' character denotes a cake cell with no evil strawberry; </li><li> '<span class="tex-font-style-tt">S</span>' character denotes a cake cell with an evil strawberry. </li></ul>

## Output

<p>Output the maximum number of cake cells that the cakeminator can eat.</p>





```input1
3 4
S...
....
..S.

```




```output1
8

```



## Note

<p>For the first example, one possible way to eat the maximum number of cake cells is as follows (perform 3 eats).</p><center> <img class="tex-graphics" src="file://K5Bcr0I2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="file://3w8qLd00.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <img class="tex-graphics" src="file://hXm8nXtz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
