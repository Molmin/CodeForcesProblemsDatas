## Description

<div><p>Arkady is playing Battleship. The rules of this game aren't really important.</p><p>There is a field of $n \times n$ cells. There should be exactly one $k$-decker on the field, i.&nbsp;e. a ship that is $k$ cells long oriented either horizontally or vertically. However, Arkady doesn't know where it is located. For each cell Arkady knows if it is definitely empty or can contain a part of the ship.</p><p>Consider all possible locations of the ship. Find such a cell that belongs to the maximum possible number of different locations of the ship.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 100$)&nbsp;— the size of the field and the size of the ship.</p><p>The next $n$ lines contain the field. Each line contains $n$ characters, each of which is either '<span class="tex-font-style-tt">#</span>' (denotes a definitely empty cell) or '<span class="tex-font-style-tt">.</span>' (denotes a cell that can belong to the ship).</p></div><div class="output-specification"><p>Output two integers&nbsp;— the row and the column of a cell that belongs to the maximum possible number of different locations of the ship.</p><p>If there are multiple answers, output any of them. In particular, if no ship can be placed on the field, you can output any cell.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 100$)&nbsp;— the size of the field and the size of the ship.</p><p>The next $n$ lines contain the field. Each line contains $n$ characters, each of which is either '<span class="tex-font-style-tt">#</span>' (denotes a definitely empty cell) or '<span class="tex-font-style-tt">.</span>' (denotes a cell that can belong to the ship).</p>

## Output

<p>Output two integers&nbsp;— the row and the column of a cell that belongs to the maximum possible number of different locations of the ship.</p><p>If there are multiple answers, output any of them. In particular, if no ship can be placed on the field, you can output any cell.</p>





```input1
4 3
#..#
#.#.
....
.###

```




```input2
10 4
#....##...
.#...#....
..#..#..#.
...#.#....
.#..##.#..
.....#...#
...#.##...
.#...#.#..
.....#..#.
...#.#...#

```




```input3
19 6
##..............###
#......#####.....##
.....#########.....
....###########....
...#############...
..###############..
.#################.
.#################.
.#################.
.#################.
#####....##....####
####............###
####............###
#####...####...####
.#####..####..#####
...###........###..
....###########....
.........##........
#.................#

```




```output1
3 2

```




```output2
6 1

```




```output3
1 8

```



## Note

<p>The picture below shows the three possible locations of the ship that contain the cell $(3, 2)$ in the first sample.</p><center> <img class="tex-graphics" height="378px" src="file://dlTRjVtH.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center>
