## Description

<div><p><span class="tex-font-style-it">The problem statement looms below, filling you with determination.</span></p><p>Consider a grid in which some cells are empty and some cells are filled. Call a cell in this grid <span class="tex-font-style-bf">exitable</span> if, starting at that cell, you can exit the grid by moving up and left through only empty cells. This includes the cell itself, so all filled in cells are not exitable. Note that you can exit the grid from any leftmost empty cell (cell in the first column) by going left, and from any topmost empty cell (cell in the first row) by going up.</p><p>Let's call a grid <span class="tex-font-style-bf">determinable</span> if, given only which cells are exitable, we can exactly determine which cells are filled in and which aren't.</p><p>You are given a grid $a$ of dimensions $n \times m$ , i. e. a grid with $n$ rows and $m$ columns. You need to answer $q$ queries ($1 \leq q \leq 2 \cdot 10^5$). Each query gives two integers $x_1, x_2$ ($1 \leq x_1 \leq x_2 \leq m$) and asks whether the subgrid of $a$ consisting of the columns $x_1, x_1 + 1, \ldots, x_2 - 1, x_2$ is determinable.</p></div><div class="input-specification"><p>The first line contains two integers $n, m$ ($1 \leq n, m \leq 10^6$, $nm \leq 10^6$) &nbsp;— the dimensions of the grid $a$.</p><p>$n$ lines follow. The $y$-th line contains $m$ characters, the $x$-th of which is '<span class="tex-font-style-tt">X</span>' if the cell on the intersection of the the $y$-th row and $x$-th column is filled and "<span class="tex-font-style-tt">.</span>" if it is empty.</p><p>The next line contains a single integer $q$ ($1 \leq q \leq 2 \cdot 10^5$) &nbsp;— the number of queries.</p><p>$q$ lines follow. Each line contains two integers $x_1$ and $x_2$ ($1 \leq x_1 \leq x_2 \leq m$), representing a query asking whether the subgrid of $a$ containing the columns $x_1, x_1 + 1, \ldots, x_2 - 1, x_2$ is determinable.</p></div><div class="output-specification"><p>For each query, output one line containing "<span class="tex-font-style-tt">YES</span>" if the subgrid specified by the query is determinable and "<span class="tex-font-style-tt">NO</span>" otherwise. The output is case insensitive (so "<span class="tex-font-style-tt">yEs</span>" and "<span class="tex-font-style-tt">No</span>" will also be accepted).</p></div>

## Input

<p>The first line contains two integers $n, m$ ($1 \leq n, m \leq 10^6$, $nm \leq 10^6$) &nbsp;— the dimensions of the grid $a$.</p><p>$n$ lines follow. The $y$-th line contains $m$ characters, the $x$-th of which is '<span class="tex-font-style-tt">X</span>' if the cell on the intersection of the the $y$-th row and $x$-th column is filled and "<span class="tex-font-style-tt">.</span>" if it is empty.</p><p>The next line contains a single integer $q$ ($1 \leq q \leq 2 \cdot 10^5$) &nbsp;— the number of queries.</p><p>$q$ lines follow. Each line contains two integers $x_1$ and $x_2$ ($1 \leq x_1 \leq x_2 \leq m$), representing a query asking whether the subgrid of $a$ containing the columns $x_1, x_1 + 1, \ldots, x_2 - 1, x_2$ is determinable.</p>

## Output

<p>For each query, output one line containing "<span class="tex-font-style-tt">YES</span>" if the subgrid specified by the query is determinable and "<span class="tex-font-style-tt">NO</span>" otherwise. The output is case insensitive (so "<span class="tex-font-style-tt">yEs</span>" and "<span class="tex-font-style-tt">No</span>" will also be accepted).</p>





```input1
4 5
..XXX
...X.
...X.
...X.
5
1 3
3 3
4 5
5 5
1 5
```




```output1
YES
YES
NO
YES
NO
```



## Note

<p>For each query of the example, the corresponding subgrid is displayed twice below: first in its input format, then with each cell marked as "<span class="tex-font-style-tt">E</span>" if it is exitable and "<span class="tex-font-style-tt">N</span>" otherwise.</p><p>For the first query: </p><pre class="verbatim"><br>..X EEN<br>... EEE<br>... EEE<br>... EEE<br></pre><pre class="verbatim"><br><br></pre><p>For the second query: </p><pre class="verbatim"><br>X N<br>. E<br>. E<br>. E<br></pre><p>Note that you can exit the grid by going left from any leftmost cell (or up from any topmost cell); you do not need to reach the top left corner cell to exit the grid.</p><pre class="verbatim"><br><br></pre><p>For the third query: </p><pre class="verbatim"><br>XX NN<br>X. NN<br>X. NN<br>X. NN<br></pre><p>This subgrid cannot be determined only from whether each cell is exitable, because the below grid produces the above "exitability grid" as well: </p><pre class="verbatim"><br>XX<br>XX<br>XX<br>XX<br></pre><pre class="verbatim"><br><br></pre><p>For the fourth query: </p><pre class="verbatim"><br>X N<br>. E<br>. E<br>. E<br></pre><pre class="verbatim"><br><br></pre><p>For the fifth query: </p><pre class="verbatim"><br>..XXX EENNN<br>...X. EEENN<br>...X. EEENN<br>...X. EEENN<br></pre><p>This query is simply the entire grid. It cannot be determined only from whether each cell is exitable because the below grid produces the above "exitability grid" as well: </p><pre class="verbatim"><br>..XXX<br>...XX<br>...XX<br>...XX<br></pre>
