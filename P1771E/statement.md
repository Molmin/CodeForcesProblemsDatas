## Description

<div><p>Hossam bought a new piece of ground with length $n$ and width $m$, he divided it into an $n \cdot m$ grid, each cell being of size $1\times1$.</p><p>Since Hossam's name starts with the letter '<span class="tex-font-style-tt">H</span>', he decided to draw the capital letter '<span class="tex-font-style-tt">H</span>' by building walls of size $1\times1$ on some squares of the ground. Each square $1\times1$ on the ground is assigned a quality degree: perfect, medium, or bad.</p><p>The process of building walls to form up letter '<span class="tex-font-style-tt">H</span>' has the following constraints:</p><ul> <li> The letter must consist of one horizontal and two vertical lines. </li><li> The vertical lines must not be in the same or neighboring columns. </li><li> The vertical lines must start in the same row and end in the same row (and thus have the same length). </li><li> The horizontal line should connect the vertical lines, but must not cross them. </li><li> The horizontal line can be in any row between the vertical lines (not only in the middle), except the top and the bottom one. (With the horizontal line in the top row the letter looks like '<span class="tex-font-style-tt">n</span>', and in the bottom row like '<span class="tex-font-style-tt">U</span>'.) </li><li> It is forbidden to build walls in cells of bad quality. </li><li> You can use at most one square of medium quality. </li><li> You can use any number of squares of perfect quality. </li></ul><p>Find the maximum number of walls that can be used to draw the letter '<span class="tex-font-style-tt">H</span>'.</p><p>Check the note for more clarification.</p></div><div class="input-specification"><p>The first line of the input contains two integer numbers $n$, $m$ ($1 \le n, m \le 400$).</p><p>The next $n$ lines of the input contain $m$ characters each, describing the grid. The character '<span class="tex-font-style-tt">.</span>' stands for a perfect square, the character '<span class="tex-font-style-tt">m</span>' stands for a medium square, and the character '<span class="tex-font-style-tt">#</span>' stands for a bad square.</p></div><div class="output-specification"><p>Print a single integer — the maximum number of walls that form a capital letter '<span class="tex-font-style-tt">H</span>'.</p><p>If it is not possible to draw any letter '<span class="tex-font-style-tt">H</span>', print $0$.</p></div>

## Input

<p>The first line of the input contains two integer numbers $n$, $m$ ($1 \le n, m \le 400$).</p><p>The next $n$ lines of the input contain $m$ characters each, describing the grid. The character '<span class="tex-font-style-tt">.</span>' stands for a perfect square, the character '<span class="tex-font-style-tt">m</span>' stands for a medium square, and the character '<span class="tex-font-style-tt">#</span>' stands for a bad square.</p>

## Output

<p>Print a single integer — the maximum number of walls that form a capital letter '<span class="tex-font-style-tt">H</span>'.</p><p>If it is not possible to draw any letter '<span class="tex-font-style-tt">H</span>', print $0$.</p>





```input1
2 3
#m.
.#.
```




```input2
7 8
...#.m..
..m...m.
.#..#.m#
...m..m.
m.......
..#.m.mm
......m.
```




```output1
0
```




```output2
16
```



## Note

<p>In the first test case, we can't build the letter '<span class="tex-font-style-tt">H</span>'.</p><p>For the second test case, the figure below represents the grid and some of the valid letters '<span class="tex-font-style-tt">H</span>'. Perfect, medium, and bad squares are represented with white, yellow, and black colors respectively.</p><center> <img class="tex-graphics" src="file://LmjjJBzW.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
