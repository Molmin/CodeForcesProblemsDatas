## Description

<div><p>Petya has recently started working as a programmer in the IT city company that develops computer games.</p><p>Besides game mechanics implementation to create a game it is necessary to create tool programs that can be used by game designers to create game levels. Petya's first assignment is to create a tool that allows to paint different arrows on the screen.</p><p>A user of this tool will choose a point on the screen, specify a vector (the arrow direction) and vary several parameters to get the required graphical effect. In the first version of the program Petya decided to limit parameters of the arrow by the following: a point with coordinates <span class="tex-span">(<i>px</i>, <i>py</i>)</span>, a nonzero vector with coordinates <span class="tex-span">(<i>vx</i>, <i>vy</i>)</span>, positive scalars <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>, <i>a</i> &gt; <i>c</i></span>.</p><p>The produced arrow should have the following properties. The arrow consists of a triangle and a rectangle. The triangle is isosceles with base of length <span class="tex-span"><i>a</i></span> and altitude of length <span class="tex-span"><i>b</i></span> perpendicular to the base. The rectangle sides lengths are <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span>. Point <span class="tex-span">(<i>px</i>, <i>py</i>)</span> is situated in the middle of the triangle base and in the middle of side of rectangle that has length <span class="tex-span"><i>c</i></span>. Area of intersection of the triangle and the rectangle is zero. The direction from <span class="tex-span">(<i>px</i>, <i>py</i>)</span> point to the triangle vertex opposite to base containing the point coincides with direction of <span class="tex-span">(<i>vx</i>, <i>vy</i>)</span> vector.</p><p>Enumerate the arrow points coordinates in counter-clockwise order starting from the tip.</p><center> <img class="tex-graphics" src="file://aavBVPSY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The only line of the input contains eight integers <span class="tex-span"><i>px</i>, <i>py</i>, <i>vx</i>, <i>vy</i></span> (<span class="tex-span"> - 1000 ≤ <i>px</i>, <i>py</i>, <i>vx</i>, <i>vy</i> ≤ 1000, <i>vx</i><sup class="upper-index">2</sup> + <i>vy</i><sup class="upper-index">2</sup> &gt; 0</span>), <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ 1000, <i>a</i> &gt; <i>c</i></span>).</p></div><div class="output-specification"><p>Output coordinates of the arrow points in counter-clockwise order. Each line should contain two coordinates, first <span class="tex-span"><i>x</i></span>, then <span class="tex-span"><i>y</i></span>. Relative or absolute error should not be greater than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The only line of the input contains eight integers <span class="tex-span"><i>px</i>, <i>py</i>, <i>vx</i>, <i>vy</i></span> (<span class="tex-span"> - 1000 ≤ <i>px</i>, <i>py</i>, <i>vx</i>, <i>vy</i> ≤ 1000, <i>vx</i><sup class="upper-index">2</sup> + <i>vy</i><sup class="upper-index">2</sup> &gt; 0</span>), <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, <i>d</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ 1000, <i>a</i> &gt; <i>c</i></span>).</p>

## Output

<p>Output coordinates of the arrow points in counter-clockwise order. Each line should contain two coordinates, first <span class="tex-span"><i>x</i></span>, then <span class="tex-span"><i>y</i></span>. Relative or absolute error should not be greater than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
8 8 0 2 8 3 4 5

```




```output1
8.000000000000 11.000000000000
4.000000000000 8.000000000000
6.000000000000 8.000000000000
6.000000000000 3.000000000000
10.000000000000 3.000000000000
10.000000000000 8.000000000000
12.000000000000 8.000000000000

```


