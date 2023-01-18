## Description

<div><p>Greg has a pad. The pad's screen is an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangle, each cell can be either black or white. We'll consider the pad rows to be numbered with integers from 1 to <span class="tex-span"><i>n</i></span> from top to bottom. Similarly, the pad's columns are numbered with integers from 1 to <span class="tex-span"><i>m</i></span> from left to right.</p><p>Greg thinks that the pad's screen displays a cave if the following conditions hold:</p><ul> <li> There is a segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span>, such that each of the rows <span class="tex-span"><i>l</i>, <i>l</i> + 1, ..., <i>r</i></span> has exactly two black cells and all other rows have only white cells. </li><li> There is a row number <span class="tex-span"><i>t</i></span> <span class="tex-span">(<i>l</i> ≤ <i>t</i> ≤ <i>r</i>)</span>, such that for all pairs of rows with numbers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(<i>l</i> ≤ <i>i</i> ≤ <i>j</i> ≤ <i>t</i>)</span> the set of columns between the black cells in row <span class="tex-span"><i>i</i></span> <span class="tex-font-style-bf">(with the columns where is these black cells)</span> is the subset of the set of columns between the black cells in row <span class="tex-span"><i>j</i></span> <span class="tex-font-style-bf">(with the columns where is these black cells)</span>. Similarly, for all pairs of rows with numbers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> <span class="tex-span">(<i>t</i> ≤ <i>i</i> ≤ <i>j</i> ≤ <i>r</i>)</span> the set of columns between the black cells in row <span class="tex-span"><i>j</i></span> <span class="tex-font-style-bf">(with the columns where is these black cells)</span> is the subset of the set of columns between the black cells in row <span class="tex-span"><i>i</i></span> <span class="tex-font-style-bf">(with the columns where is these black cells)</span>. </li></ul><p>Greg wondered, how many ways there are to paint a cave on his pad. Two ways can be considered distinct if there is a cell that has distinct colors on the two pictures.</p><p>Help Greg.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> — the pad's screen size <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2000)</span>.</p></div><div class="output-specification"><p>In the single line print the remainder after dividing the answer to the problem by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> — the pad's screen size <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2000)</span>.</p>

## Output

<p>In the single line print the remainder after dividing the answer to the problem by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1 1

```




```input2
4 4

```




```input3
3 5

```




```output1
0

```




```output2
485

```




```output3
451

```


