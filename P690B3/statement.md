## Description

<div><p>Zombies have found out about the Zombie Contamination level checker and managed to damage it! Now detecting the shape of their main compound will be a real challenge for Heidi. As before, a lair can be represented as a strictly convex polygon on a lattice. Each vertex of the polygon occupies a point on the lattice. However, the damaged Zombie Contamination level checker can only tell, for each cell, whether the level of Zombie Contamination for that cell is in the set <span class="tex-span">{1, 2, 3}</span>. In other words, Heidi knows all the cells of the lattice for which the Contamination level is not <span class="tex-span">0</span> and not <span class="tex-span">4</span>.</p><p>Given this information, Heidi still wants to know the exact shape of the lair to rain destruction on the zombies. Help her!</p></div><div class="input-specification"><p>The input contains multiple test cases.</p><p>The first line of each test case contains two space-separated integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span>, where <span class="tex-span"><i>N</i></span> is the size of the lattice grid (<span class="tex-span">5 ≤ <i>N</i> ≤ 100000</span>) and <span class="tex-span"><i>M</i></span> is the number of lattice points for which the Zombie Contamination level is 1, 2, or 3 (<span class="tex-span">8 ≤ <i>M</i> ≤ 200000</span>).</p><p>The second line of each test case contains <span class="tex-span"><i>M</i></span> pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>M</i></sub>, <i>y</i><sub class="lower-index"><i>M</i></sub></span> – coordinates of the cells with Zombie Contamination level not equal to 0 nor 4. It is guaranteed that <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>N</i></span>. All pairs <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> are different.</p><p>Cells are enumerated based on the coordinates of their upper right corner. This means that the bottommost leftmost cell that touches the origin has coordinates <span class="tex-span">(1, 1)</span>, and the uppermost leftmost cell is identified as <span class="tex-span">(1, <i>N</i>)</span>.</p><p>The last line of the file contains two zeroes. This line should not be treated as a test case. The sum of the <span class="tex-span"><i>M</i></span> values for all tests in one file will not exceed <span class="tex-span">200000</span>.</p></div><div class="output-specification"><p>For each test case, the following output is expected:</p><p>The first line of the output should contain one integer <span class="tex-span"><i>V</i></span>, the number of vertices of the polygon that is the secret lair. The next <span class="tex-span"><i>V</i></span> lines each should contain two integers, denoting the vertices of the polygon in the clockwise order, starting from the lexicographically smallest vertex.</p></div>

## Input

<p>The input contains multiple test cases.</p><p>The first line of each test case contains two space-separated integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span>, where <span class="tex-span"><i>N</i></span> is the size of the lattice grid (<span class="tex-span">5 ≤ <i>N</i> ≤ 100000</span>) and <span class="tex-span"><i>M</i></span> is the number of lattice points for which the Zombie Contamination level is 1, 2, or 3 (<span class="tex-span">8 ≤ <i>M</i> ≤ 200000</span>).</p><p>The second line of each test case contains <span class="tex-span"><i>M</i></span> pairs of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>M</i></sub>, <i>y</i><sub class="lower-index"><i>M</i></sub></span> – coordinates of the cells with Zombie Contamination level not equal to 0 nor 4. It is guaranteed that <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>N</i></span>. All pairs <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> are different.</p><p>Cells are enumerated based on the coordinates of their upper right corner. This means that the bottommost leftmost cell that touches the origin has coordinates <span class="tex-span">(1, 1)</span>, and the uppermost leftmost cell is identified as <span class="tex-span">(1, <i>N</i>)</span>.</p><p>The last line of the file contains two zeroes. This line should not be treated as a test case. The sum of the <span class="tex-span"><i>M</i></span> values for all tests in one file will not exceed <span class="tex-span">200000</span>.</p>

## Output

<p>For each test case, the following output is expected:</p><p>The first line of the output should contain one integer <span class="tex-span"><i>V</i></span>, the number of vertices of the polygon that is the secret lair. The next <span class="tex-span"><i>V</i></span> lines each should contain two integers, denoting the vertices of the polygon in the clockwise order, starting from the lexicographically smallest vertex.</p>





```input1
8 19
2 3 2 4 2 5 3 3 3 5 4 3 4 5 4 6 5 2 5 3 5 6 6 2 6 3 6 4 6 5 6 6 6 7 7 6 7 7
5 8
2 2 2 3 2 4 3 2 3 4 4 2 4 3 4 4
0 0

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

```



## Note

<p>It is guaranteed that the solution always exists and is unique. It is guaranteed that in the correct solution the coordinates of the polygon vertices are between <span class="tex-span">1</span> and <span class="tex-span"><i>N</i> - 1</span>. A vertex <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> is lexicographically smaller than vertex <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> if <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub></span> or <img align="middle" class="tex-formula" src="file://ra4j09Ff.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
