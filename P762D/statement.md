## Description

<div><p>You are given a rectangular table <span class="tex-span">3 × <i>n</i></span>. Each cell contains an integer. You can move from one cell to another if they share a side.</p><p>Find such path from the upper left cell to the bottom right cell of the table that doesn't visit any of the cells twice, and the sum of numbers written in the cells of this path is maximum possible.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) &nbsp;— the number of columns in the table.</p><p>Next three lines contain <span class="tex-span"><i>n</i></span> integers each &nbsp;— the description of the table. The <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th line corresponds to the cell <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) of the table.</p></div><div class="output-specification"><p>Output the maximum sum of numbers on a path from the upper left cell to the bottom right cell of the table, that doesn't visit any of the cells twice.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) &nbsp;— the number of columns in the table.</p><p>Next three lines contain <span class="tex-span"><i>n</i></span> integers each &nbsp;— the description of the table. The <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th line corresponds to the cell <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) of the table.</p>

## Output

<p>Output the maximum sum of numbers on a path from the upper left cell to the bottom right cell of the table, that doesn't visit any of the cells twice.</p>





```input1
3
1 1 1
1 -1 1
1 1 1

```




```input2
5
10 10 10 -1 -1
-1 10 10 10 10
-1 10 10 10 10

```




```output1
7

```




```output2
110

```



## Note

<p>The path for the first example:</p><center> <img class="tex-graphics" src="file://lvpJWTwe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The path for the second example:</p><center> <img class="tex-graphics" src="file://ClCX6UNb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
