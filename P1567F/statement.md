## Description

<div><p>Alice has an empty grid with $n$ rows and $m$ columns. Some of the cells are marked, and <span class="tex-font-style-bf">no marked cells are adjacent to the edge of the grid</span>. (Two squares are <span class="tex-font-style-it">adjacent</span> if they share a side.) </p><p>Alice wants to fill each cell with a number such that the following statements are true: </p><ul> <li> every <span class="tex-font-style-it">unmarked</span> cell contains either the number $1$ or $4$; </li><li> every <span class="tex-font-style-it">marked</span> cell contains the sum of the numbers in all <span class="tex-font-style-bf">unmarked</span> cells adjacent to it (if a marked cell is not adjacent to any unmarked cell, this sum is $0$); </li><li> every <span class="tex-font-style-it">marked</span> cell contains a multiple of $5$. </li></ul> Alice couldn't figure it out, so she asks Bob to help her. Help Bob find any such grid, or state that no such grid exists.</div><div class="input-specification"><p>The first line of input contains two integers $n$ and $m$ ($1 \leq n, m \leq 500$)&nbsp;— the number of rows and the number of columns in the grid, respectively.</p><p>Then $n$ lines follow, each containing $m$ characters. Each of these characters is either '<span class="tex-font-style-tt">.</span>' or '<span class="tex-font-style-tt">X</span>'&nbsp;— an unmarked and a marked cell, respectively. <span class="tex-font-style-bf">No marked cells are adjacent to the edge of the grid.</span></p></div><div class="output-specification"><p>Output "'<span class="tex-font-style-tt">NO</span>" if no suitable grid exists. Otherwise, output "'<span class="tex-font-style-tt">YES</span>"'. Then output $n$ lines of $m$ space-separated integers&nbsp;— the integers in the grid.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $m$ ($1 \leq n, m \leq 500$)&nbsp;— the number of rows and the number of columns in the grid, respectively.</p><p>Then $n$ lines follow, each containing $m$ characters. Each of these characters is either '<span class="tex-font-style-tt">.</span>' or '<span class="tex-font-style-tt">X</span>'&nbsp;— an unmarked and a marked cell, respectively. <span class="tex-font-style-bf">No marked cells are adjacent to the edge of the grid.</span></p>

## Output

<p>Output "'<span class="tex-font-style-tt">NO</span>" if no suitable grid exists. Otherwise, output "'<span class="tex-font-style-tt">YES</span>"'. Then output $n$ lines of $m$ space-separated integers&nbsp;— the integers in the grid.</p>





```input1
5 5
.....
.XXX.
.X.X.
.XXX.
.....
```




```input2
5 5
.....
.XXX.
.XXX.
.XXX.
.....
```




```input3
3 2
..
..
..
```




```input4
9 9
.........
.XXXXX.X.
.X...X...
.X.XXXXX.
.X.X.X.X.
.X.XXX.X.
.X.....X.
.XXXXXXX.
.........
```




```output1
YES
4 1 4 4 1
4 5 5 5 1
4 5 1 5 4
1 5 5 5 4
1 4 4 1 4
```




```output2
NO
```




```output3
YES
4 1
4 1
1 4
```




```output4
YES
4 4 4 1 4 1 4 1 4
1 5 5 5 5 5 4 10 1
4 5 1 4 1 5 4 4 4
4 5 1 5 5 0 5 5 1
4 5 1 5 4 5 1 5 4
4 5 1 5 5 5 4 5 1
1 5 4 4 1 1 4 5 1
4 5 5 5 5 5 5 5 4
1 1 1 1 4 4 1 1 4
```



## Note

<p>It can be shown that no such grid exists for the second test.</p>
