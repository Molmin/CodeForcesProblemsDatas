## Description

<div><p>Limak has a grid that consists of <span class="tex-span">2</span> rows and <span class="tex-span"><i>n</i></span> columns. The <span class="tex-span"><i>j</i></span>-th cell in the <span class="tex-span"><i>i</i></span>-th row contains an integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> which can be positive, negative or zero.</p><p>A non-empty rectangle of cells is called <span class="tex-font-style-it">nice</span> if and only if the sum of numbers in its cells is equal to <span class="tex-span">0</span>.</p><p>Limak wants to choose some nice rectangles and give them to his friends, as gifts. No two chosen rectangles should share a cell. What is the maximum possible number of nice rectangles Limak can choose?</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>)&nbsp;— the number of columns in the grid.</p><p>The next two lines contain numbers in the grid. The <span class="tex-span"><i>i</i></span>-th of those two lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>t</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>t</i><sub class="lower-index"><i>i</i>, <i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>t</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print one integer, denoting the maximum possible number of cell-disjoint nice rectangles.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>)&nbsp;— the number of columns in the grid.</p><p>The next two lines contain numbers in the grid. The <span class="tex-span"><i>i</i></span>-th of those two lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>t</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>t</i><sub class="lower-index"><i>i</i>, <i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>t</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print one integer, denoting the maximum possible number of cell-disjoint nice rectangles.</p>





```input1
6
70 70 70 70 70 -15
90 -60 -30 30 -30 15

```




```input2
4
0 -1 0 0
0 0 1 0

```




```input3
3
1000000000 999999999 -1000000000
999999999 -1000000000 -999999998

```




```output1
3

```




```output2
6

```




```output3
1

```



## Note

<p>In the first sample, there are four nice rectangles:</p><center> <img class="tex-graphics" src="file://vUbbA3kK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Limak can't choose all of them because they are not disjoint. He should take three nice rectangles: those denoted as blue frames on the drawings.</p><p>In the second sample, it's optimal to choose six nice rectangles, each consisting of one cell with a number <span class="tex-span">0</span>.</p><p>In the third sample, the only nice rectangle is the whole grid&nbsp;— the sum of all numbers is <span class="tex-span">0</span>. Clearly, Limak can choose at most one nice rectangle, so the answer is <span class="tex-span">1</span>.</p>
