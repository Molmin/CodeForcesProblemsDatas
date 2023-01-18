## Description

<div><p>They say "<span class="tex-font-style-it">years are like dominoes, tumbling one after the other</span>". But would a year fit into a grid? I don't think so.</p><p>Limak is a little polar bear who loves to play. He has recently got a rectangular grid with <span class="tex-span"><i>h</i></span> rows and <span class="tex-span"><i>w</i></span> columns. Each cell is a square, either empty (denoted by '<span class="tex-font-style-tt">.</span>') or forbidden (denoted by '<span class="tex-font-style-tt">#</span>'). Rows are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>h</i></span> from top to bottom. Columns are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>w</i></span> from left to right.</p><p>Also, Limak has a single domino. He wants to put it somewhere in a grid. A domino will occupy exactly two adjacent cells, located either in one row or in one column. Both adjacent cells must be empty and must be inside a grid.</p><p>Limak needs more fun and thus he is going to consider some queries. In each query he chooses some rectangle and wonders, how many way are there to put a single domino inside of the chosen rectangle?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>h</i>, <i>w</i> ≤ 500</span>)&nbsp;– the number of rows and the number of columns, respectively.</p><p>The next <span class="tex-span"><i>h</i></span> lines describe a grid. Each line contains a string of the length <span class="tex-span"><i>w</i></span>. Each character is either '<span class="tex-font-style-tt">.</span>' or '<span class="tex-font-style-tt">#</span>'&nbsp;— denoting an empty or forbidden cell, respectively.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of queries.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains four integers <span class="tex-span"><i>r</i>1<sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i>1<sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i>2<sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i>2<sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i>1<sub class="lower-index"><i>i</i></sub> ≤ <i>r</i>2<sub class="lower-index"><i>i</i></sub> ≤ <i>h</i>, 1 ≤ <i>c</i>1<sub class="lower-index"><i>i</i></sub> ≤ <i>c</i>2<sub class="lower-index"><i>i</i></sub> ≤ <i>w</i></span>)&nbsp;— the <span class="tex-span"><i>i</i></span>-th query. Numbers <span class="tex-span"><i>r</i>1<sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i>1<sub class="lower-index"><i>i</i></sub></span> denote the row and the column (respectively) of the upper left cell of the rectangle. Numbers <span class="tex-span"><i>r</i>2<sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i>2<sub class="lower-index"><i>i</i></sub></span> denote the row and the column (respectively) of the bottom right cell of the rectangle.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> integers, <span class="tex-span"><i>i</i></span>-th should be equal to the number of ways to put a single domino inside the <span class="tex-span"><i>i</i></span>-th rectangle.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>h</i>, <i>w</i> ≤ 500</span>)&nbsp;– the number of rows and the number of columns, respectively.</p><p>The next <span class="tex-span"><i>h</i></span> lines describe a grid. Each line contains a string of the length <span class="tex-span"><i>w</i></span>. Each character is either '<span class="tex-font-style-tt">.</span>' or '<span class="tex-font-style-tt">#</span>'&nbsp;— denoting an empty or forbidden cell, respectively.</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of queries.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains four integers <span class="tex-span"><i>r</i>1<sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i>1<sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i>2<sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i>2<sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i>1<sub class="lower-index"><i>i</i></sub> ≤ <i>r</i>2<sub class="lower-index"><i>i</i></sub> ≤ <i>h</i>, 1 ≤ <i>c</i>1<sub class="lower-index"><i>i</i></sub> ≤ <i>c</i>2<sub class="lower-index"><i>i</i></sub> ≤ <i>w</i></span>)&nbsp;— the <span class="tex-span"><i>i</i></span>-th query. Numbers <span class="tex-span"><i>r</i>1<sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i>1<sub class="lower-index"><i>i</i></sub></span> denote the row and the column (respectively) of the upper left cell of the rectangle. Numbers <span class="tex-span"><i>r</i>2<sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i>2<sub class="lower-index"><i>i</i></sub></span> denote the row and the column (respectively) of the bottom right cell of the rectangle.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> integers, <span class="tex-span"><i>i</i></span>-th should be equal to the number of ways to put a single domino inside the <span class="tex-span"><i>i</i></span>-th rectangle.</p>





```input1
5 8
....#..#
.#......
##.#....
##..#.##
........
4
1 1 2 3
4 1 4 1
1 2 4 5
2 5 5 8

```




```input2
7 39
.......................................
.###..###..#..###.....###..###..#..###.
...#..#.#..#..#.........#..#.#..#..#...
.###..#.#..#..###.....###..#.#..#..###.
.#....#.#..#....#.....#....#.#..#..#.#.
.###..###..#..###.....###..###..#..###.
.......................................
6
1 1 3 20
2 10 6 30
2 10 7 30
2 2 7 7
1 7 7 7
1 8 7 8

```




```output1
4
0
10
15

```




```output2
53
89
120
23
0
2

```



## Note

<p>A red frame below corresponds to the first query of the first sample. A domino can be placed in 4 possible ways.</p><center> <img class="tex-graphics" src="file://VdjZzIZj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
