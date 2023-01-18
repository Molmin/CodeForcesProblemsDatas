## Description

<div><p>You've got an <span class="tex-span"><i>n</i> × <i>m</i></span> table (<span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns), each cell of the table contains a "0" or a "1".</p><p>Your task is to calculate the number of rectangles with the sides that are parallel to the sides of the table and go along the cell borders, such that the number one occurs exactly <span class="tex-span"><i>k</i></span> times in the rectangle. </p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2500</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 6</span>) — the sizes of the table and the required number of numbers one.</p><p>Next <span class="tex-span"><i>n</i></span> lines each contains <span class="tex-span"><i>m</i></span> characters "0" or "1". The <span class="tex-span"><i>i</i></span>-th character of the <span class="tex-span"><i>j</i></span>-th line corresponds to the character that is in the <span class="tex-span"><i>j</i></span>-th row and the <span class="tex-span"><i>i</i></span>-th column of the table.</p></div><div class="output-specification"><p>Print a single number — the number of rectangles that contain exactly <span class="tex-span"><i>k</i></span> numbers one.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2500</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 6</span>) — the sizes of the table and the required number of numbers one.</p><p>Next <span class="tex-span"><i>n</i></span> lines each contains <span class="tex-span"><i>m</i></span> characters "0" or "1". The <span class="tex-span"><i>i</i></span>-th character of the <span class="tex-span"><i>j</i></span>-th line corresponds to the character that is in the <span class="tex-span"><i>j</i></span>-th row and the <span class="tex-span"><i>i</i></span>-th column of the table.</p>

## Output

<p>Print a single number — the number of rectangles that contain exactly <span class="tex-span"><i>k</i></span> numbers one.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3 3 2
101
000
101

```




```input2
5 5 1
00000
00000
00100
00000
00000

```




```input3
5 5 6
01010
10101
01010
10101
01010

```




```input4
3 3 0
001
010
000

```




```input5
4 4 0
0000
0101
0000
0000

```




```output1
8

```




```output2
81

```




```output3
12

```




```output4
15

```




```output5
52

```


