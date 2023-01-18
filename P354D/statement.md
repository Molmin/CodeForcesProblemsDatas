## Description

<div><p>Vasya and Petya are using an interesting data storing structure: a pyramid.</p><p>The pyramid consists of <span class="tex-span"><i>n</i></span> rows, the <span class="tex-span"><i>i</i></span>-th row contains <span class="tex-span"><i>i</i></span> cells. Each row is shifted half a cell to the left relative to the previous row. The cells are numbered by integers from 1 to <img align="middle" class="tex-formula" src="file://1hYV3gk7.png" style="max-width: 100.0%;max-height: 100.0%;"> as shown on the picture below.</p><p>An example of a pyramid at <span class="tex-span"><i>n</i> = 5</span> is: </p><center> <img class="tex-graphics" src="file://vMj8S8mG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>This data structure can perform operations of two types: </p><ol> <li> Change the value of a specific cell. It is described by three integers: <span class="tex-span">"<i>t</i> <i>i</i> <i>v</i>"</span>, where <span class="tex-span"><i>t</i> = 1</span> (the type of operation), <span class="tex-span"><i>i</i></span> — the number of the cell to change and <span class="tex-span"><i>v</i></span> the value to assign to the cell. </li><li> Change the value of some subpyramid. The picture shows a highlighted subpyramid with the top in cell <span class="tex-span">5</span>. It is described by <span class="tex-span"><i>s</i> + 2</span> numbers: <span class="tex-span">"<i>t</i> <i>i</i> <i>v</i><sub class="lower-index">1</sub> <i>v</i><sub class="lower-index">2</sub> ... <i>v</i><sub class="lower-index"><i>s</i></sub>"</span>, where <span class="tex-span"><i>t</i> = 2</span>, <span class="tex-span"><i>i</i></span> — the number of the top cell of the pyramid, <span class="tex-span"><i>s</i></span> — the size of the subpyramid (the number of cells it has), <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> — the value you should assign to the <span class="tex-span"><i>j</i></span>-th cell of the subpyramid. </li></ol><p>Formally: a subpyramid with top at the <span class="tex-span"><i>i</i></span>-th cell of the <span class="tex-span"><i>k</i></span>-th row (the <span class="tex-span">5</span>-th cell is the second cell of the third row) will contain cells from rows from <span class="tex-span"><i>k</i></span> to <span class="tex-span"><i>n</i></span>, the <span class="tex-span">(<i>k</i> + <i>p</i>)</span>-th row contains cells from the <span class="tex-span"><i>i</i></span>-th to the <span class="tex-span">(<i>i</i> + <i>p</i>)</span>-th (<span class="tex-span">0 ≤ <i>p</i> ≤ <i>n</i> - <i>k</i></span>).</p><p>Vasya and Petya had two identical pyramids. Vasya changed some cells in his pyramid and he now wants to send his changes to Petya. For that, he wants to find a sequence of operations at which Petya can repeat all Vasya's changes. Among all possible sequences, Vasya has to pick the minimum one (the one that contains the fewest numbers).</p><p>You have a pyramid of <span class="tex-span"><i>n</i></span> rows with <span class="tex-span"><i>k</i></span> changed cells. Find the sequence of operations which result in <span class="tex-font-style-bf">each of the <span class="tex-span"><i>k</i></span> changed cells being changed by at least one operation</span>. Among all the possible sequences pick <span class="tex-font-style-bf">the one that contains the fewest numbers</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>k</i></span> lines contain the coordinates of the modified cells <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the row and the cell's number in the row. All cells are distinct.</p></div><div class="output-specification"><p>Print a single number showing how many numbers the final sequence has.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>k</i></span> lines contain the coordinates of the modified cells <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the row and the cell's number in the row. All cells are distinct.</p>

## Output

<p>Print a single number showing how many numbers the final sequence has.</p>





```input1
4 5
3 1
3 3
4 1
4 3
4 4

```




```input2
7 11
2 2
3 1
4 3
5 1
5 2
5 5
6 4
7 2
7 3
7 4
7 5

```




```output1
10

```




```output2
26

```



## Note

<p>One of the possible solutions of the first sample consists of two operations:</p><p><span class="tex-span">2 4 <i>v</i><sub class="lower-index">4</sub> <i>v</i><sub class="lower-index">7</sub> <i>v</i><sub class="lower-index">8</sub></span></p><p><span class="tex-span">2 6 <i>v</i><sub class="lower-index">6</sub> <i>v</i><sub class="lower-index">9</sub> <i>v</i><sub class="lower-index">10</sub></span></p><p>The picture shows the changed cells color-highlighted. The subpyramid used by the first operation is highlighted blue and the subpyramid used by the first operation is highlighted yellow: </p><center> <img class="tex-graphics" src="file://9E20nvqW.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
