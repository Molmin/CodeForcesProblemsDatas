## Description

<div><p>Consider some square matrix <span class="tex-span"><i>A</i></span> with side <span class="tex-span"><i>n</i></span> consisting of zeros and ones. There are <span class="tex-span"><i>n</i></span> rows numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom and <span class="tex-span"><i>n</i></span> columns numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right in this matrix. We'll denote the element of the matrix which is located at the intersection of the <span class="tex-span"><i>i</i></span>-row and the <span class="tex-span"><i>j</i></span>-th column as <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>.</p><p>Let's call matrix <span class="tex-span"><i>A</i></span> <span class="tex-font-style-underline">clear</span> if no two cells containing ones have a common side.</p><p>Let's call matrix <span class="tex-span"><i>A</i></span> <span class="tex-font-style-underline">symmetrical</span> if it matches the matrices formed from it by a horizontal and/or a vertical reflection. Formally, for each pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> <span class="tex-span">(1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i>)</span> both of the following conditions must be met: <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>A</i><sub class="lower-index"><i>n</i> - <i>i</i> + 1, <i>j</i></sub></span> and <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>A</i><sub class="lower-index"><i>i</i>, <i>n</i> - <i>j</i> + 1</sub></span>.</p><p>Let's define the <span class="tex-font-style-underline">sharpness</span> of matrix <span class="tex-span"><i>A</i></span> as the number of ones in it.</p><p>Given integer <span class="tex-span"><i>x</i></span>, your task is to find the smallest positive integer <span class="tex-span"><i>n</i></span> such that there exists a clear symmetrical matrix <span class="tex-span"><i>A</i></span> with side <span class="tex-span"><i>n</i></span> and sharpness <span class="tex-span"><i>x</i></span>.</p></div><div class="input-specification"><p>The only line contains a single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 100</span>) — the required sharpness of the matrix.</p></div><div class="output-specification"><p>Print a single number — the sought value of <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The only line contains a single integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 100</span>) — the required sharpness of the matrix.</p>

## Output

<p>Print a single number — the sought value of <span class="tex-span"><i>n</i></span>.</p>





```input1
4

```




```input2
9

```




```output1
3

```




```output2
5

```



## Note

<p>The figure below shows the matrices that correspond to the samples:</p><center> <img class="tex-graphics" src="file://R6vzEg4x.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
