## Description

<div><p>You have a grid with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns. Each cell is either empty (denoted by '<span class="tex-font-style-tt">.</span>') or blocked (denoted by '<span class="tex-font-style-tt">X</span>').</p><p>Two empty cells are <span class="tex-font-style-it">directly connected</span> if they share a side. Two cells <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> (located in the row <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and column <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>) and <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span> are <span class="tex-font-style-it">connected</span> if there exists a sequence of empty cells that starts with <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span>, finishes with <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>, and any two consecutive cells in this sequence are directly connected. A <span class="tex-font-style-it">connected component</span> is a set of empty cells such that any two cells in the component are connected, and there is no cell in this set that is connected to some cell not in this set.</p><p>Your friend Limak is a big grizzly bear. He is able to destroy any obstacles in some range. More precisely, you can choose a square of size <span class="tex-span"><i>k</i> × <i>k</i></span> in the grid and Limak will transform all blocked cells there to empty ones. However, you can ask Limak to help only once.</p><p>The chosen square must be completely inside the grid. It's possible that Limak won't change anything because all cells are empty anyway.</p><p>You like big connected components. After Limak helps you, what is the maximum possible size of the biggest connected component in the grid?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 500</span>)&nbsp;— the size of the grid and Limak's range, respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a string with <span class="tex-span"><i>n</i></span> characters, denoting the <span class="tex-span"><i>i</i></span>-th row of the grid. Each character is '<span class="tex-font-style-tt">.</span>' or '<span class="tex-font-style-tt">X</span>', denoting an empty cell or a blocked one, respectively.</p></div><div class="output-specification"><p>Print the maximum possible size (the number of cells) of the biggest connected component, after using Limak's help.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 500</span>)&nbsp;— the size of the grid and Limak's range, respectively.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a string with <span class="tex-span"><i>n</i></span> characters, denoting the <span class="tex-span"><i>i</i></span>-th row of the grid. Each character is '<span class="tex-font-style-tt">.</span>' or '<span class="tex-font-style-tt">X</span>', denoting an empty cell or a blocked one, respectively.</p>

## Output

<p>Print the maximum possible size (the number of cells) of the biggest connected component, after using Limak's help.</p>





```input1
5 2
..XXX
XX.XX
X.XXX
X...X
XXXX.

```




```input2
5 3
.....
.XXX.
.XXX.
.XXX.
.....

```




```output1
10

```




```output2
25

```



## Note

<p>In the first sample, you can choose a square of size <span class="tex-span">2 × 2</span>. It's optimal to choose a square in the red frame on the left drawing below. Then, you will get a connected component with <span class="tex-span">10</span> cells, marked blue in the right drawing.</p><center> <img class="tex-graphics" src="file://fAVSNMoS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
