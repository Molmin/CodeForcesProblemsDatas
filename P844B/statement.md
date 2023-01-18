## Description

<div><p>You are given <span class="tex-span"><i>n</i> × <i>m</i></span> table. Each cell of the table is colored white or black. Find the number of non-empty sets of cells such that:</p><ol> <li> All cells in a set have the same color. </li><li> Every two cells in a set share row or column. </li></ol></div><div class="input-specification"><p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>)&nbsp;— the number of rows and the number of columns correspondingly.</p><p>The next <span class="tex-span"><i>n</i></span> lines of input contain descriptions of rows. There are <span class="tex-span"><i>m</i></span> integers, separated by spaces, in each line. The number equals <span class="tex-span">0</span> if the corresponding cell is colored white and equals <span class="tex-span">1</span> if the corresponding cell is colored black.</p></div><div class="output-specification"><p>Output single integer &nbsp;— the number of non-empty sets from the problem description.</p></div>

## Input

<p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>)&nbsp;— the number of rows and the number of columns correspondingly.</p><p>The next <span class="tex-span"><i>n</i></span> lines of input contain descriptions of rows. There are <span class="tex-span"><i>m</i></span> integers, separated by spaces, in each line. The number equals <span class="tex-span">0</span> if the corresponding cell is colored white and equals <span class="tex-span">1</span> if the corresponding cell is colored black.</p>

## Output

<p>Output single integer &nbsp;— the number of non-empty sets from the problem description.</p>





```input1
1 1
0

```




```input2
2 3
1 0 1
0 1 0

```




```output1
1

```




```output2
8

```



## Note

<p>In the second example, there are six one-element sets. Additionally, there are two two-element sets, the first one consists of the first and the third cells of the first row, the second one consists of the first and the third cells of the second row. To sum up, there are <span class="tex-span">8</span> sets.</p>
