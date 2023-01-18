## Description

<div><p>Little Petya is preparing for the first contact with aliens. He knows that alien spaceships have shapes of non-degenerate triangles and there will be exactly 4 ships. Landing platform for a ship can be made of 3 special columns located at some points of a Cartesian plane such that these 3 points form a triangle equal to the ship with respect to rotations, translations (parallel shifts along some vector) and reflections (symmetries along the edges). The ships can overlap after the landing.</p><p>Each column can be used to land more than one ship, for example, if there are two equal ships, we don't need to build 6 columns to land both ships, 3 will be enough. Petya wants to know what minimum number of columns will be enough to land all ships. </p></div><div class="input-specification"><p>Each of 4 lines will contain 6 integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">3</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub> ≤ 20</span>), representing 3 points that describe the shape of each of 4 ships. It is guaranteed that 3 points in each line will represent a non-degenerate triangle.</p></div><div class="output-specification"><p>First line should contain minimum number of columns enough to land all spaceships.</p></div>

## Input

<p>Each of 4 lines will contain 6 integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">3</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">3</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub> ≤ 20</span>), representing 3 points that describe the shape of each of 4 ships. It is guaranteed that 3 points in each line will represent a non-degenerate triangle.</p>

## Output

<p>First line should contain minimum number of columns enough to land all spaceships.</p>





```input1
0 0 1 0 1 2
0 0 0 2 2 2
0 0 3 0 1 2
0 0 3 0 2 2

```




```input2
0 0 0 1 1 1
0 0 0 2 2 2
0 0 0 5 5 5
0 0 0 17 17 17

```




```output1
4

```




```output2
9

```



## Note

<p>In the first test case columns can be put in these points: <span class="tex-span">(0, 0), (1, 0), (3, 0), (1, 2)</span>. Note that the second ship can land using last 3 columns.</p><p>In the second test case following points can be chosen: <span class="tex-span">(0, 0), (0, 1), (1, 0), (0, 2), (2, 0), (0, 5), (5, 0), (0, 17), (17, 0)</span>. It is impossible to use less than 9 columns.</p>
