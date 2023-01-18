## Description

<div><p>When Valera was playing football on a stadium, it suddenly began to rain. Valera hid in the corridor under the grandstand not to get wet. However, the desire to play was so great that he decided to train his hitting the ball right in this corridor. Valera went back far enough, put the ball and hit it. The ball bounced off the walls, the ceiling and the floor corridor and finally hit the exit door. As the ball was wet, it left a spot on the door. Now Valera wants to know the coordinates for this spot.</p><p>Let's describe the event more formally. The ball will be considered a point in space. The door of the corridor will be considered a rectangle located on plane <span class="tex-span"><i>xOz</i></span>, such that the lower left corner of the door is located at point <span class="tex-span">(0, 0, 0)</span>, and the upper right corner is located at point <span class="tex-span">(<i>a</i>, 0, <i>b</i>)</span> . The corridor will be considered as a rectangular parallelepiped, infinite in the direction of increasing coordinates of <span class="tex-span"><i>y</i></span>. In this corridor the floor will be considered as plane <span class="tex-span"><i>xOy</i></span>, and the ceiling as plane, parallel to <span class="tex-span"><i>xOy</i></span> and passing through point <span class="tex-span">(<i>a</i>, 0, <i>b</i>)</span>. We will also assume that one of the walls is plane <span class="tex-span"><i>yOz</i></span>, and the other wall is plane, parallel to <span class="tex-span"><i>yOz</i></span> and passing through point <span class="tex-span">(<i>a</i>, 0, <i>b</i>)</span>.</p><p>We'll say that the ball hit the door when its coordinate <span class="tex-span"><i>y</i></span> was equal to <span class="tex-span">0</span>. Thus the coordinates of the spot are point <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, 0, <i>z</i><sub class="lower-index">0</sub>)</span>, where <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">0</sub> ≤ <i>a</i>, 0 ≤ <i>z</i><sub class="lower-index">0</sub> ≤ <i>b</i></span>. To hit the ball, Valera steps away from the door at distance <span class="tex-span"><i>m</i></span> and puts the ball in the center of the corridor at point <img align="middle" class="tex-formula" src="file://SiIVhQii.png" style="max-width: 100.0%;max-height: 100.0%;">. After the hit the ball flies at speed <span class="tex-span">(<i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>, <i>v</i><sub class="lower-index"><i>z</i></sub>)</span>. This means that if the ball has coordinates <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>)</span>, then after one second it will have coordinates <span class="tex-span">(<i>x</i> + <i>v</i><sub class="lower-index"><i>x</i></sub>, <i>y</i> + <i>v</i><sub class="lower-index"><i>y</i></sub>, <i>z</i> + <i>v</i><sub class="lower-index"><i>z</i></sub>)</span>.</p><p>See image in notes for clarification.</p><p>When the ball collides with the ceiling, the floor or a wall of the corridor, it bounces off in accordance with the laws of reflection (the angle of incidence equals the angle of reflection). In the problem we consider the ideal physical model, so we can assume that there is no air resistance, friction force, or any loss of energy.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i>, <i>m</i> ≤ 100)</span>. The first two integers specify point <span class="tex-span">(<i>a</i>, 0, <i>b</i>)</span>, through which the ceiling and one of the corridor walls pass. The third integer is the distance at which Valera went away from the door.</p><p>The second line has three space-separated integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>, <i>v</i><sub class="lower-index"><i>z</i></sub></span> <span class="tex-span">(|<i>v</i><sub class="lower-index"><i>x</i></sub>|, |<i>v</i><sub class="lower-index"><i>y</i></sub>|, |<i>v</i><sub class="lower-index"><i>z</i></sub>| ≤ 100, <i>v</i><sub class="lower-index"><i>y</i></sub> &lt; 0, <i>v</i><sub class="lower-index"><i>z</i></sub> ≥ 0)</span> — the speed of the ball after the hit.</p><p>It is guaranteed that the ball hits the door.</p></div><div class="output-specification"><p>Print two real numbers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>z</i><sub class="lower-index">0</sub></span> — the <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>z</i></span> coordinates of point <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, 0, <i>z</i><sub class="lower-index">0</sub>)</span>, at which the ball hits the exit door. The answer will be considered correct, if its absolute or relative error does not exceed <span class="tex-span">10 <sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i>, <i>m</i> ≤ 100)</span>. The first two integers specify point <span class="tex-span">(<i>a</i>, 0, <i>b</i>)</span>, through which the ceiling and one of the corridor walls pass. The third integer is the distance at which Valera went away from the door.</p><p>The second line has three space-separated integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>x</i></sub>, <i>v</i><sub class="lower-index"><i>y</i></sub>, <i>v</i><sub class="lower-index"><i>z</i></sub></span> <span class="tex-span">(|<i>v</i><sub class="lower-index"><i>x</i></sub>|, |<i>v</i><sub class="lower-index"><i>y</i></sub>|, |<i>v</i><sub class="lower-index"><i>z</i></sub>| ≤ 100, <i>v</i><sub class="lower-index"><i>y</i></sub> &lt; 0, <i>v</i><sub class="lower-index"><i>z</i></sub> ≥ 0)</span> — the speed of the ball after the hit.</p><p>It is guaranteed that the ball hits the door.</p>

## Output

<p>Print two real numbers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>z</i><sub class="lower-index">0</sub></span> — the <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>z</i></span> coordinates of point <span class="tex-span">(<i>x</i><sub class="lower-index">0</sub>, 0, <i>z</i><sub class="lower-index">0</sub>)</span>, at which the ball hits the exit door. The answer will be considered correct, if its absolute or relative error does not exceed <span class="tex-span">10 <sup class="upper-index"> - 6</sup></span>.</p>





```input1
7 2 11
3 -11 2

```




```input2
7 2 11
4 -3 3

```




```output1
6.5000000000 2.0000000000

```




```output2
4.1666666667 1.0000000000

```



## Note

<p><img class="tex-graphics" src="file://gHVuf4Uz.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
