## Description

<div><p>Trouble came from the overseas lands: a three-headed dragon Gorynych arrived. The dragon settled at point <span class="tex-span"><i>C</i></span> and began to terrorize the residents of the surrounding villages.</p><p>A brave hero decided to put an end to the dragon. He moved from point <span class="tex-span"><i>A</i></span> to fight with Gorynych. The hero rode from point <span class="tex-span"><i>A</i></span> along a straight road and met point <span class="tex-span"><i>B</i></span> on his way. The hero knows that in this land for every pair of roads it is true that they are either parallel to each other, or lie on a straight line, or are perpendicular to each other. He also knows well that points <span class="tex-span"><i>B</i></span> and <span class="tex-span"><i>C</i></span> are connected by a road. So the hero must either turn 90 degrees to the left or continue riding straight ahead or turn 90 degrees to the right. But he forgot where the point <span class="tex-span"><i>C</i></span> is located.</p><p>Fortunately, a Brave Falcon flew right by. It can see all three points from the sky. The hero asked him what way to go to get to the dragon's lair.</p><p>If you have not got it, you are the falcon. Help the hero and tell him how to get him to point <span class="tex-span"><i>C</i></span>: turn left, go straight or turn right.</p><p>At this moment the hero is believed to stand at point <span class="tex-span"><i>B</i></span>, turning his back to point <span class="tex-span"><i>A</i></span>.</p></div><div class="input-specification"><p>The first input line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub>, <i>y</i><sub class="lower-index"><i>a</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>a</i></sub>|, |<i>y</i><sub class="lower-index"><i>a</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the coordinates of point <span class="tex-span"><i>A</i></span>. The second line contains the coordinates of point <span class="tex-span"><i>B</i></span> in the same form, the third line contains the coordinates of point <span class="tex-span"><i>C</i></span>.</p><p>It is guaranteed that all points are pairwise different. It is also guaranteed that either point <span class="tex-span"><i>B</i></span> lies on segment <span class="tex-span"><i>AC</i></span>, or angle <span class="tex-span"><i>ABC</i></span> is right.</p></div><div class="output-specification"><p>Print a single line. If a hero must turn left, print "LEFT" (without the quotes); If he must go straight ahead, print "TOWARDS" (without the quotes); if he should turn right, print "RIGHT" (without the quotes).</p></div>

## Input

<p>The first input line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub>, <i>y</i><sub class="lower-index"><i>a</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>a</i></sub>|, |<i>y</i><sub class="lower-index"><i>a</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> — the coordinates of point <span class="tex-span"><i>A</i></span>. The second line contains the coordinates of point <span class="tex-span"><i>B</i></span> in the same form, the third line contains the coordinates of point <span class="tex-span"><i>C</i></span>.</p><p>It is guaranteed that all points are pairwise different. It is also guaranteed that either point <span class="tex-span"><i>B</i></span> lies on segment <span class="tex-span"><i>AC</i></span>, or angle <span class="tex-span"><i>ABC</i></span> is right.</p>

## Output

<p>Print a single line. If a hero must turn left, print "LEFT" (without the quotes); If he must go straight ahead, print "TOWARDS" (without the quotes); if he should turn right, print "RIGHT" (without the quotes).</p>





```input1
0 0
0 1
1 1

```




```input2
-1 -1
-3 -3
-4 -4

```




```input3
-4 -6
-3 -7
-2 -6

```




```output1
RIGHT

```




```output2
TOWARDS

```




```output3
LEFT

```



## Note

<p>The picture to the first sample: </p><center><img class="tex-graphics" src="file://MCM6IzUW.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>The red color shows points A, B and C. The blue arrow shows the hero's direction. The green color shows the hero's trajectory.</p><p>The picture to the second sample: </p><center><img class="tex-graphics" src="file://FOSNvWTZ.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
