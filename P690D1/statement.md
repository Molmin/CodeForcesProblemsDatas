## Description

<div><p><span class="tex-font-style-it">"The zombies are lurking outside. Waiting. Moaning. And when they come..."</span></p><p><span class="tex-font-style-it">"When they come?"</span></p><p><span class="tex-font-style-it">"I hope the Wall is high enough."</span></p><p>Zombie attacks have hit the Wall, our line of defense in the North. Its protection is failing, and cracks are showing. In places, gaps have appeared, splitting the wall into multiple segments. We call on <span class="tex-font-style-it">you</span> for help. Go forth and explore the wall! Report how many disconnected segments there are.</p><p>The wall is a two-dimensional structure made of bricks. Each brick is one unit wide and one unit high. Bricks are stacked on top of each other to form columns that are up to <span class="tex-span"><i>R</i></span> bricks high. Each brick is placed either on the ground or directly on top of another brick. Consecutive non-empty columns form a <span class="tex-font-style-it">wall segment</span>. The entire wall, all the segments and empty columns in-between, is <span class="tex-span"><i>C</i></span> columns wide.</p></div><div class="input-specification"><p>The first line of the input consists of two space-separated integers <span class="tex-span"><i>R</i></span> and <span class="tex-span"><i>C</i></span>, <span class="tex-span">1 ≤ <i>R</i>, <i>C</i> ≤ 100</span>. The next <span class="tex-span"><i>R</i></span> lines provide a description of the columns as follows: </p><ul> <li> each of the <span class="tex-span"><i>R</i></span> lines contains a string of length <span class="tex-span"><i>C</i></span>, </li><li> the <span class="tex-span"><i>c</i></span>-th character of line <span class="tex-span"><i>r</i></span> is <span class="tex-font-style-tt">B</span> if there is a brick in column <span class="tex-span"><i>c</i></span> and row <span class="tex-span"><i>R</i> - <i>r</i> + 1</span>, and <span class="tex-font-style-tt">.</span> otherwise. </li></ul> The input will contain at least one character <span class="tex-font-style-tt">B</span> and it will be valid.</div><div class="output-specification"><p>The number of wall segments in the input configuration.</p></div>

## Input

<p>The first line of the input consists of two space-separated integers <span class="tex-span"><i>R</i></span> and <span class="tex-span"><i>C</i></span>, <span class="tex-span">1 ≤ <i>R</i>, <i>C</i> ≤ 100</span>. The next <span class="tex-span"><i>R</i></span> lines provide a description of the columns as follows: </p><ul> <li> each of the <span class="tex-span"><i>R</i></span> lines contains a string of length <span class="tex-span"><i>C</i></span>, </li><li> the <span class="tex-span"><i>c</i></span>-th character of line <span class="tex-span"><i>r</i></span> is <span class="tex-font-style-tt">B</span> if there is a brick in column <span class="tex-span"><i>c</i></span> and row <span class="tex-span"><i>R</i> - <i>r</i> + 1</span>, and <span class="tex-font-style-tt">.</span> otherwise. </li></ul> The input will contain at least one character <span class="tex-font-style-tt">B</span> and it will be valid.

## Output

<p>The number of wall segments in the input configuration.</p>





```input1
3 7
.......
.......
.BB.B..

```




```input2
4 5
..B..
..B..
B.B.B
BBB.B

```




```input3
4 6
..B...
B.B.BB
BBB.BB
BBBBBB

```




```input4
1 1
B

```




```input5
10 7
.......
.......
.......
.......
.......
.......
.......
.......
...B...
B.BB.B.

```




```input6
8 8
........
........
........
........
.B......
.B.....B
.B.....B
.BB...BB

```




```output1
2

```




```output2
2

```




```output3
1

```




```output4
1

```




```output5
3

```




```output6
2

```



## Note

<p>In the first sample case, the 2nd and 3rd columns define the first wall segment, and the 5th column defines the second.</p>
