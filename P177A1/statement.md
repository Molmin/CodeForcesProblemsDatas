## Description

<div><p>The Smart Beaver from ABBYY got hooked on square matrices. Now he is busy studying an <span class="tex-span"><i>n</i> × <i>n</i></span> size matrix, where <span class="tex-span"><i>n</i></span> is odd. The Smart Beaver considers the following matrix elements good:  </p><ul> <li> Elements of the main diagonal.  </li><li> Elements of the secondary diagonal.  </li><li> Elements of the "middle" row — the row which has exactly <img align="middle" class="tex-formula" src="file://VtL5bvpY.png" style="max-width: 100.0%;max-height: 100.0%;"> rows above it and the same number of rows below it.  </li><li> Elements of the "middle" column — the column that has exactly <img align="middle" class="tex-formula" src="file://m5wIG4RB.png" style="max-width: 100.0%;max-height: 100.0%;"> columns to the left of it and the same number of columns to the right of it. </li></ul><center> <img class="tex-graphics" src="file://emJE0Fm3.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> The figure shows a <span class="tex-span">5 × 5</span> matrix.   The good elements are marked with green. </span> </center><p>Help the Smart Beaver count the sum of good elements of the given matrix.</p></div><div class="input-specification"><p>The first line of input data contains a single odd integer <span class="tex-span"><i>n</i></span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 100)</span> separated by single spaces — the elements of the given matrix.</p><p>The input limitations for getting 30 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 5</span> </li></ul><p>The input limitations for getting 100 points are:</p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 101</span> </li></ul></div><div class="output-specification"><p>Print a single integer — the sum of good matrix elements.</p></div>

## Input

<p>The first line of input data contains a single odd integer <span class="tex-span"><i>n</i></span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 100)</span> separated by single spaces — the elements of the given matrix.</p><p>The input limitations for getting 30 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 5</span> </li></ul><p>The input limitations for getting 100 points are:</p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 101</span> </li></ul>

## Output

<p>Print a single integer — the sum of good matrix elements.</p>





```input1
3
1 2 3
4 5 6
7 8 9

```




```input2
5
1 1 1 1 1
1 1 1 1 1
1 1 1 1 1
1 1 1 1 1
1 1 1 1 1

```




```output1
45

```




```output2
17

```



## Note

<p>In the first sample all matrix elements will be good. Good elements in the second sample are shown on the figure.</p>
