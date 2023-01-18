## Description

<div><p>A big company decided to launch a new series of rectangular displays, and decided that the display must have exactly <span class="tex-span"><i>n</i></span> pixels. </p><p>Your task is to determine the size of the rectangular display — the number of lines (rows) of pixels <span class="tex-span"><i>a</i></span> and the number of columns of pixels <span class="tex-span"><i>b</i></span>, so that:</p><ul> <li> there are exactly <span class="tex-span"><i>n</i></span> pixels on the display; </li><li> the number of rows does not exceed the number of columns, it means <span class="tex-span"><i>a</i> ≤ <i>b</i></span>; </li><li> the difference <span class="tex-span"><i>b</i> - <i>a</i></span> is as small as possible. </li></ul></div><div class="input-specification"><p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of pixels display should have.</p></div><div class="output-specification"><p>Print two integers&nbsp;— the number of rows and columns on the display. </p></div>

## Input

<p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of pixels display should have.</p>

## Output

<p>Print two integers&nbsp;— the number of rows and columns on the display. </p>





```input1
8

```




```input2
64

```




```input3
5

```




```input4
999999

```




```output1
2 4

```




```output2
8 8

```




```output3
1 5

```




```output4
999 1001

```



## Note

<p>In the first example the minimum possible difference equals 2, so on the display should be 2 rows of 4 pixels.</p><p>In the second example the minimum possible difference equals 0, so on the display should be 8 rows of 8 pixels.</p><p>In the third example the minimum possible difference equals 4, so on the display should be 1 row of 5 pixels.</p>
