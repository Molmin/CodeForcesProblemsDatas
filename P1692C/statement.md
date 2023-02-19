## Description

<div><p>Mihai has an $8 \times 8$ chessboard whose rows are numbered from $1$ to $8$ from top to bottom and whose columns are numbered from $1$ to $8$ from left to right.</p><p>Mihai has placed exactly one bishop on the chessboard. <span class="tex-font-style-bf">The bishop is not placed on the edges of the board.</span> (In other words, the row and column of the bishop are between $2$ and $7$, inclusive.)</p><p>The bishop attacks in all directions diagonally, and there is no limit to the distance which the bishop can attack. Note that the cell on which the bishop is placed is also considered attacked. </p><center> <img class="tex-graphics" src="file://HEszFAsz.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">An example of a bishop on a chessboard. The squares it attacks are marked in red.</span> </center><p>Mihai has marked all squares the bishop attacks, but forgot where the bishop was! Help Mihai find the position of the bishop.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \leq t \leq 36$)&nbsp;— the number of test cases. The description of test cases follows. There is an empty line before each test case.</p><p>Each test case consists of $8$ lines, each containing $8$ characters. Each of these characters is either '<span class="tex-font-style-tt">#</span>' or '<span class="tex-font-style-tt">.</span>', denoting a square under attack and a square not under attack, respectively.</p></div><div class="output-specification"><p>For each test case, output two integers $r$ and $c$ ($2 \leq r, c \leq 7$)&nbsp;— the row and column of the bishop. </p><p>The input is generated in such a way that there is always exactly one possible location of the bishop that is not on the edge of the board.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \leq t \leq 36$)&nbsp;— the number of test cases. The description of test cases follows. There is an empty line before each test case.</p><p>Each test case consists of $8$ lines, each containing $8$ characters. Each of these characters is either '<span class="tex-font-style-tt">#</span>' or '<span class="tex-font-style-tt">.</span>', denoting a square under attack and a square not under attack, respectively.</p>

## Output

<p>For each test case, output two integers $r$ and $c$ ($2 \leq r, c \leq 7$)&nbsp;— the row and column of the bishop. </p><p>The input is generated in such a way that there is always exactly one possible location of the bishop that is not on the edge of the board.</p>





```input1
3

.....#..
#...#...
.#.#....
..#.....
.#.#....
#...#...
.....#..
......#.

#.#.....
.#......
#.#.....
...#....
....#...
.....#..
......#.
.......#

.#.....#
..#...#.
...#.#..
....#...
...#.#..
..#...#.
.#.....#
#.......
```




```output1
4 3
2 2
4 5
```



## Note

<p>The first test case is pictured in the statement. Since the bishop lies in the intersection row $4$ and column $3$, the correct output is <span class="tex-font-style-tt">4 3</span>.</p>
