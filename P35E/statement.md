## Description

<div><p>No Great Victory anniversary in Berland has ever passed without the war parade. This year is not an exception. That’s why the preparations are on in full strength. Tanks are building a line, artillery mounts are ready to fire, soldiers are marching on the main square... And the air forces general Mr. Generalov is in trouble again. This year a lot of sky-scrapers have been built which makes it difficult for the airplanes to fly above the city. It was decided that the planes should fly strictly from south to north. Moreover, there must be no sky scraper on a plane’s route, otherwise the anniversary will become a tragedy. The Ministry of Building gave the data on <span class="tex-span"><i>n</i></span> sky scrapers (the rest of the buildings are rather small and will not be a problem to the planes). When looking at the city from south to north as a geometrical plane, the <span class="tex-span"><i>i</i></span>-th building is a rectangle of height <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. Its westernmost point has the x-coordinate of <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and the easternmost — of <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. The terrain of the area is plain so that all the buildings stand on one level. Your task as the Ministry of Defence’s head programmer is to find an <span class="tex-font-style-it">enveloping</span> polyline using the data on the sky-scrapers. The polyline’s properties are as follows:</p><ul> <li> If you look at the city from south to north as a plane, then any part of any building will be inside or on the boarder of the area that the polyline encloses together with the land surface. </li><li> The polyline starts and ends on the land level, i.e. at the height equal to 0. </li><li> The segments of the polyline are parallel to the coordinate axes, i.e. they can only be vertical or horizontal. </li><li> The polyline’s vertices should have integer coordinates. </li><li> If you look at the city from south to north the polyline (together with the land surface) must enclose the minimum possible area. </li><li> The polyline must have the smallest length among all the polylines, enclosing the minimum possible area with the land. </li><li> The consecutive segments of the polyline must be perpendicular. </li></ul><center> <img class="tex-graphics" height="151px" src="file://KER9Nnun.png" style="max-width: 100.0%;max-height: 100.0%;" width="680px"> </center><center> Picture to the second sample test (the enveloping polyline is marked on the right). </center></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>). Then follow <span class="tex-span"><i>n</i></span> lines, each containing three integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>,  - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>In the first line output integer <span class="tex-span"><i>m</i></span> — amount of vertices of the enveloping polyline. The next <span class="tex-span"><i>m</i></span> lines should contain 2 integers each — the position and the height of the polyline’s vertex. Output the coordinates of each vertex in the order of traversing the polyline from west to east. Remember that the first and the last vertices of the polyline should have the height of 0.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>). Then follow <span class="tex-span"><i>n</i></span> lines, each containing three integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>,  - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>In the first line output integer <span class="tex-span"><i>m</i></span> — amount of vertices of the enveloping polyline. The next <span class="tex-span"><i>m</i></span> lines should contain 2 integers each — the position and the height of the polyline’s vertex. Output the coordinates of each vertex in the order of traversing the polyline from west to east. Remember that the first and the last vertices of the polyline should have the height of 0.</p>





```input1
2
3 0 2
4 1 3

```




```input2
5
3 -3 0
2 -1 1
4 2 4
2 3 7
3 6 8

```




```output1
6
0 0
0 3
1 3
1 4
3 4
3 0

```




```output2
14
-3 0
-3 3
0 3
0 2
1 2
1 0
2 0
2 4
4 4
4 2
6 2
6 3
8 3
8 0

```


