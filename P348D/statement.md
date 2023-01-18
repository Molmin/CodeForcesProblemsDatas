## Description

<div><p>You've got a table of size <span class="tex-span"><i>n</i> × <i>m</i></span>. We'll consider the table rows numbered from top to bottom 1 through <span class="tex-span"><i>n</i></span>, and the columns numbered from left to right 1 through <span class="tex-span"><i>m</i></span>. Then we'll denote the cell in row <span class="tex-span"><i>x</i></span> and column <span class="tex-span"><i>y</i></span> as <span class="tex-span">(<i>x</i>, <i>y</i>)</span>.</p><p>Initially cell <span class="tex-span">(1, 1)</span> contains two similar turtles. Both turtles want to get to cell <span class="tex-span">(<i>n</i>, <i>m</i>)</span>. Some cells of the table have obstacles but it is guaranteed that there aren't any obstacles in the upper left and lower right corner. A turtle (one or the other) can go from cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to one of two cells <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span> and <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span>, as long as the required cell doesn't contain an obstacle. The turtles have had an argument so they don't want to have any chance of meeting each other along the way. Help them find the number of ways in which they can go from cell <span class="tex-span">(1, 1)</span> to cell <span class="tex-span">(<i>n</i>, <i>m</i>)</span>.</p><p>More formally, find the number of pairs of non-intersecting ways from cell <span class="tex-span">(1, 1)</span> to cell <span class="tex-span">(<i>n</i>, <i>m</i>)</span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. Two ways are called non-intersecting if they have exactly two common points — the starting point and the final point.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 3000)</span>. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters describing the table. The empty cells are marked by characters "<span class="tex-font-style-tt">.</span>", the cells with obstacles are marked by "<span class="tex-font-style-tt">#</span>".</p><p>It is guaranteed that the upper left and the lower right cells are empty.</p></div><div class="output-specification"><p>In a single line print a single integer — the number of pairs of non-intersecting paths from cell <span class="tex-span">(1, 1)</span> to cell <span class="tex-span">(<i>n</i>, <i>m</i>)</span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i>, <i>m</i> ≤ 3000)</span>. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters describing the table. The empty cells are marked by characters "<span class="tex-font-style-tt">.</span>", the cells with obstacles are marked by "<span class="tex-font-style-tt">#</span>".</p><p>It is guaranteed that the upper left and the lower right cells are empty.</p>

## Output

<p>In a single line print a single integer — the number of pairs of non-intersecting paths from cell <span class="tex-span">(1, 1)</span> to cell <span class="tex-span">(<i>n</i>, <i>m</i>)</span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
4 5
.....
.###.
.###.
.....

```




```input2
2 3
...
...

```




```output1
1

```




```output2
1

```


