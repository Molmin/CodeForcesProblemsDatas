## Description

<div><p>Harry Potter has a difficult homework. Given a rectangular table, consisting of <span class="tex-span"><i>n</i> × <i>m</i></span> cells. Each cell of the table contains the integer. Harry knows how to use two spells: the first spell change the sign of the integers in the selected row, the second — in the selected column. Harry's task is to make non-negative the sum of the numbers in each row and each column using these spells.</p><p>Alone, the boy can not cope. Help the young magician!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, &nbsp;<i>m</i> ≤ 100)</span> — the number of rows and the number of columns. </p><p>Next <span class="tex-span"><i>n</i></span> lines follow, each contains <span class="tex-span"><i>m</i></span> integers: <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub>| ≤ 100)</span>, the number in the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column of the table.</p><p>The rows of the table numbered from 1 to <span class="tex-span"><i>n</i></span>. The columns of the table numbered from 1 to <span class="tex-span"><i>m</i></span>.</p></div><div class="output-specification"><p>In the first line print the number <span class="tex-span"><i>a</i></span> — the number of required applications of the first spell. Next print <span class="tex-span"><i>a</i></span> space-separated integers — the row numbers, you want to apply a spell. These row numbers must be distinct!</p><p>In the second line print the number <span class="tex-span"><i>b</i></span> — the number of required applications of the second spell. Next print <span class="tex-span"><i>b</i></span> space-separated integers — the column numbers, you want to apply a spell. These column numbers must be distinct!</p><p>If there are several solutions are allowed to print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, &nbsp;<i>m</i> ≤ 100)</span> — the number of rows and the number of columns. </p><p>Next <span class="tex-span"><i>n</i></span> lines follow, each contains <span class="tex-span"><i>m</i></span> integers: <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th line is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> <span class="tex-span">(|<i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub>| ≤ 100)</span>, the number in the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column of the table.</p><p>The rows of the table numbered from 1 to <span class="tex-span"><i>n</i></span>. The columns of the table numbered from 1 to <span class="tex-span"><i>m</i></span>.</p>

## Output

<p>In the first line print the number <span class="tex-span"><i>a</i></span> — the number of required applications of the first spell. Next print <span class="tex-span"><i>a</i></span> space-separated integers — the row numbers, you want to apply a spell. These row numbers must be distinct!</p><p>In the second line print the number <span class="tex-span"><i>b</i></span> — the number of required applications of the second spell. Next print <span class="tex-span"><i>b</i></span> space-separated integers — the column numbers, you want to apply a spell. These column numbers must be distinct!</p><p>If there are several solutions are allowed to print any of them.</p>





```input1
4 1
-1
-1
-1
-1

```




```input2
2 4
-1 -1 -1 2
1 1 1 1

```




```output1
4 1 2 3 4 
0 

```




```output2
1 1 
1 4 

```


