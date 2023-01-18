## Description

<div><p>So nearly half of the winter is over and Maria is dreaming about summer. She's fed up with skates and sleds, she was dreaming about Hopscotch all night long. It's a very popular children's game. The game field, the court, looks as is shown in the figure (all blocks are square and are numbered from bottom to top, blocks in the same row are numbered from left to right). Let us describe the hopscotch with numbers that denote the number of squares in the row, staring from the lowest one: 1-1-2-1-2-1-2-(1-2)..., where then the period is repeated (1-2).</p><center> <img class="tex-graphics" height="189px" src="file://Vvb29nob.png" style="max-width: 100.0%;max-height: 100.0%;" width="227px"> </center><p>The coordinate system is defined as shown in the figure. Side of all the squares are equal and have length <span class="tex-span"><i>a</i></span>.</p><p>Maria is a very smart and clever girl, and she is concerned with quite serious issues: if she throws a stone into a point with coordinates <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, then will she hit some square? If the answer is positive, you are also required to determine the number of the square.</p><p>It is believed that the stone has fallen into the square if it is located <span class="tex-font-style-bf">strictly</span> inside it. In other words a stone that has fallen on the square border is not considered a to hit a square.</p></div><div class="input-specification"><p>The only input line contains three integers: <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, where <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 100</span>) is the side of the square, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>y</i> ≤ 10<sup class="upper-index">6</sup></span>) are coordinates of the stone.</p></div><div class="output-specification"><p>Print the number of the square, inside which the stone fell. If the stone is on a border of some stone or outside the court, print "<span class="tex-font-style-tt">-1</span>" without the quotes.</p></div>

## Input

<p>The only input line contains three integers: <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, where <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 100</span>) is the side of the square, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>y</i> ≤ 10<sup class="upper-index">6</sup></span>) are coordinates of the stone.</p>

## Output

<p>Print the number of the square, inside which the stone fell. If the stone is on a border of some stone or outside the court, print "<span class="tex-font-style-tt">-1</span>" without the quotes.</p>





```input1
1 0 0

```




```input2
3 1 1

```




```input3
3 0 10

```




```input4
3 0 7

```




```input5
3 4 0

```




```output1
-1

```




```output2
1

```




```output3
5

```




```output4
-1

```




```output5
-1

```


