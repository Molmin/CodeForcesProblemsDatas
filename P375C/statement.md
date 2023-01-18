## Description

<div><p>You have a map as a rectangle table. Each cell of the table is either an obstacle, or a treasure with a certain price, or a bomb, or an empty cell. Your initial position is also given to you.</p><p>You can go from one cell of the map to a side-adjacent one. At that, you are not allowed to go beyond the borders of the map, enter the cells with treasures, obstacles and bombs. To pick the treasures, you need to build a closed path (starting and ending in the starting cell). The closed path mustn't contain any cells with bombs inside. Let's assume that the sum of the treasures' values that are located inside the closed path equals <span class="tex-span"><i>v</i></span>, and besides, you've made <span class="tex-span"><i>k</i></span> single moves (from one cell to another) while you were going through the path, then such path brings you the profit of <span class="tex-span"><i>v</i> - <i>k</i></span> rubles.</p><p>Your task is to build a closed path that doesn't contain any bombs and brings maximum profit.</p><p>Note that the path can have self-intersections. In order to determine if a cell lies inside a path or not, use the following algorithm:</p><ol> <li> Assume that the table cells are points on the plane (the table cell on the intersection of the <span class="tex-span"><i>i</i></span>-th column and the <span class="tex-span"><i>j</i></span>-th row is point <span class="tex-span">(<i>i</i>, <i>j</i>)</span>). And the given path is a closed polyline that goes through these points. </li><li> You need to find out if the point <span class="tex-span"><i>p</i></span> of the table that is not crossed by the polyline lies inside the polyline. </li><li> Let's draw a ray that starts from point <span class="tex-span"><i>p</i></span> and does not intersect other points of the table (such ray must exist). </li><li> Let's count the number of segments of the polyline that intersect the painted ray. If this number is odd, we assume that point <span class="tex-span"><i>p</i></span> (and consequently, the table cell) lie inside the polyline (path). Otherwise, we assume that it lies outside. </li></ol></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 20)</span> — the sizes of the table. Next <span class="tex-span"><i>n</i></span> lines each contains <span class="tex-span"><i>m</i></span> characters — the description of the table. The description means the following:</p><ul> <li> character "<span class="tex-font-style-tt">B</span>" is a cell with a bomb; </li><li> character "<span class="tex-font-style-tt">S</span>" is the starting cell, you can assume that it's empty; </li><li> digit <span class="tex-span"><i>c</i></span> (<span class="tex-font-style-tt">1-8</span>) is treasure with index <span class="tex-span"><i>c</i></span>; </li><li> character "<span class="tex-font-style-tt">.</span>" is an empty cell; </li><li> character "<span class="tex-font-style-tt">#</span>" is an obstacle. </li></ul><p>Assume that the map has <span class="tex-span"><i>t</i></span> treasures. Next <span class="tex-span"><i>t</i></span> lines contain the prices of the treasures. The <span class="tex-span"><i>i</i></span>-th line contains the price of the treasure with index <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 200 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 200)</span>. It is guaranteed that the treasures are numbered from 1 to <span class="tex-span"><i>t</i></span>. It is guaranteed that the map has not more than 8 objects in total. Objects are bombs and treasures. It is guaranteed that the map has exactly one character "<span class="tex-font-style-tt">S</span>".</p></div><div class="output-specification"><p>Print a single integer — the maximum possible profit you can get.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 20)</span> — the sizes of the table. Next <span class="tex-span"><i>n</i></span> lines each contains <span class="tex-span"><i>m</i></span> characters — the description of the table. The description means the following:</p><ul> <li> character "<span class="tex-font-style-tt">B</span>" is a cell with a bomb; </li><li> character "<span class="tex-font-style-tt">S</span>" is the starting cell, you can assume that it's empty; </li><li> digit <span class="tex-span"><i>c</i></span> (<span class="tex-font-style-tt">1-8</span>) is treasure with index <span class="tex-span"><i>c</i></span>; </li><li> character "<span class="tex-font-style-tt">.</span>" is an empty cell; </li><li> character "<span class="tex-font-style-tt">#</span>" is an obstacle. </li></ul><p>Assume that the map has <span class="tex-span"><i>t</i></span> treasures. Next <span class="tex-span"><i>t</i></span> lines contain the prices of the treasures. The <span class="tex-span"><i>i</i></span>-th line contains the price of the treasure with index <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 200 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 200)</span>. It is guaranteed that the treasures are numbered from 1 to <span class="tex-span"><i>t</i></span>. It is guaranteed that the map has not more than 8 objects in total. Objects are bombs and treasures. It is guaranteed that the map has exactly one character "<span class="tex-font-style-tt">S</span>".</p>

## Output

<p>Print a single integer — the maximum possible profit you can get.</p>





```input1
4 4
....
.S1.
....
....
10

```




```input2
7 7
.......
.1###2.
.#...#.
.#.B.#.
.3...4.
..##...
......S
100
100
100
100

```




```input3
7 8
........
........
....1B..
.S......
....2...
3.......
........
100
-100
100

```




```input4
1 1
S

```




```output1
2

```




```output2
364

```




```output3
0

```




```output4
0

```



## Note

<p>In the first example the answer will look as follows.</p><center> <img class="tex-graphics" src="file://7s5nJSF9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example the answer will look as follows.</p><center> <img class="tex-graphics" src="file://XD7jsnu4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third example you cannot get profit.</p><p>In the fourth example you cannot get profit as you cannot construct a closed path with more than one cell.</p>
