## Description

<div><p>Consider a square grid with $h$ rows and $w$ columns with some dominoes on it. Each domino covers exactly two cells of the grid that share a common side. Every cell is covered by at most one domino.</p><p>Let's call a placement of dominoes on the grid <span class="tex-font-style-it">perfectly balanced</span> if no row and no column contains a pair of cells covered by two different dominoes. In other words, every row and column may contain no covered cells, one covered cell, or two covered cells that belong to the same domino.</p><p>You are given a perfectly balanced placement of dominoes on a grid. Find the number of ways to place zero or more extra dominoes on this grid to keep the placement perfectly balanced. Output this number modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains three integers $h$, $w$, and $n$ ($1 \le h, w \le 3600$; $0 \le n \le 2400$), denoting the dimensions of the grid and the number of already placed dominoes. The rows are numbered from $1$ to $h$, and the columns are numbered from $1$ to $w$.</p><p>Each of the next $n$ lines contains four integers $r_{i, 1}, c_{i, 1}, r_{i, 2}, c_{i, 2}$ ($1 \le r_{i, 1} \le r_{i, 2} \le h$; $1 \le c_{i, 1} \le c_{i, 2} \le w$), denoting the row id and the column id of the cells covered by the $i$-th domino. Cells $(r_{i, 1}, c_{i, 1})$ and $(r_{i, 2}, c_{i, 2})$ are distinct and share a common side.</p><p>The given domino placement is perfectly balanced.</p></div><div class="output-specification"><p>Output the number of ways to place zero or more extra dominoes on the grid to keep the placement perfectly balanced, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains three integers $h$, $w$, and $n$ ($1 \le h, w \le 3600$; $0 \le n \le 2400$), denoting the dimensions of the grid and the number of already placed dominoes. The rows are numbered from $1$ to $h$, and the columns are numbered from $1$ to $w$.</p><p>Each of the next $n$ lines contains four integers $r_{i, 1}, c_{i, 1}, r_{i, 2}, c_{i, 2}$ ($1 \le r_{i, 1} \le r_{i, 2} \le h$; $1 \le c_{i, 1} \le c_{i, 2} \le w$), denoting the row id and the column id of the cells covered by the $i$-th domino. Cells $(r_{i, 1}, c_{i, 1})$ and $(r_{i, 2}, c_{i, 2})$ are distinct and share a common side.</p><p>The given domino placement is perfectly balanced.</p>

## Output

<p>Output the number of ways to place zero or more extra dominoes on the grid to keep the placement perfectly balanced, modulo $998\,244\,353$.</p>





```input1
5 7 2
3 1 3 2
4 4 4 5
```




```input2
5 4 2
1 2 2 2
4 3 4 4
```




```input3
23 42 0
```




```output1
8
```




```output2
1
```




```output3
102848351
```



## Note

<p>In the first example, the initial grid looks like this:</p><p><img class="tex-graphics" src="file://Nm3u6rwQ.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Here are $8$ ways to place zero or more extra dominoes to keep the placement perfectly balanced:</p><p><img class="tex-graphics" src="file://fsokUBsu.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the second example, the initial grid looks like this:</p><p><img class="tex-graphics" src="file://peIUVyOM.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>No extra dominoes can be placed here.</p>
