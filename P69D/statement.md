## Description

<div><p>Anton and Dasha like to play different games during breaks on checkered paper. By the 11th grade they managed to play all the games of this type and asked Vova the programmer to come up with a new game. Vova suggested to them to play a game under the code name "dot" with the following rules: </p><ul><li> On the checkered paper a coordinate system is drawn. A dot is initially put in the position <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. </li><li> A move is shifting a dot to one of the pre-selected vectors. Also each player can once per game symmetrically reflect a dot relatively to the line <span class="tex-span"><i>y</i> = <i>x</i></span>. </li><li> Anton and Dasha take turns. Anton goes first. </li><li> The player after whose move the distance from the dot to the coordinates' origin exceeds <span class="tex-span"><i>d</i></span>, loses. </li></ul><p>Help them to determine the winner.</p></div><div class="input-specification"><p>The first line of the input file contains 4 integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span"> - 200 ≤ <i>x</i>, <i>y</i> ≤ 200, 1 ≤ <i>d</i> ≤ 200, 1 ≤ <i>n</i> ≤ 20</span>) — the initial coordinates of the dot, the distance <span class="tex-span"><i>d</i></span> and the number of vectors. It is guaranteed that the initial dot is at the distance less than <span class="tex-span"><i>d</i></span> from the origin of the coordinates. The following <span class="tex-span"><i>n</i></span> lines each contain two non-negative numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>) — the coordinates of the i-th vector. It is guaranteed that all the vectors are nonzero and different.</p></div><div class="output-specification"><p>You should print "<span class="tex-font-style-tt">Anton</span>", if the winner is Anton in case of both players play the game optimally, and "<span class="tex-font-style-tt">Dasha</span>" otherwise.</p></div>

## Input

<p>The first line of the input file contains 4 integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span"> - 200 ≤ <i>x</i>, <i>y</i> ≤ 200, 1 ≤ <i>d</i> ≤ 200, 1 ≤ <i>n</i> ≤ 20</span>) — the initial coordinates of the dot, the distance <span class="tex-span"><i>d</i></span> and the number of vectors. It is guaranteed that the initial dot is at the distance less than <span class="tex-span"><i>d</i></span> from the origin of the coordinates. The following <span class="tex-span"><i>n</i></span> lines each contain two non-negative numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>) — the coordinates of the i-th vector. It is guaranteed that all the vectors are nonzero and different.</p>

## Output

<p>You should print "<span class="tex-font-style-tt">Anton</span>", if the winner is Anton in case of both players play the game optimally, and "<span class="tex-font-style-tt">Dasha</span>" otherwise.</p>





```input1
0 0 2 3
1 1
1 2

```




```input2
0 0 2 4
1 1
1 2

```




```output1
Anton
```




```output2
Dasha
```



## Note

<p>In the first test, Anton goes to the vector (1;2), and Dasha loses. In the second test Dasha with her first move shifts the dot so that its coordinates are (2;3), and Anton loses, as he has the only possible move — to reflect relatively to the line <span class="tex-span"><i>y</i> = <i>x</i></span>. Dasha will respond to it with the same move and return the dot in position (2;3).</p>
