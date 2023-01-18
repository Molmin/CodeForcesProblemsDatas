## Description

<div><p>Gildong has bought a famous painting software <span class="tex-font-style-it">cfpaint</span>. The working screen of cfpaint is square-shaped consisting of $n$ rows and $n$ columns of square cells. The rows are numbered from $1$ to $n$, from top to bottom, and the columns are numbered from $1$ to $n$, from left to right. The position of a cell at row $r$ and column $c$ is represented as $(r, c)$. There are only two colors for the cells in cfpaint — black and white.</p><p>There is a tool named <span class="tex-font-style-it">eraser</span> in cfpaint. The eraser has an integer size $k$ ($1 \le k \le n$). To use the eraser, Gildong needs to click on a cell $(i, j)$ where $1 \le i, j \le n - k + 1$. When a cell $(i, j)$ is clicked, all of the cells $(i', j')$ where $i \le i' \le i + k - 1$ and $j \le j' \le j + k - 1$ become white. In other words, a square with side equal to $k$ cells and top left corner at $(i, j)$ is colored white.</p><p>A <span class="tex-font-style-it">white line</span> is a row or a column without any black cells.</p><p>Gildong has worked with cfpaint for some time, so some of the cells (possibly zero or all) are currently black. He wants to know the maximum number of <span class="tex-font-style-it">white lines</span> after using the eraser <span class="tex-font-style-bf">exactly once</span>. Help Gildong find the answer to his question.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 2000$) — the number of rows and columns, and the size of the eraser.</p><p>The next $n$ lines contain $n$ characters each without spaces. The $j$-th character in the $i$-th line represents the cell at $(i,j)$. Each character is given as either '<span class="tex-font-style-tt">B</span>' representing a black cell, or '<span class="tex-font-style-tt">W</span>' representing a white cell.</p></div><div class="output-specification"><p>Print one integer: the maximum number of white lines after using the eraser exactly once.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 2000$) — the number of rows and columns, and the size of the eraser.</p><p>The next $n$ lines contain $n$ characters each without spaces. The $j$-th character in the $i$-th line represents the cell at $(i,j)$. Each character is given as either '<span class="tex-font-style-tt">B</span>' representing a black cell, or '<span class="tex-font-style-tt">W</span>' representing a white cell.</p>

## Output

<p>Print one integer: the maximum number of white lines after using the eraser exactly once.</p>





```input1
4 2
BWWW
WBBW
WBBW
WWWB
```




```input2
3 1
BWB
WWB
BWB
```




```input3
5 3
BWBBB
BWBBB
BBBBB
BBBBB
WBBBW
```




```input4
2 2
BW
WB
```




```input5
2 1
WW
WW
```




```output1
4
```




```output2
2
```




```output3
2
```




```output4
4
```




```output5
4
```



## Note

<p>In the first example, Gildong can click the cell $(2, 2)$, then the working screen becomes: </p><pre class="verbatim">BWWW<br>WWWW<br>WWWW<br>WWWB<br></pre><p>Then there are four white lines — the $2$-nd and $3$-rd row, and the $2$-nd and $3$-rd column.</p><p>In the second example, clicking the cell $(2, 3)$ makes the $2$-nd row a white line.</p><p>In the third example, both the $2$-nd column and $5$-th row become white lines by clicking the cell $(3, 2)$.</p>
