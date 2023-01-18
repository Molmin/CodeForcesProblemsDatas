## Description

<div><p>Ivan is playing a strange game.</p><p>He has a matrix <span class="tex-span"><i>a</i></span> with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Each element of the matrix is equal to either <span class="tex-span">0</span> or <span class="tex-span">1</span>. Rows and columns are <span class="tex-span">1</span>-indexed. Ivan can replace any number of ones in this matrix with zeroes. After that, his score in the game will be calculated as follows:</p><ol> <li> Initially Ivan's score is <span class="tex-span">0</span>; </li><li> In each column, Ivan will find the topmost <span class="tex-span">1</span> (that is, if the current column is <span class="tex-span"><i>j</i></span>, then he will find minimum <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 1</span>). If there are no <span class="tex-span">1</span>'s in the column, this column is skipped; </li><li> Ivan will look at the next <span class="tex-span"><i>min</i>(<i>k</i>, <i>n</i> - <i>i</i> + 1)</span> elements in this column (starting from the element he found) and count the number of <span class="tex-span">1</span>'s among these elements. This number will be added to his score. </li></ol><p>Of course, Ivan wants to maximize his score in this strange game. Also he doesn't want to change many elements, so he will replace the minimum possible number of ones with zeroes. Help him to determine the maximum possible score he can get and the minimum possible number of replacements required to achieve that score.</p></div><div class="input-specification"><p>The first line contains three integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>).</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th of them contains <span class="tex-span"><i>m</i></span> integer numbers — the elements of <span class="tex-span"><i>i</i></span>-th row of matrix <span class="tex-span"><i>a</i></span>. Each number is either <span class="tex-span">0</span> or <span class="tex-span">1</span>.</p></div><div class="output-specification"><p>Print two numbers: the maximum possible score Ivan can get and the minimum number of replacements required to get this score.</p></div>

## Input

<p>The first line contains three integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>).</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th of them contains <span class="tex-span"><i>m</i></span> integer numbers — the elements of <span class="tex-span"><i>i</i></span>-th row of matrix <span class="tex-span"><i>a</i></span>. Each number is either <span class="tex-span">0</span> or <span class="tex-span">1</span>.</p>

## Output

<p>Print two numbers: the maximum possible score Ivan can get and the minimum number of replacements required to get this score.</p>





```input1
4 3 2
0 1 0
1 0 1
0 1 0
1 1 1

```




```input2
3 2 1
1 0
0 1
0 0

```




```output1
4 1

```




```output2
2 0

```



## Note

<p>In the first example Ivan will replace the element <span class="tex-span"><i>a</i><sub class="lower-index">1, 2</sub></span>.</p>
