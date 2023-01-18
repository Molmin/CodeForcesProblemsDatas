## Description

<div><p>A coder cannot sit and code all day. Sometimes it is a good idea to rise from the desk, have a rest, have small talk with colleagues and even play. The coders of the F company have their favorite ball game.</p><p>Let's imagine the game on the plane with a cartesian coordinate system. The point (0, 0) contains the player who chooses an arbitrary direction and throws a ball in that direction. The ball hits the plane at distance <span class="tex-span"><i>d</i></span> from the player's original position and continues flying in the same direction. After the ball hits the plane for the first time, it flies on and hits the plane again at distance <span class="tex-span">2·<i>d</i></span> from the player's original position and so on (it continue flying in the chosen direction and hitting the plane after each <span class="tex-span"><i>d</i></span> units). All coders in the F company are strong, so the ball flies infinitely far away.</p><p>The plane has <span class="tex-span"><i>n</i></span> circles painted on it. If a ball hits the plane and hits a circle that is painted on the plane (including its border), then the player gets one point. The ball can hit multiple circles at once and get one point for each of them (if the ball hits some circle <span class="tex-span"><i>x</i></span> times during the move, the player also gets <span class="tex-span"><i>x</i></span> points). Count the maximum number of points a player can get if he throws a ball in the arbitrary direction. Note that the direction may have real cooridinates.</p></div><div class="input-specification"><p>The first line contains two space-separated integers — <span class="tex-span"><i>n</i></span> и <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">4</sup>;&nbsp;5 ≤ <i>d</i> ≤ 10)</span>. Next <span class="tex-span"><i>n</i></span> lines contain the circles' description. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 10000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10000;&nbsp;1 ≤ <i>r</i> ≤ 50)</span>, where <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> are the coordinates of the center and the radius of the circle, correspondingly. The point (0, 0) is not inside or on the border of some circle.</p></div><div class="output-specification"><p>Print a single integer — the maximum number of points you can get.</p></div>

## Input

<p>The first line contains two space-separated integers — <span class="tex-span"><i>n</i></span> и <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">4</sup>;&nbsp;5 ≤ <i>d</i> ≤ 10)</span>. Next <span class="tex-span"><i>n</i></span> lines contain the circles' description. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 10000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10000;&nbsp;1 ≤ <i>r</i> ≤ 50)</span>, where <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> are the coordinates of the center and the radius of the circle, correspondingly. The point (0, 0) is not inside or on the border of some circle.</p>

## Output

<p>Print a single integer — the maximum number of points you can get.</p>





```input1
2 5
1 1 1
5 0 1

```




```input2
2 5
4 0 3
5 3 1

```




```input3
1 10
20 0 10

```




```output1
1

```




```output2
2

```




```output3
3

```


