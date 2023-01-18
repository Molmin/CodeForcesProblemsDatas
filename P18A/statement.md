## Description

<div><p>At a geometry lesson Bob learnt that a triangle is called right-angled if it is nondegenerate and one of its angles is right. Bob decided to draw such a triangle immediately: on a sheet of paper he drew three points with integer coordinates, and joined them with segments of straight lines, then he showed the triangle to Peter. Peter said that Bob's triangle is not right-angled, but is <span class="tex-font-style-underline">almost</span> right-angled: the triangle itself is not right-angled, but it is possible to move one of the points exactly by distance 1 so, that all the coordinates remain integer, and the triangle become right-angled. Bob asks you to help him and find out if Peter tricks him. By the given coordinates of the triangle you should find out if it is right-angled, almost right-angled, or neither of these.</p></div><div class="input-specification"><p>The first input line contains 6 space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub></span> — coordinates of the triangle's vertices. All the coordinates are integer and don't exceed 100 in absolute value. It's guaranteed that the triangle is nondegenerate, i.e. its total area is not zero.</p></div><div class="output-specification"><p>If the given triangle is right-angled, output <span class="tex-font-style-tt">RIGHT</span>, if it is almost right-angled, output <span class="tex-font-style-tt">ALMOST</span>, and if it is neither of these, output <span class="tex-font-style-tt">NEITHER</span>.</p></div>

## Input

<p>The first input line contains 6 space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub></span> — coordinates of the triangle's vertices. All the coordinates are integer and don't exceed 100 in absolute value. It's guaranteed that the triangle is nondegenerate, i.e. its total area is not zero.</p>

## Output

<p>If the given triangle is right-angled, output <span class="tex-font-style-tt">RIGHT</span>, if it is almost right-angled, output <span class="tex-font-style-tt">ALMOST</span>, and if it is neither of these, output <span class="tex-font-style-tt">NEITHER</span>.</p>





```input1
0 0 2 0 0 1

```




```input2
2 3 4 5 6 6

```




```input3
-1 0 2 0 0 1

```




```output1
RIGHT

```




```output2
NEITHER

```




```output3
ALMOST

```


