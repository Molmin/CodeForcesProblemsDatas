## Description

<div><p>Arkady reached the <span class="tex-span"><i>n</i></span>-th level in Township game, so Masha decided to bake a pie for him! Of course, the pie has a shape of convex <span class="tex-span"><i>n</i></span>-gon, i.e. a polygon with <span class="tex-span"><i>n</i></span> vertices.</p><p>Arkady decided to cut the pie in two equal in area parts by cutting it by a straight line, so that he can eat one of them and give the other to Masha. There is a difficulty because Arkady has already put a knife at some point of the pie, so he now has to cut the pie by a straight line passing trough this point.</p><p>Help Arkady: find a line that passes through the point Arkady has put a knife into and cuts the pie into two parts of equal area, or determine that it's impossible. Your program has to quickly answer many queries with the same pie, but different points in which Arkady puts a knife.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in the pie and the number of queries.</p><p><span class="tex-span"><i>n</i></span> line follow describing the polygon vertices in clockwise order. The <span class="tex-span"><i>i</i></span>-th of these line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex. It is guaranteed that the polygon is strictly convex, in particular, no three vertices line on the same line.</p><p>An empty line follows.</p><p><span class="tex-span"><i>q</i></span> lines follow describing the query points. The <span class="tex-span"><i>i</i></span>-th of these lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the coordinates of the point in which Arkady puts the knife in the <span class="tex-span"><i>i</i></span>-th query. In is guaranteed that in each query the given point is strictly inside the polygon, in particular, is not on its edges.</p></div><div class="output-specification"><p>For each query print single integer&nbsp;— the polar angle of the line that is the answer for the corresponding query, in radians. The angle should be in the segment <span class="tex-span">[0;π]</span>, the angles are measured from the direction of <span class="tex-span"><i>OX</i></span> axis in counter-clockwise order. For example, the polar angle of the <span class="tex-span"><i>OY</i></span> axis is <img align="middle" class="tex-formula" src="file://tagnzxiA.png" style="max-width: 100.0%;max-height: 100.0%;">. If there is no answer in that query, print <span class="tex-font-style-tt">-1</span>.</p><p>If there are several answers, print any of them. Your answer is considered correct if the difference between the areas of the parts divided by the total area of the polygon doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> by absolute value. In other words, if <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are the areas of the parts after the cut, then your answer is correct if and only of <img align="middle" class="tex-formula" src="file://i7114hyk.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in the pie and the number of queries.</p><p><span class="tex-span"><i>n</i></span> line follow describing the polygon vertices in clockwise order. The <span class="tex-span"><i>i</i></span>-th of these line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex. It is guaranteed that the polygon is strictly convex, in particular, no three vertices line on the same line.</p><p>An empty line follows.</p><p><span class="tex-span"><i>q</i></span> lines follow describing the query points. The <span class="tex-span"><i>i</i></span>-th of these lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the coordinates of the point in which Arkady puts the knife in the <span class="tex-span"><i>i</i></span>-th query. In is guaranteed that in each query the given point is strictly inside the polygon, in particular, is not on its edges.</p>

## Output

<p>For each query print single integer&nbsp;— the polar angle of the line that is the answer for the corresponding query, in radians. The angle should be in the segment <span class="tex-span">[0;π]</span>, the angles are measured from the direction of <span class="tex-span"><i>OX</i></span> axis in counter-clockwise order. For example, the polar angle of the <span class="tex-span"><i>OY</i></span> axis is <img align="middle" class="tex-formula" src="file://tagnzxiA.png" style="max-width: 100.0%;max-height: 100.0%;">. If there is no answer in that query, print <span class="tex-font-style-tt">-1</span>.</p><p>If there are several answers, print any of them. Your answer is considered correct if the difference between the areas of the parts divided by the total area of the polygon doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> by absolute value. In other words, if <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are the areas of the parts after the cut, then your answer is correct if and only of <img align="middle" class="tex-formula" src="file://i7114hyk.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 1
0 0
0 3
3 0

1 1

```




```input2
5 3
6 5
6 3
5 0
0 0
0 5

5 4
3 3
5 2

```




```output1
2.67794504460098710000

```




```output2
0.60228734612690049000
1.27933953226473580000
2.85805511179015910000

```


