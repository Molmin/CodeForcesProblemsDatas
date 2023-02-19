## Description

<div><p>You are given a matrix, consisting of $n$ rows and $m$ columns. The rows are numbered top to bottom, the columns are numbered left to right.</p><p>Each cell of the matrix can be either free or locked.</p><p>Let's call a path in the matrix <span class="tex-font-style-it">a staircase</span> if it: </p><ul> <li> starts and ends in the free cell; </li><li> visits only free cells; </li><li> has one of the two following structures: <ol> <li> the second cell is $1$ to the right from the first one, the third cell is $1$ to the bottom from the second one, the fourth cell is $1$ to the right from the third one, and so on; </li><li> the second cell is $1$ to the bottom from the first one, the third cell is $1$ to the right from the second one, the fourth cell is $1$ to the bottom from the third one, and so on. </li></ol> </li></ul><p>In particular, a path, consisting of a single cell, is considered to be a staircase.</p><p>Here are some examples of staircases:</p><center> <img class="tex-graphics" src="file://bChIx0XL.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Initially all the cells of the matrix are <span class="tex-font-style-bf">free</span>.</p><p>You have to process $q$ queries, each of them flips the state of a single cell. So, if a cell is currently free, it makes it locked, and if a cell is currently locked, it makes it free.</p><p>Print the number of different staircases after each query. Two staircases are considered different if there exists such a cell that appears in one path and doesn't appear in the other path.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $q$ ($1 \le n, m \le 1000$; $1 \le q \le 10^4$)&nbsp;— the sizes of the matrix and the number of queries.</p><p>Each of the next $q$ lines contains two integers $x$ and $y$ ($1 \le x \le n$; $1 \le y \le m$)&nbsp;— the description of each query.</p></div><div class="output-specification"><p>Print $q$ integers&nbsp;— the $i$-th value should be equal to the number of different staircases after $i$ queries. Two staircases are considered different if there exists such a cell that appears in one path and doesn't appear in the other path.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $q$ ($1 \le n, m \le 1000$; $1 \le q \le 10^4$)&nbsp;— the sizes of the matrix and the number of queries.</p><p>Each of the next $q$ lines contains two integers $x$ and $y$ ($1 \le x \le n$; $1 \le y \le m$)&nbsp;— the description of each query.</p>

## Output

<p>Print $q$ integers&nbsp;— the $i$-th value should be equal to the number of different staircases after $i$ queries. Two staircases are considered different if there exists such a cell that appears in one path and doesn't appear in the other path.</p>





```input1
2 2 8
1 1
1 1
1 1
2 2
1 1
1 2
2 1
1 1
```




```input2
3 4 10
1 4
1 2
2 3
1 2
2 3
3 2
1 3
3 4
1 3
3 1
```




```input3
1000 1000 2
239 634
239 634
```




```output1
5
10
5
2
5
3
1
0
```




```output2
49
35
24
29
49
39
31
23
29
27
```




```output3
1332632508
1333333000
```


