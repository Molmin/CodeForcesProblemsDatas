## Description

<div><p>Bertown is under siege! The attackers have blocked all the ways out and their cannon is bombarding the city. Fortunately, Berland intelligence managed to intercept the enemies' shooting plan. Let's introduce the Cartesian system of coordinates, the origin of which coincides with the cannon's position, the <span class="tex-span"><i>Ox</i></span> axis is directed rightwards in the city's direction, the <span class="tex-span"><i>Oy</i></span> axis is directed upwards (to the sky). The cannon will make <span class="tex-span"><i>n</i></span> more shots. The cannon balls' initial speeds are the same in all the shots and are equal to <span class="tex-span"><i>V</i></span>, so that every shot is characterized by only one number <span class="tex-span"><i>alpha</i><sub class="lower-index"><i>i</i></sub></span> which represents the angle at which the cannon fires. Due to the cannon's technical peculiarities this angle does not exceed <span class="tex-span">45</span> angles (<span class="tex-span">π / 4</span>). We disregard the cannon sizes and consider the firing made from the point <span class="tex-span">(0, 0)</span>.</p><p>The balls fly according to the known physical laws of a body thrown towards the horizon at an angle: </p><center class="tex-equation"><span class="tex-span"><i>v</i><sub class="lower-index"><i>x</i></sub>(<i>t</i>) = <i>V</i>·<i>cos</i>(<i>alpha</i>)</span></center> <center class="tex-equation"><span class="tex-span"><i>v</i><sub class="lower-index"><i>y</i></sub>(<i>t</i>) = <i>V</i>·<i>sin</i>(<i>alpha</i>)&nbsp; – &nbsp;<i>g</i>·<i>t</i></span></center> <center class="tex-equation"><span class="tex-span"><i>x</i>(<i>t</i>) = <i>V</i>·<i>cos</i>(<i>alpha</i>)·<i>t</i></span></center> <center class="tex-equation"><span class="tex-span"><i>y</i>(<i>t</i>) = <i>V</i>·<i>sin</i>(<i>alpha</i>)·<i>t</i>&nbsp; – &nbsp;<i>g</i>·<i>t</i><sup class="upper-index">2</sup> / 2</span></center><p>Think of the acceleration of gravity <span class="tex-span"><i>g</i></span> as equal to <span class="tex-span">9.8</span>.</p><p>Bertown defends <span class="tex-span"><i>m</i></span> walls. The <span class="tex-span"><i>i</i></span>-th wall is represented as a vertical segment <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, 0) - (<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. When a ball hits a wall, it gets stuck in it and doesn't fly on. If a ball doesn't hit any wall it falls on the ground (<span class="tex-span"><i>y</i> = 0</span>) and stops. If the ball exactly hits the point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, it is considered stuck. </p><p>Your task is to find for each ball the coordinates of the point where it will be located in the end.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>V</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>, 1 ≤ <i>V</i> ≤ 1000</span>) which represent the number of shots and the initial speed of every ball. The second line contains <span class="tex-span"><i>n</i></span> space-separated real numbers <span class="tex-span"><i>alpha</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 &lt; <i>alpha</i><sub class="lower-index"><i>i</i></sub> &lt; π / 4</span>) which represent the angles in radians at which the cannon will fire. The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) which represents the number of walls. Then follow <span class="tex-span"><i>m</i></span> lines, each containing two real numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, 0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) which represent the wall’s coordinates. All the real numbers have no more than 4 decimal digits. The walls may partially overlap or even coincide.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines containing two real numbers each — calculate for every ball the coordinates of its landing point. Your answer should have the relative or absolute error less than <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>V</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>, 1 ≤ <i>V</i> ≤ 1000</span>) which represent the number of shots and the initial speed of every ball. The second line contains <span class="tex-span"><i>n</i></span> space-separated real numbers <span class="tex-span"><i>alpha</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 &lt; <i>alpha</i><sub class="lower-index"><i>i</i></sub> &lt; π / 4</span>) which represent the angles in radians at which the cannon will fire. The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) which represents the number of walls. Then follow <span class="tex-span"><i>m</i></span> lines, each containing two real numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, 0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) which represent the wall’s coordinates. All the real numbers have no more than 4 decimal digits. The walls may partially overlap or even coincide.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines containing two real numbers each — calculate for every ball the coordinates of its landing point. Your answer should have the relative or absolute error less than <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
2 10
0.7853
0.3
3
5.0 5.0
4.0 2.4
6.0 1.9

```




```input2
2 10
0.7853
0.3
2
4.0 2.4
6.0 1.9

```




```output1
5.000000000 2.549499369
4.000000000 0.378324889

```




```output2
10.204081436 0.000000000
4.000000000 0.378324889

```


