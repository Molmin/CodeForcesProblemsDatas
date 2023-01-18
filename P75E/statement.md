## Description

<div><p>You have got a new job, and it's very interesting, you are a ship captain. Your first task is to move your ship from one point to another point, and for sure you want to move it at the minimum cost.</p><p>And it's well known that the shortest distance between any 2 points is the length of the line segment between these 2 points. But unfortunately there is an island in the sea, so sometimes you won't be able to move your ship in the line segment between the 2 points.</p><p>You can <span class="tex-font-style-bf">only</span> move to safe points. A point is called safe if it's on the line segment between the start and end points, or if it's on the island's edge.</p><p>But you are too lucky, you have got some clever and strong workers and they can help you in your trip, they can help you move the ship in the sea and they will take 1 Egyptian pound for each moving unit in the sea, and they can carry the ship (yes, they are very strong) and walk on the island and they will take 2 Egyptian pounds for each moving unit in the island. The money which you will give to them will be divided between all workers, so the number of workers does not matter here.</p><p>You can move your ship on the island edge, and it will be considered moving in the sea.</p><p>Now you have a sea map, and you have to decide what is the minimum cost for your trip.</p><p>Your starting point is (<span class="tex-span"><i>xStart</i></span>, <span class="tex-span"><i>yStart</i></span>), and the end point is (<span class="tex-span"><i>xEnd</i></span>, <span class="tex-span"><i>yEnd</i></span>), both points will be different.</p><p>The island will be a convex polygon and there will be no more than 2 polygon points on the same line, also the starting and the end points won't be inside or on the boundary of the island. The points for the polygon will be given in the anti-clockwise order.</p></div><div class="input-specification"><p>The first line contains 4 integers, <span class="tex-span"><i>xStart</i></span>, <span class="tex-span"><i>yStart</i></span>, <span class="tex-span"><i>xEnd</i></span> and <span class="tex-span"><i>yEnd</i></span> (<span class="tex-span"> - 100 ≤ <i>xStart</i>, <i>yStart</i>, <i>xEnd</i>, <i>yEnd</i> ≤ 100</span>). The second line contains an integer <span class="tex-span"><i>n</i></span>, which is the number of points in the polygon (<span class="tex-span">3 ≤ <i>n</i> ≤ 30</span>), followed by a line containing <span class="tex-span"><i>n</i></span> pairs of integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, which are the coordinates of the points (<span class="tex-span"> - 100 ≤ <i>x</i>, <i>y</i> ≤ 100</span>), the polygon points will be distinct.</p></div><div class="output-specification"><p>Print one line which contains the minimum possible cost. The absolute or relative error in the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains 4 integers, <span class="tex-span"><i>xStart</i></span>, <span class="tex-span"><i>yStart</i></span>, <span class="tex-span"><i>xEnd</i></span> and <span class="tex-span"><i>yEnd</i></span> (<span class="tex-span"> - 100 ≤ <i>xStart</i>, <i>yStart</i>, <i>xEnd</i>, <i>yEnd</i> ≤ 100</span>). The second line contains an integer <span class="tex-span"><i>n</i></span>, which is the number of points in the polygon (<span class="tex-span">3 ≤ <i>n</i> ≤ 30</span>), followed by a line containing <span class="tex-span"><i>n</i></span> pairs of integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, which are the coordinates of the points (<span class="tex-span"> - 100 ≤ <i>x</i>, <i>y</i> ≤ 100</span>), the polygon points will be distinct.</p>

## Output

<p>Print one line which contains the minimum possible cost. The absolute or relative error in the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
1 7 6 7
4
4 2 4 12 3 12 3 2

```




```input2
-1 0 2 0
4
0 0 1 0 1 1 0 1

```




```output1
6.000000000

```




```output2
3.000000000

```


