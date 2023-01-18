## Description

<div><p>The whole world got obsessed with robots,and to keep pace with the progress, great Berland's programmer Draude decided to build his own robot. He was working hard at the robot. He taught it to walk the shortest path from one point to another, to record all its movements, but like in many Draude's programs, there was a bug — the robot didn't always walk the shortest path. Fortunately, the robot recorded its own movements correctly. Now Draude wants to find out when his robot functions wrong. Heh, if Draude only remembered the map of the field, where he tested the robot, he would easily say if the robot walked in the right direction or not. But the field map was lost never to be found, that's why he asks you to find out if there exist at least one map, where the path recorded by the robot is the shortest.</p><p>The map is an infinite checkered field, where each square is either empty, or contains an obstruction. It is also known that the robot never tries to run into the obstruction. By the recorded robot's movements find out if there exist at least one such map, that it is possible to choose for the robot a starting square (the starting square should be empty) such that when the robot moves from this square its movements coincide with the recorded ones (the robot doesn't run into anything, moving along empty squares only), and the path from the starting square to the end one is the shortest.</p><p>In one movement the robot can move into the square (providing there are no obstrutions in this square) that has common sides with the square the robot is currently in.</p></div><div class="input-specification"><p>The first line of the input file contains the recording of the robot's movements. This recording is a non-empty string, consisting of uppercase Latin letters <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">U</span> and <span class="tex-font-style-tt">D</span>, standing for movements left, right, up and down respectively. The length of the string does not exceed <span class="tex-font-style-tt">100</span>.</p></div><div class="output-specification"><p>In the first line output the only word <span class="tex-font-style-tt">OK</span> (if the above described map exists), or <span class="tex-font-style-tt">BUG</span> (if such a map does not exist).</p></div>

## Input

<p>The first line of the input file contains the recording of the robot's movements. This recording is a non-empty string, consisting of uppercase Latin letters <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">U</span> and <span class="tex-font-style-tt">D</span>, standing for movements left, right, up and down respectively. The length of the string does not exceed <span class="tex-font-style-tt">100</span>.</p>

## Output

<p>In the first line output the only word <span class="tex-font-style-tt">OK</span> (if the above described map exists), or <span class="tex-font-style-tt">BUG</span> (if such a map does not exist).</p>





```input1
LLUUUR

```




```input2
RRUULLDD

```




```output1
OK

```




```output2
BUG

```


