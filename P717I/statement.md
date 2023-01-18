## Description

<div><p>Cowboy Beblop is a funny little boy who likes sitting at his computer. He somehow obtained two elastic hoops in the shape of 2D polygons, which are not necessarily convex. Since there's no gravity on his spaceship, the hoops are standing still in the air. Since the hoops are very elastic, Cowboy Beblop can stretch, rotate, translate or shorten their edges as much as he wants.</p><p>For both hoops, you are given the number of their vertices, as well as the position of each vertex, defined by the X , Y and Z coordinates. The vertices are given in the order they're connected: the 1st vertex is connected to the 2nd, which is connected to the 3rd, etc., and the last vertex is connected to the first one. Two hoops are connected if it's impossible to pull them to infinity in different directions by manipulating their edges, without having their edges or vertices intersect at any point – <span class="tex-font-style-bf">just like when two links of a chain are connected</span>. <span class="tex-font-style-bf">The polygons' edges do not intersect or overlap</span>. </p><p>To make things easier, we say that two polygons are <span class="tex-font-style-bf">well-connected</span>, if the edges of one polygon cross the area of the other polygon in two different directions (from the upper and lower sides of the plane defined by that polygon) a different number of times.</p><p>Cowboy Beblop is fascinated with the hoops he has obtained and he would like to know whether they are well-connected or not. Since he’s busy playing with his dog, Zwei, he’d like you to figure it out for him. He promised you some sweets if you help him! </p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000</span>), which denotes the number of edges of the first polygon. The next N lines each contain the integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span"> - 1 000 000 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 1 000 000</span>)&nbsp;— coordinates of the vertices, in the manner mentioned above. The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>m</i> ≤ 100 000</span>) , denoting the number of edges of the second polygon, followed by <span class="tex-span"><i>m</i></span> lines containing the coordinates of the second polygon’s vertices.</p><p>It is guaranteed that both polygons are simple (no self-intersections), and in general that <span class="tex-font-style-bf">the obtained polygonal lines do not intersect each other</span>. Also, you can assume that no 3 consecutive points of a polygon lie on the same line.</p></div><div class="output-specification"><p>Your output should contain only one line, with the words "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", depending on whether the two given polygons are well-connected. </p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000</span>), which denotes the number of edges of the first polygon. The next N lines each contain the integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span"> - 1 000 000 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 1 000 000</span>)&nbsp;— coordinates of the vertices, in the manner mentioned above. The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>m</i> ≤ 100 000</span>) , denoting the number of edges of the second polygon, followed by <span class="tex-span"><i>m</i></span> lines containing the coordinates of the second polygon’s vertices.</p><p>It is guaranteed that both polygons are simple (no self-intersections), and in general that <span class="tex-font-style-bf">the obtained polygonal lines do not intersect each other</span>. Also, you can assume that no 3 consecutive points of a polygon lie on the same line.</p>

## Output

<p>Your output should contain only one line, with the words "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", depending on whether the two given polygons are well-connected. </p>





```input1
4
0 0 0
2 0 0
2 2 0
0 2 0
4
1 1 -1
1 1 1
1 3 1
1 3 -1

```




```output1
YES

```



## Note

<p>On the picture below, the two polygons are well-connected, as the edges of the vertical polygon cross the area of the horizontal one exactly once in one direction (for example, from above to below), and zero times in the other (in this case, from below to above). Note that the polygons do not have to be parallel to any of the xy-,xz-,yz- planes in general. <img class="tex-graphics" src="file://MCqG3p0R.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
