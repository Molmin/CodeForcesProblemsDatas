## Description

<div><p>You are given a rectangular field of <span class="tex-span"><i>n</i> × <i>m</i></span> cells. Each cell is either empty or impassable (contains an obstacle). Empty cells are marked with '<span class="tex-font-style-tt">.</span>', impassable cells are marked with '<span class="tex-font-style-tt">*</span>'. Let's call two empty cells <span class="tex-font-style-tt">adjacent</span> if they share a side.</p><p>Let's call a <span class="tex-font-style-it">connected component</span> any non-extendible set of cells such that any two of them are connected by the path of adjacent cells. It is a typical well-known definition of a connected component.</p><p>For each impassable cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> imagine that it is an empty cell (all other cells remain unchanged) and find the size (the number of cells) of the connected component which contains <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. You should do it for each impassable cell independently.</p><p>The answer should be printed as a matrix with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. The <span class="tex-span"><i>j</i></span>-th symbol of the <span class="tex-span"><i>i</i></span>-th row should be "<span class="tex-font-style-tt">.</span>" if the cell is empty at the start. Otherwise the <span class="tex-span"><i>j</i></span>-th symbol of the <span class="tex-span"><i>i</i></span>-th row should contain the only digit —- the answer modulo <span class="tex-span">10</span>. The matrix should be printed without any spaces.</p><p>To make your output faster it is recommended to build the output as an array of <span class="tex-span"><i>n</i></span> strings having length <span class="tex-span"><i>m</i></span> and print it as a sequence of lines. It will be much faster than writing character-by-character.</p><p>As input/output can reach huge size it is recommended to use fast input/output methods: for example, prefer to use <span class="tex-font-style-tt">scanf/printf</span> instead of <span class="tex-font-style-tt">cin/cout</span> in C++, prefer to use <span class="tex-font-style-tt">BufferedReader/PrintWriter</span> instead of <span class="tex-font-style-tt">Scanner/System.out</span> in <span class="tex-font-style-tt">Java</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the number of rows and columns in the field.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> symbols: "<span class="tex-font-style-tt">.</span>" for empty cells, "<span class="tex-font-style-tt">*</span>" for impassable cells.</p></div><div class="output-specification"><p>Print the answer as a matrix as described above. See the examples to precise the format of the output.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the number of rows and columns in the field.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> symbols: "<span class="tex-font-style-tt">.</span>" for empty cells, "<span class="tex-font-style-tt">*</span>" for impassable cells.</p>

## Output

<p>Print the answer as a matrix as described above. See the examples to precise the format of the output.</p>





```input1
3 3
*.*
.*.
*.*

```




```input2
4 5
**..*
..***
.*.*.
*.*.*

```




```output1
3.3
.5.
3.3

```




```output2
46..3
..732
.6.4.
5.4.3

```



## Note

<p>In first example, if we imagine that the central cell is empty then it will be included to component of size <span class="tex-span">5</span> (cross). If any of the corner cell will be empty then it will be included to component of size <span class="tex-span">3</span> (corner).</p>
