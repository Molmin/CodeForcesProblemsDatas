## Description

<div><p>Barney has finally found the one, a beautiful young lady named Lyanna. The problem is, Lyanna and Barney are trapped in Lord Loss' castle. This castle has shape of a convex polygon of <span class="tex-span"><i>n</i></span> points. Like most of castles in Demonata worlds, this castle has no ceiling.</p><center> <img class="tex-graphics" src="file://QpYDRFuq.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Barney and Lyanna have an escape plan, but it requires some geometry knowledge, so they asked for your help.</p><p>Barney knows that demons are organized and move in lines. He and Lyanna want to wait for the appropriate time so they need to watch for the demons. Each of them wants to stay in a point <span class="tex-font-style-bf">inside the castle</span> (possibly on edges or corners), also they may stay in the same position. They both want to pick a real number <span class="tex-span"><i>r</i></span> and watch all points in the circles with radius <span class="tex-span"><i>r</i></span> around each of them (these two circles may overlap).</p><center> <img class="tex-graphics" src="file://KlJKEYPY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>We say that Barney and Lyanna are <span class="tex-font-style-it">watching carefully</span> if and only if for every edge of the polygon, at least one of them can see at least one point on the line this edge lies on, thus such point may not be on the edge but it should be on edge's line. Formally, each edge line should have at least one common point with at least one of two circles.</p><p>The greater <span class="tex-span"><i>r</i></span> is, the more energy and focus they need. So they asked you to tell them the minimum value of <span class="tex-span"><i>r</i></span> such that they can watch carefully.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 300</span>)&nbsp;— the number of castle polygon vertices.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe the polygon vertices in counter-clockwise order. <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— the coordinates of <span class="tex-span"><i>i</i></span>-th point of the castle. It is guaranteed that given points form a convex polygon, in particular, any three of them do not line on the same line.</p></div><div class="output-specification"><p>In the first line print the single number <span class="tex-span"><i>r</i></span>&nbsp;— minimum radius of guys' watching circles.</p><p>In the second line print the pair of coordinates of point where Barney should stay.</p><p>In the third line print the pair of coordinates of point where Lyanna should stay.</p><p>Points should lie inside the polygon.</p><p>Coordinates may not be integers. If there are multiple answers print any of them.</p><p>Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 300</span>)&nbsp;— the number of castle polygon vertices.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe the polygon vertices in counter-clockwise order. <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">4</sup></span>)&nbsp;— the coordinates of <span class="tex-span"><i>i</i></span>-th point of the castle. It is guaranteed that given points form a convex polygon, in particular, any three of them do not line on the same line.</p>

## Output

<p>In the first line print the single number <span class="tex-span"><i>r</i></span>&nbsp;— minimum radius of guys' watching circles.</p><p>In the second line print the pair of coordinates of point where Barney should stay.</p><p>In the third line print the pair of coordinates of point where Lyanna should stay.</p><p>Points should lie inside the polygon.</p><p>Coordinates may not be integers. If there are multiple answers print any of them.</p><p>Your answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
4
-41 67
-16 20
25 25
-36 85

```




```input2
7
-7 54
-5 31
-2 17
20 19
32 23
34 27
26 57

```




```output1
0
-16 20
-36 85

```




```output2
2.9342248
32.019503 23.0390067
-6.929116 54.006444

```



## Note

<p>In the first example guys can stay in opposite corners of the castle.</p>
