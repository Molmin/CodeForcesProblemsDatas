## Description

<div><p>The last product of the R2 company in the 2D games' field is a new revolutionary algorithm of searching for the shortest path in a <span class="tex-span">2 × <i>n</i></span> maze.</p><p>Imagine a maze that looks like a <span class="tex-span">2 × <i>n</i></span> rectangle, divided into unit squares. Each unit square is either an empty cell or an obstacle. In one unit of time, a person can move from an empty cell of the maze to any side-adjacent empty cell. The shortest path problem is formulated as follows. Given two free maze cells, you need to determine the minimum time required to go from one cell to the other.</p><p>Unfortunately, the developed algorithm works well for only one request for finding the shortest path, in practice such requests occur quite often. You, as the chief R2 programmer, are commissioned to optimize the algorithm to find the shortest path. Write a program that will effectively respond to multiple requests to find the shortest path in a <span class="tex-span">2 × <i>n</i></span> maze.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the width of the maze and the number of queries, correspondingly. Next two lines contain the maze. Each line contains <span class="tex-span"><i>n</i></span> characters, each character equals either '<span class="tex-font-style-tt">.</span>' (empty cell), or '<span class="tex-font-style-tt">X</span>' (obstacle).</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>n</i>)</span> — the description of the <span class="tex-span"><i>i</i></span>-th request. Numbers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> mean that you need to print the value of the shortest path from the cell of the maze number <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to the cell number <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>. We assume that the cells of the first line of the maze are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, from left to right, and the cells of the second line are numbered from <span class="tex-span"><i>n</i> + 1</span> to <span class="tex-span">2<i>n</i></span> from left to right. It is guaranteed that both given cells are empty.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print the answer to the <span class="tex-span"><i>i</i></span>-th request — either the size of the shortest path or -1, if we can't reach the second cell from the first one.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the width of the maze and the number of queries, correspondingly. Next two lines contain the maze. Each line contains <span class="tex-span"><i>n</i></span> characters, each character equals either '<span class="tex-font-style-tt">.</span>' (empty cell), or '<span class="tex-font-style-tt">X</span>' (obstacle).</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>n</i>)</span> — the description of the <span class="tex-span"><i>i</i></span>-th request. Numbers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> mean that you need to print the value of the shortest path from the cell of the maze number <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to the cell number <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>. We assume that the cells of the first line of the maze are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, from left to right, and the cells of the second line are numbered from <span class="tex-span"><i>n</i> + 1</span> to <span class="tex-span">2<i>n</i></span> from left to right. It is guaranteed that both given cells are empty.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print the answer to the <span class="tex-span"><i>i</i></span>-th request — either the size of the shortest path or -1, if we can't reach the second cell from the first one.</p>





```input1
4 7
.X..
...X
5 1
1 3
7 7
1 4
6 1
4 7
5 7

```




```input2
10 3
X...X..X..
..X...X..X
11 7
7 18
18 10

```




```output1
1
4
0
5
2
2
2

```




```output2
9
-1
3

```


