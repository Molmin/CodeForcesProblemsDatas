## Description

<div><p>Rats have bred to hundreds and hundreds in the basement of the store, owned by Vasily Petrovich. Vasily Petrovich may have not noticed their presence, but they got into the habit of sneaking into the warehouse and stealing food from there. Vasily Petrovich cannot put up with it anymore, he has to destroy the rats in the basement. Since mousetraps are outdated and do not help, and rat poison can poison inattentive people as well as rats, he chose a radical way: to blow up two grenades in the basement (he does not have more).</p><p>In this problem, we will present the shop basement as a rectangular table of <span class="tex-span"><i>n</i> × <i>m</i></span> cells. Some of the cells are occupied by walls, and the rest of them are empty. Vasily has been watching the rats and he found out that at a certain time they go to sleep, and all the time they sleep in the same places. He wants to blow up a grenade when this convenient time comes. On the plan of his basement, he marked cells with sleeping rats in them. Naturally, these cells are not occupied by walls.</p><p>Grenades can only blow up in a cell that is not occupied by a wall. The blast wave from a grenade distributes as follows. We assume that the grenade blast occurs at time 0. During this initial time only the cell where the grenade blew up gets 'clear'. If at time <span class="tex-span"><i>t</i></span> some cell is clear, then at time <span class="tex-span"><i>t</i> + 1</span> those side-neighbouring cells which are not occupied by the walls get clear too (some of them could have been cleared before). The blast wave distributes for exactly <span class="tex-span"><i>d</i></span> seconds, then it dies immediately.</p><center> <img class="tex-graphics" src="file://6xJBon03.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-script">An example of a distributing blast wave: Picture 1 shows the situation before the blast, and the following pictures show "clear" cells by time 0,1,2,3 and 4. Thus, the blast wave on the picture distributes for <span class="tex-span"><i>d</i> = 4</span> seconds.</span> </center><p>Vasily Petrovich wonders, whether he can choose two cells to blast the grenades so as to clear all cells with sleeping rats. Write the program that finds it out.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span>, separated by single spaces (<span class="tex-span">4 ≤ <i>n</i>, <i>m</i> ≤ 1000, 1 ≤ <i>d</i> ≤ 8</span>). Next <span class="tex-span"><i>n</i></span> lines contain the table that represents the basement plan. Each row of the table consists of <span class="tex-span"><i>m</i></span> characters. Character "<span class="tex-font-style-tt">X</span>" means that the corresponding cell is occupied by the wall, character "<span class="tex-font-style-tt">.</span>" represents a empty cell, character "<span class="tex-font-style-tt">R</span>" represents a empty cell with sleeping rats. </p><p>It is guaranteed that the first and the last row, as well as the first and the last column consist of characters "<span class="tex-font-style-tt">X</span>". The plan has at least two empty cells. There is at least one cell with sleeping rats.</p></div><div class="output-specification"><p>If it is impossible to blow up all cells with sleeping rats, print a single integer <span class="tex-font-style-tt">-1</span>. Otherwise, print four space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub></span>, that mean that one grenade should go off in cell <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span>, and the other one — in cell <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>. </p><p>Consider the table rows numbered from top to bottom from 1 to <span class="tex-span"><i>n</i></span> and the table columns — from left to right from 1 to <span class="tex-span"><i>m</i></span>. As <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> represent the row numbers, and <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> represent the column numbers in the table, they should fit the limits: <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>. It is forbidden to blow a grenade twice in the same cell. The blast waves of the grenades can intersect. It is possible that one grenade blast destroys no rats, and the other one destroys all of them.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span>, separated by single spaces (<span class="tex-span">4 ≤ <i>n</i>, <i>m</i> ≤ 1000, 1 ≤ <i>d</i> ≤ 8</span>). Next <span class="tex-span"><i>n</i></span> lines contain the table that represents the basement plan. Each row of the table consists of <span class="tex-span"><i>m</i></span> characters. Character "<span class="tex-font-style-tt">X</span>" means that the corresponding cell is occupied by the wall, character "<span class="tex-font-style-tt">.</span>" represents a empty cell, character "<span class="tex-font-style-tt">R</span>" represents a empty cell with sleeping rats. </p><p>It is guaranteed that the first and the last row, as well as the first and the last column consist of characters "<span class="tex-font-style-tt">X</span>". The plan has at least two empty cells. There is at least one cell with sleeping rats.</p>

## Output

<p>If it is impossible to blow up all cells with sleeping rats, print a single integer <span class="tex-font-style-tt">-1</span>. Otherwise, print four space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub></span>, that mean that one grenade should go off in cell <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span>, and the other one — in cell <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>. </p><p>Consider the table rows numbered from top to bottom from 1 to <span class="tex-span"><i>n</i></span> and the table columns — from left to right from 1 to <span class="tex-span"><i>m</i></span>. As <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> represent the row numbers, and <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> represent the column numbers in the table, they should fit the limits: <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>. It is forbidden to blow a grenade twice in the same cell. The blast waves of the grenades can intersect. It is possible that one grenade blast destroys no rats, and the other one destroys all of them.</p>





```input1
4 4 1
XXXX
XR.X
X.RX
XXXX

```




```input2
9 14 5
XXXXXXXXXXXXXX
X....R...R...X
X..R.........X
X....RXR..R..X
X..R...X.....X
XR.R...X.....X
X....XXR.....X
X....R..R.R..X
XXXXXXXXXXXXXX

```




```input3
7 7 1
XXXXXXX
X.R.R.X
X.....X
X..X..X
X..R..X
X....RX
XXXXXXX

```




```output1
2 2 2 3

```




```output2
2 3 6 9

```




```output3
-1

```


