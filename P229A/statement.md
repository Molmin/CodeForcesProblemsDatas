## Description

<div><p>You are given a table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Each cell of the table contains a number, 0 or 1. In one move we can choose some row of the table and cyclically shift its values either one cell to the left, or one cell to the right.</p><p>To <span class="tex-font-style-underline">cyclically shift</span> a table row one cell to the right means to move the value of each cell, except for the last one, to the right neighboring cell, and to move the value of the last cell to the first cell. A cyclical shift of a row to the left is performed similarly, but in the other direction. For example, if we cyclically shift a row "<span class="tex-font-style-tt">00110</span>" one cell to the right, we get a row "<span class="tex-font-style-tt">00011</span>", but if we shift a row "<span class="tex-font-style-tt">00110</span>" one cell to the left, we get a row "<span class="tex-font-style-tt">01100</span>".</p><p>Determine the minimum number of moves needed to make some table column consist only of numbers 1.</p></div><div class="input-specification"><p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of rows in the table and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— the number of columns in the table. Then <span class="tex-span"><i>n</i></span> lines follow, each of them contains <span class="tex-span"><i>m</i></span> characters "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>": the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line describes the contents of the cell in the <span class="tex-span"><i>i</i></span>-th row and in the <span class="tex-span"><i>j</i></span>-th column of the table.</p><p>It is guaranteed that the description of the table contains no other characters besides "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>".</p></div><div class="output-specification"><p>Print a single number: the minimum number of moves needed to get only numbers 1 in some column of the table. If this is impossible, print -1.</p></div>

## Input

<p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of rows in the table and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— the number of columns in the table. Then <span class="tex-span"><i>n</i></span> lines follow, each of them contains <span class="tex-span"><i>m</i></span> characters "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>": the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line describes the contents of the cell in the <span class="tex-span"><i>i</i></span>-th row and in the <span class="tex-span"><i>j</i></span>-th column of the table.</p><p>It is guaranteed that the description of the table contains no other characters besides "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>".</p>

## Output

<p>Print a single number: the minimum number of moves needed to get only numbers 1 in some column of the table. If this is impossible, print -1.</p>





```input1
3 6
101010
000100
100000

```




```input2
2 3
111
000

```




```output1
3

```




```output2
-1

```



## Note

<p>In the first sample one way to achieve the goal with the least number of moves is as follows: cyclically shift the second row to the right once, then shift the third row to the left twice. Then the table column before the last one will contain only 1s.</p><p>In the second sample one can't shift the rows to get a column containing only 1s.</p>
