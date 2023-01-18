## Description

<div><p>Now that Heidi has made sure her Zombie Contamination level checker works, it's time to strike! This time, the zombie lair is a strictly convex polygon on the lattice. Each vertex of the polygon occupies a point on the lattice. For each cell of the lattice, Heidi knows the level of Zombie Contamination – the number of corners of the cell that are inside or on the border of the lair.</p><p>Given this information, Heidi wants to know the exact shape of the lair to rain destruction on the zombies. Help her!</p><p><img class="tex-graphics" src="file://B2NcRPD2.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"></p></div><div class="input-specification"><p>The input contains multiple test cases.</p><p>The first line of each test case contains one integer <span class="tex-span"><i>N</i></span>, the size of the lattice grid (<span class="tex-span">5 ≤ <i>N</i> ≤ 500</span>). The next <span class="tex-span"><i>N</i></span> lines each contain <span class="tex-span"><i>N</i></span> characters, describing the level of Zombie Contamination of each cell in the lattice. Every character of every line is a digit between 0 and 4. </p><p>Cells are given in the same order as they are shown in the picture above: rows go in the decreasing value of <span class="tex-span"><i>y</i></span> coordinate, and in one row cells go in the order of increasing <span class="tex-span"><i>x</i></span> coordinate. This means that the first row corresponds to cells with coordinates <span class="tex-span">(1, <i>N</i>), ..., (<i>N</i>, <i>N</i>)</span> and the last row corresponds to cells with coordinates <span class="tex-span">(1, 1), ..., (<i>N</i>, 1)</span>.</p><p>The last line of the file contains a zero. This line should not be treated as a test case. The sum of the <span class="tex-span"><i>N</i></span> values for all tests in one file will not exceed <span class="tex-span">5000</span>.</p></div><div class="output-specification"><p>For each test case, give the following output:</p><p>The first line of the output should contain one integer <span class="tex-span"><i>V</i></span>, the number of vertices of the polygon that is the secret lair. The next <span class="tex-span"><i>V</i></span> lines each should contain two integers, denoting the vertices of the polygon in the clockwise order, starting from the lexicographically smallest vertex.</p></div>

## Input

<p>The input contains multiple test cases.</p><p>The first line of each test case contains one integer <span class="tex-span"><i>N</i></span>, the size of the lattice grid (<span class="tex-span">5 ≤ <i>N</i> ≤ 500</span>). The next <span class="tex-span"><i>N</i></span> lines each contain <span class="tex-span"><i>N</i></span> characters, describing the level of Zombie Contamination of each cell in the lattice. Every character of every line is a digit between 0 and 4. </p><p>Cells are given in the same order as they are shown in the picture above: rows go in the decreasing value of <span class="tex-span"><i>y</i></span> coordinate, and in one row cells go in the order of increasing <span class="tex-span"><i>x</i></span> coordinate. This means that the first row corresponds to cells with coordinates <span class="tex-span">(1, <i>N</i>), ..., (<i>N</i>, <i>N</i>)</span> and the last row corresponds to cells with coordinates <span class="tex-span">(1, 1), ..., (<i>N</i>, 1)</span>.</p><p>The last line of the file contains a zero. This line should not be treated as a test case. The sum of the <span class="tex-span"><i>N</i></span> values for all tests in one file will not exceed <span class="tex-span">5000</span>.</p>

## Output

<p>For each test case, give the following output:</p><p>The first line of the output should contain one integer <span class="tex-span"><i>V</i></span>, the number of vertices of the polygon that is the secret lair. The next <span class="tex-span"><i>V</i></span> lines each should contain two integers, denoting the vertices of the polygon in the clockwise order, starting from the lexicographically smallest vertex.</p>





```input1
8
00000000
00000110
00012210
01234200
02444200
01223200
00001100
00000000
5
00000
01210
02420
01210
00000
7
0000000
0122100
0134200
0013200
0002200
0001100
0000000
0

```




```output1
4
2 3
2 4
6 6
5 2
4
2 2
2 3
3 3
3 2
3
2 5
4 5
4 2

```



## Note

<p>It is guaranteed that the solution always exists and is unique. It is guaranteed that in the correct solution the coordinates of the polygon vertices are between <span class="tex-span">2</span> and <span class="tex-span"><i>N</i> - 2</span>. A vertex <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> is lexicographically smaller than vertex <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> if <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub></span> or <img align="middle" class="tex-formula" src="file://N15Y3spA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
