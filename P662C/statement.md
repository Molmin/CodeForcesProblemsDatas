## Description

<div><p>You are given a table consisting of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Each cell of the table contains either <span class="tex-span">0</span> or <span class="tex-span">1</span>. In one move, you are allowed to pick any row or any column and invert all values, that is, replace <span class="tex-span">0</span> by <span class="tex-span">1</span> and vice versa.</p><p>What is the minimum number of cells with value 1 you can get after applying some number of operations?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of rows and the number of columns, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follows with the descriptions of the rows. Each line has length <span class="tex-span"><i>m</i></span> and contains only digits '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the minimum possible number of ones you can get after applying some sequence of operations.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 20</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of rows and the number of columns, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follows with the descriptions of the rows. Each line has length <span class="tex-span"><i>m</i></span> and contains only digits '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'.</p>

## Output

<p>Output a single integer&nbsp;— the minimum possible number of ones you can get after applying some sequence of operations.</p>





```input1
3 4
0110
1010
0111

```




```output1
2

```


