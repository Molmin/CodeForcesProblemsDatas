## Description

<div><p>An <span class="tex-span"><i>n</i> × <i>n</i></span> table <span class="tex-span"><i>a</i></span> is defined as follows:</p><ul> <li> The first row and the first column contain ones, that is: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, 1</sub> = <i>a</i><sub class="lower-index">1, <i>i</i></sub> = 1</span> for all <span class="tex-span"><i>i</i> = 1, 2, ..., <i>n</i></span>. </li><li> Each of the remaining numbers in the table is equal to the sum of the number above it and the number to the left of it. In other words, the remaining elements are defined by the formula <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>a</i><sub class="lower-index"><i>i</i> - 1, <i>j</i></sub> + <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i> - 1</sub></span>. </li></ul><p>These conditions define all the values in the table.</p><p>You are given a number <span class="tex-span"><i>n</i></span>. You need to determine the maximum value in the <span class="tex-span"><i>n</i> × <i>n</i></span> table defined by the rules above.</p></div><div class="input-specification"><p>The only line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>) — the number of rows and columns of the table.</p></div><div class="output-specification"><p>Print a single line containing a positive integer <span class="tex-span"><i>m</i></span> — the maximum value in the table.</p></div>

## Input

<p>The only line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>) — the number of rows and columns of the table.</p>

## Output

<p>Print a single line containing a positive integer <span class="tex-span"><i>m</i></span> — the maximum value in the table.</p>





```input1
1

```




```input2
5

```




```output1
1
```




```output2
70
```



## Note

<p>In the second test the rows of the table look as follows: </p><center class="tex-equation"><span class="tex-span">{1, 1, 1, 1, 1}, </span></center> <center class="tex-equation"><span class="tex-span">{1, 2, 3, 4, 5}, </span></center> <center class="tex-equation"><span class="tex-span">{1, 3, 6, 10, 15}, </span></center> <center class="tex-equation"><span class="tex-span">{1, 4, 10, 20, 35}, </span></center> <center class="tex-equation"><span class="tex-span">{1, 5, 15, 35, 70}.</span></center>
