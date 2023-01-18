## Description

<div><p>A long time ago somewhere in the depths of America existed a powerful tribe governed by the great leader Pinnie-the-Wooh. Once the tribe conquered three Maya cities. Pinnie-the-Wooh grew concerned: there had to be some control over the conquered territories. That's why he appealed to the priests of the supreme god Mogohu-Rea for help.</p><p>The priests conveyed the god's will to him: to control these three cities he should put an idol to Mogohu-Rea — that will create a religious field over the cities. However, the idol is so powerful that it can easily drive the people around it mad unless it is balanced by exactly three sacrifice altars, placed one in each city. To balance the idol the altars should be placed so that the center of mass of the system of these three points coincided with the idol. When counting the center of mass consider that all the altars have the same mass.</p><p>Now Pinnie-the-Wooh is thinking where to put the idol. He has a list of hills, that are suitable to put an idol there. Help him to identify on which of them you can put an idol without risking to fry off the brains of the cities' population with the religious field.</p><p>Each city has a shape of a convex polygon such that no three vertexes lie on a straight line. The cities can intersect. Each altar should be attached to the city through a special ceremony, besides, it must be situated on the city's territory (possibly at the border). Thus, there may be several altars on a city's territory, but exactly one of them will be attached to the city. The altars, the idol and the hills are points on the plane, some of them may coincide.</p><p>The hills are taken into consideration independently from each other, the altars' location for different hills may also be different.</p></div><div class="input-specification"><p>First follow descriptions of the three cities, divided by empty lines. The descriptions are in the following format:</p><p>The first line contains an integer <span class="tex-span"><i>n</i></span>, which represent the number of the polygon's vertexes (<span class="tex-span">3 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>). Next <span class="tex-span"><i>n</i></span> lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> each, they are the coordinates of the polygon's <span class="tex-span"><i>i</i></span>-th vertex in the counterclockwise order.</p><p>After the cities' description follows the integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), which represents the number of hills. Next <span class="tex-span"><i>m</i></span> lines each contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>, they are the coordinates of the <span class="tex-span"><i>j</i></span>-th hill.</p><p>All the coordinates in the input data do not exceed <span class="tex-span">5·10<sup class="upper-index">8</sup></span> in the absolute value.</p></div><div class="output-specification"><p>For each hill print on a single line "<span class="tex-font-style-tt">YES</span>" (without the quotes) or "<span class="tex-font-style-tt">NO</span>" (without the quotes), depending on whether the three sacrifice altars can be put to balance the idol or not.</p></div>

## Input

<p>First follow descriptions of the three cities, divided by empty lines. The descriptions are in the following format:</p><p>The first line contains an integer <span class="tex-span"><i>n</i></span>, which represent the number of the polygon's vertexes (<span class="tex-span">3 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span>). Next <span class="tex-span"><i>n</i></span> lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> each, they are the coordinates of the polygon's <span class="tex-span"><i>i</i></span>-th vertex in the counterclockwise order.</p><p>After the cities' description follows the integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), which represents the number of hills. Next <span class="tex-span"><i>m</i></span> lines each contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>, they are the coordinates of the <span class="tex-span"><i>j</i></span>-th hill.</p><p>All the coordinates in the input data do not exceed <span class="tex-span">5·10<sup class="upper-index">8</sup></span> in the absolute value.</p>

## Output

<p>For each hill print on a single line "<span class="tex-font-style-tt">YES</span>" (without the quotes) or "<span class="tex-font-style-tt">NO</span>" (without the quotes), depending on whether the three sacrifice altars can be put to balance the idol or not.</p>





```input1
3
0 0
1 0
1 1

4
8 8
5 5
6 4
8 4

3
-1 -1
-3 -1
-2 -2

5
0 0
2 1
7 1
1 1
5 3

```




```output1
NO
YES
NO
YES
NO

```



## Note

<p>For the hill at <span class="tex-span">(2, 1)</span> the altars can be placed at the points <span class="tex-span">(1, 0), (7, 5), ( - 2,  - 2)</span>, for the hill at <span class="tex-span">(1, 1)</span> — at the points <span class="tex-span">(0, 0), (6, 4), ( - 3,  - 1)</span>. Many other groups of three points can do the trick. There are no suitable points for other hills.</p>
