## Description

<div><p>You are given a circular maze such as the ones shown in the figures. </p><center> <img class="tex-graphics" src="file://RNea2G6h.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center> Determine if it can be solved, i.e., if there is a path which goes from the center to the outside of the maze which does not touch any wall. The maze is described by $n$ walls. Each wall can be either circular or straight. <ul> <li> Circular walls are described by a radius $r$, the distance from the center, and two angles $\theta_1, \theta_2$ describing the beginning and the end of the wall in the clockwise direction. Notice that swapping the two angles changes the wall. </li><li> Straight walls are described by an angle $\theta$, the direction of the wall, and two radii $r_1 &lt; r_2$ describing the beginning and the end of the wall. </li></ul><p>Angles are measured in degrees; the angle $0$ corresponds to the upward pointing direction; and angles increase clockwise (hence the east direction corresponds to the angle $90$).</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 20$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 5000$) — the number of walls. </p><p>Each of the following $n$ lines each contains a character (<span class="tex-font-style-tt">C</span> for circular, and <span class="tex-font-style-tt">S</span> for straight) and three integers: </p><ul> <li> either $r, \theta_1, \theta_2$ ($1 \leq r \leq 20$ and $0 \leq \theta_1,\theta_2 &lt; 360$ with $\theta_1 \neq \theta_2$) if the wall is circular, </li><li> or $r_1$, $r_2$ and $\theta$ ($1 \leq r_1 &lt; r_2 \leq 20$ and $0 \leq \theta &lt; 360$) if the wall is straight. </li></ul><p>It is guaranteed that circular walls do not overlap (but two circular walls may intersect at one or two points), and that straight walls do not overlap (but two straight walls may intersect at one point). However, circular and straight walls can intersect arbitrarily.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if the maze can be solved and <span class="tex-font-style-tt">NO</span> otherwise. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 20$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 5000$) — the number of walls. </p><p>Each of the following $n$ lines each contains a character (<span class="tex-font-style-tt">C</span> for circular, and <span class="tex-font-style-tt">S</span> for straight) and three integers: </p><ul> <li> either $r, \theta_1, \theta_2$ ($1 \leq r \leq 20$ and $0 \leq \theta_1,\theta_2 &lt; 360$ with $\theta_1 \neq \theta_2$) if the wall is circular, </li><li> or $r_1$, $r_2$ and $\theta$ ($1 \leq r_1 &lt; r_2 \leq 20$ and $0 \leq \theta &lt; 360$) if the wall is straight. </li></ul><p>It is guaranteed that circular walls do not overlap (but two circular walls may intersect at one or two points), and that straight walls do not overlap (but two straight walls may intersect at one point). However, circular and straight walls can intersect arbitrarily.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if the maze can be solved and <span class="tex-font-style-tt">NO</span> otherwise. </p>





```input1
2
5
C 1 180 90
C 5 250 230
C 10 150 140
C 20 185 180
S 1 20 180
6
C 1 180 90
C 5 250 230
C 10 150 140
C 20 185 180
S 1 20 180
S 5 10 0
```




```output1
YES
NO
```



## Note

<p>The two sample test cases correspond to the two mazes in the picture.</p>
