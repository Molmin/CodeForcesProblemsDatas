## Description

<div><p>Igor the analyst fell asleep on the work and had a strange dream. In the dream his desk was crowded with computer mice, so he bought a mousetrap to catch them.</p><p>The desk can be considered as an infinite plane, then the mousetrap is a rectangle which sides are parallel to the axes, and which opposite sides are located in points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p><p>Igor wants to catch all mice. Igor has analysed their behavior and discovered that each mouse is moving along a straight line with constant speed, the speed of the <span class="tex-span"><i>i</i></span>-th mouse is equal to <span class="tex-span">(<i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup>, <i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup>)</span>, that means that the <span class="tex-span"><i>x</i></span> coordinate of the mouse increases by <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup></span> units per second, while the <span class="tex-span"><i>y</i></span> coordinates increases by <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup></span> units. The mousetrap is open initially so that the mice are able to move freely on the desk. Igor can close the mousetrap at any moment catching all the mice that are <span class="tex-font-style-bf">strictly</span> inside the mousetrap.</p><p>Igor works a lot, so he is busy in the dream as well, and he asks you to write a program that by given mousetrap's coordinates, the initial coordinates of the mice and their speeds determines the earliest time moment in which he is able to catch all the mice. Please note that Igor can close the mousetrap only once.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of computer mice on the desk.</p><p>The second line contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ 100 000</span>), (<span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ 100 000</span>)&nbsp;— the coordinates of the opposite corners of the mousetrap.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the information about mice.</p><p>The <span class="tex-span"><i>i</i></span>-th of these lines contains four integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup></span>, (<span class="tex-span">0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup>, <i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup> ≤ 100 000</span>, <span class="tex-span"> - 100 000 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup>, <i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup> ≤ 100 000</span>), where <span class="tex-span">(<i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup>, <i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup>)</span> is the initial position of the mouse, and <span class="tex-span">(<i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup>, <i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup>)</span> is its speed.</p></div><div class="output-specification"><p>In the only line print minimum possible non-negative number <span class="tex-span"><i>t</i></span> such that if Igor closes the mousetrap at <span class="tex-span"><i>t</i></span> seconds from the beginning, then all the mice are <span class="tex-font-style-bf">strictly</span> inside the mousetrap. If there is no such <span class="tex-span"><i>t</i></span>, print <span class="tex-font-style-tt">-1</span>.</p><p>Your answer is considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://jhzLI5sw.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of computer mice on the desk.</p><p>The second line contains four integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ 100 000</span>), (<span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ 100 000</span>)&nbsp;— the coordinates of the opposite corners of the mousetrap.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the information about mice.</p><p>The <span class="tex-span"><i>i</i></span>-th of these lines contains four integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup></span>, (<span class="tex-span">0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup>, <i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup> ≤ 100 000</span>, <span class="tex-span"> - 100 000 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup>, <i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup> ≤ 100 000</span>), where <span class="tex-span">(<i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup>, <i>r</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup>)</span> is the initial position of the mouse, and <span class="tex-span">(<i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>x</i></sup>, <i>v</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index"><i>y</i></sup>)</span> is its speed.</p>

## Output

<p>In the only line print minimum possible non-negative number <span class="tex-span"><i>t</i></span> such that if Igor closes the mousetrap at <span class="tex-span"><i>t</i></span> seconds from the beginning, then all the mice are <span class="tex-font-style-bf">strictly</span> inside the mousetrap. If there is no such <span class="tex-span"><i>t</i></span>, print <span class="tex-font-style-tt">-1</span>.</p><p>Your answer is considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://jhzLI5sw.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4
7 7 9 8
3 5 7 5
7 5 2 4
3 3 7 8
6 6 3 2

```




```input2
4
7 7 9 8
0 3 -5 4
5 0 5 4
9 9 -1 -6
10 5 -7 -10

```




```output1
0.57142857142857139685

```




```output2
-1

```



## Note

<p>Here is a picture of the first sample</p><p>Points A, B, C, D - start mice positions, segments are their paths.</p><p><img class="tex-graphics" src="file://zIaZG3BA.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Then, at first time when all mice will be in rectangle it will be looks like this:</p><p><img class="tex-graphics" src="file://yAgha0Sv.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Here is a picture of the second sample</p><p><img class="tex-graphics" src="file://Y8yCo74A.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Points A, D, B will never enter rectangle.</p>
