## Description

<div><p>Simon has a rectangular table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Simon numbered the rows of the table from top to bottom starting from one and the columns — from left to right starting from one. We'll represent the cell on the <span class="tex-span"><i>x</i></span>-th row and the <span class="tex-span"><i>y</i></span>-th column as a pair of numbers <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. The table corners are cells: <span class="tex-span">(1, 1)</span>, <span class="tex-span">(<i>n</i>, 1)</span>, <span class="tex-span">(1, <i>m</i>)</span>, <span class="tex-span">(<i>n</i>, <i>m</i>)</span>.</p><p>Simon thinks that some cells in this table are <span class="tex-font-style-it">good</span>. Besides, it's known that no good cell is the corner of the table. </p><p>Initially, all cells of the table are colorless. Simon wants to color all cells of his table. In one move, he can choose any good cell of table <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>, an arbitrary corner of the table <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> and color all cells of the table <span class="tex-span">(<i>p</i>, <i>q</i>)</span>, which meet both inequations: <span class="tex-span"><i>min</i>(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>) ≤ <i>p</i> ≤ <i>max</i>(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span"><i>min</i>(<i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>) ≤ <i>q</i> ≤ <i>max</i>(<i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p><p>Help Simon! Find the minimum number of operations needed to color all cells of the table. Note that you can color one cell multiple times.</p></div><div class="input-specification"><p>The first line contains exactly two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 50</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of the table cells. Specifically, the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>im</i></sub></span>. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> equals zero, then cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> isn't good. Otherwise <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> equals one. It is guaranteed that at least one cell is good. It is guaranteed that no good cell is a corner.</p></div><div class="output-specification"><p>Print a single number — the minimum number of operations Simon needs to carry out his idea.</p></div>

## Input

<p>The first line contains exactly two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 50</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of the table cells. Specifically, the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub>, <i>a</i><sub class="lower-index"><i>i</i>2</sub>, ..., <i>a</i><sub class="lower-index"><i>im</i></sub></span>. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> equals zero, then cell <span class="tex-span">(<i>i</i>, <i>j</i>)</span> isn't good. Otherwise <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> equals one. It is guaranteed that at least one cell is good. It is guaranteed that no good cell is a corner.</p>

## Output

<p>Print a single number — the minimum number of operations Simon needs to carry out his idea.</p>





```input1
3 3
0 0 0
0 1 0
0 0 0

```




```input2
4 3
0 0 0
0 0 1
1 0 0
0 0 0

```




```output1
4

```




```output2
2

```



## Note

<p>In the first sample, the sequence of operations can be like this:</p><center> <img class="tex-graphics" src="file://yjBcptqy.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><ul> <li> For the first time you need to choose cell <span class="tex-span">(2, 2)</span> and corner <span class="tex-span">(1, 1)</span>. </li><li> For the second time you need to choose cell <span class="tex-span">(2, 2)</span> and corner <span class="tex-span">(3, 3)</span>. </li><li> For the third time you need to choose cell <span class="tex-span">(2, 2)</span> and corner <span class="tex-span">(3, 1)</span>. </li><li> For the fourth time you need to choose cell <span class="tex-span">(2, 2)</span> and corner <span class="tex-span">(1, 3)</span>. </li></ul><p>In the second sample the sequence of operations can be like this:</p><center> <img class="tex-graphics" src="file://cxwBiElB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><ul> <li> For the first time you need to choose cell <span class="tex-span">(3, 1)</span> and corner <span class="tex-span">(4, 3)</span>. </li><li> For the second time you need to choose cell <span class="tex-span">(2, 3)</span> and corner <span class="tex-span">(1, 1)</span>.  </li></ul>
