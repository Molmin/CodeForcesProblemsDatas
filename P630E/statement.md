## Description

<div><p>Developing tools for creation of locations maps for turn-based fights in a new game, Petya faced the following problem.</p><p>A field map consists of hexagonal cells. Since locations sizes are going to be big, a game designer wants to have a tool for quick filling of a field part with identical enemy units. This action will look like following: a game designer will select a rectangular area on the map, and each cell whose center belongs to the selected rectangle will be filled with the enemy unit.</p><p>More formally, if a game designer selected cells having coordinates <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub></span>, then all cells having center coordinates <span class="tex-span">(<i>x</i>, <i>y</i>)</span> such that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i> ≤ <i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i> ≤ <i>y</i><sub class="lower-index">2</sub></span> will be filled. Orthogonal coordinates system is set up so that one of cell sides is parallel to <span class="tex-span"><i>OX</i></span> axis, all hexagon centers have integer coordinates and for each integer <span class="tex-span"><i>x</i></span> there are cells having center with such <span class="tex-span"><i>x</i></span> coordinate and for each integer <span class="tex-span"><i>y</i></span> there are cells having center with such <span class="tex-span"><i>y</i></span> coordinate. It is guaranteed that difference <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> - <i>x</i><sub class="lower-index">1</sub></span> is divisible by <span class="tex-span">2</span>.</p><p>Working on the problem Petya decided that before painting selected units he wants to output number of units that will be painted on the map.</p><p>Help him implement counting of these units before painting.</p><center> <img class="tex-graphics" src="file://ZnhB50iG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The only line of input contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup>,  - 10<sup class="upper-index">9</sup> ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the centers of two cells.</p></div><div class="output-specification"><p>Output one integer — the number of cells to be filled.</p></div>

## Input

<p>The only line of input contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup>,  - 10<sup class="upper-index">9</sup> ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the centers of two cells.</p>

## Output

<p>Output one integer — the number of cells to be filled.</p>





```input1
1 1 5 5

```




```output1
13
```


