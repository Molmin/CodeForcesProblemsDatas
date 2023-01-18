## Description

<div><p>There is a rectangular grid of <span class="tex-span"><i>n</i></span> rows of <span class="tex-span"><i>m</i></span> initially-white cells each.</p><p>Arkady performed a certain number (possibly zero) of operations on it. In the <span class="tex-span"><i>i</i></span>-th operation, a non-empty subset of rows <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> and a non-empty subset of columns <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span> are chosen. For each row <span class="tex-span"><i>r</i></span> in <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> and each column <span class="tex-span"><i>c</i></span> in <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span>, the intersection of row <span class="tex-span"><i>r</i></span> and column <span class="tex-span"><i>c</i></span> is coloured black.</p><p>There's another constraint: a row or a column can only be chosen at most once among all operations. In other words, it means that no pair of <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span"><i>i</i> &lt; <i>j</i></span>) exists such that <img align="middle" class="tex-formula" src="file://N23NmW9X.png" style="max-width: 100.0%;max-height: 100.0%;"> or <img align="middle" class="tex-formula" src="file://nI6oUwtK.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://qvXngB8x.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes intersection of sets, and <img align="middle" class="tex-formula" src="file://1JCRUI32.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the empty set.</p><p>You are to determine whether a valid sequence of operations exists that produces a given final grid.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>)&nbsp;— the number of rows and columns of the grid, respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains a string of <span class="tex-span"><i>m</i></span> characters, each being either '<span class="tex-font-style-tt">.</span>' (denoting a white cell) or '<span class="tex-font-style-tt">#</span>' (denoting a black cell), representing the desired setup.</p></div><div class="output-specification"><p>If the given grid can be achieved by any valid sequence of operations, output "<span class="tex-font-style-tt">Yes</span>"; otherwise output "<span class="tex-font-style-tt">No</span>" (both without quotes).</p><p>You can print each character in any case (upper or lower).</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>)&nbsp;— the number of rows and columns of the grid, respectively.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains a string of <span class="tex-span"><i>m</i></span> characters, each being either '<span class="tex-font-style-tt">.</span>' (denoting a white cell) or '<span class="tex-font-style-tt">#</span>' (denoting a black cell), representing the desired setup.</p>

## Output

<p>If the given grid can be achieved by any valid sequence of operations, output "<span class="tex-font-style-tt">Yes</span>"; otherwise output "<span class="tex-font-style-tt">No</span>" (both without quotes).</p><p>You can print each character in any case (upper or lower).</p>





```input1
5 8
.#.#..#.
.....#..
.#.#..#.
#.#....#
.....#..

```




```input2
5 5
..#..
..#..
#####
..#..
..#..

```




```input3
5 9
........#
#........
..##.#...
.......#.
....#.#.#

```




```output1
Yes

```




```output2
No

```




```output3
No

```



## Note

<p>For the first example, the desired setup can be produced by <span class="tex-span">3</span> operations, as is shown below.</p><center> <img class="tex-graphics" src="file://QclzjjrF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the second example, the desired setup cannot be produced, since in order to colour the center row, the third row and all columns must be selected in one operation, but after that no column can be selected again, hence it won't be possible to colour the other cells in the center column.</p>
