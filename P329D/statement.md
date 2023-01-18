## Description

<div><p><span class="tex-font-style-underline">Important: All possible tests are in the pretest, so you shouldn't hack on this problem. So, if you passed pretests, you will also pass the system test.</span></p><p>You are an adventurer currently journeying inside an evil temple. After defeating a couple of weak monsters, you arrived at a square room consisting of tiles forming an <span class="tex-span"><i>n</i> × <i>n</i></span> grid, surrounded entirely by walls. At the end of the room lies a door locked with evil magical forces. The following inscriptions are written on the door:</p><center> <span class="tex-font-style-underline">The sound of clashing rocks will awaken the door!</span> </center><p>Being a very senior adventurer, you immediately realize what this means. In the room next door lies an infinite number of magical rocks. There are four types of rocks: </p><ul> <li> '<span class="tex-font-style-tt">^</span>': this rock moves upwards; </li><li> '<span class="tex-font-style-tt">&lt;</span>': this rock moves leftwards; </li><li> '<span class="tex-font-style-tt">&gt;</span>': this rock moves rightwards; </li><li> '<span class="tex-font-style-tt">v</span>': this rock moves downwards. </li></ul><p>To open the door, you first need to place the rocks on some of the tiles (one tile can be occupied by at most one rock). Then, you select a single rock that you have placed and activate it. The activated rock will then move in its direction until it hits another rock or hits the walls of the room (the rock will not move if something already blocks it in its chosen direction). The rock then deactivates. If it hits the walls, or if there have been already <span class="tex-span">10<sup class="upper-index">7</sup></span> events of rock becoming activated, the movements end. Otherwise, the rock that was hit becomes activated and this procedure is repeated.</p><p>If a rock moves at least one cell before hitting either the wall or another rock, the hit produces a sound. The door will open once the number of produced sounds is at least <span class="tex-span"><i>x</i></span>. It is okay for the rocks to continue moving after producing <span class="tex-span"><i>x</i></span> sounds.</p><p>The following picture illustrates the four possible scenarios of moving rocks.</p><ul><li> Moves at least one cell, then hits another rock. A sound is produced, the hit rock becomes activated.<center> <img class="tex-graphics" src="file://Mzj5GWV2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></li><li> Moves at least one cell, then hits the wall (i.e., the side of the room). A sound is produced, the movements end.<center> <img class="tex-graphics" src="file://3dGeHvGs.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></li><li> Does not move because a rock is already standing in the path. The blocking rock becomes activated, but no sounds are produced.<center> <img class="tex-graphics" src="file://C3jkivyx.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></li><li> Does not move because the wall is in the way. No sounds are produced and the movements end.<center> <img class="tex-graphics" src="file://2HmDdRji.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></li></ul><p>Assume there's an infinite number of rocks of each type in the neighboring room. You know what to do: place the rocks and open the door!</p></div><div class="input-specification"><p>The first line will consists of two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span>, denoting the size of the room and the number of sounds required to open the door. There will be exactly three test cases for this problem:</p><ul> <li> <span class="tex-span"><i>n</i> = 5, <i>x</i> = 5</span>; </li><li> <span class="tex-span"><i>n</i> = 3, <i>x</i> = 2</span>; </li><li> <span class="tex-span"><i>n</i> = 100, <i>x</i> = 10<sup class="upper-index">5</sup></span>. </li></ul><p>All of these testcases are in pretest.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> lines. Each line consists of <span class="tex-span"><i>n</i></span> characters — the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line represents the content of the tile at the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column, and should be one of these:</p><ul> <li> '<span class="tex-font-style-tt">^</span>', '<span class="tex-font-style-tt">&lt;</span>', '<span class="tex-font-style-tt">&gt;</span>', or '<span class="tex-font-style-tt">v</span>': a rock as described in the problem statement. </li><li> '<span class="tex-font-style-tt">.</span>': an empty tile. </li></ul><p>Then, output two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>r</i>, <i>c</i> ≤ <i>n</i></span>) on the next line — this means that the rock you activate first is located at the <span class="tex-span"><i>r</i></span>-th row from above and <span class="tex-span"><i>c</i></span>-th column from the left. There must be a rock in this cell.</p><p>If there are multiple solutions, you may output any of them.</p></div>

## Input

<p>The first line will consists of two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span>, denoting the size of the room and the number of sounds required to open the door. There will be exactly three test cases for this problem:</p><ul> <li> <span class="tex-span"><i>n</i> = 5, <i>x</i> = 5</span>; </li><li> <span class="tex-span"><i>n</i> = 3, <i>x</i> = 2</span>; </li><li> <span class="tex-span"><i>n</i> = 100, <i>x</i> = 10<sup class="upper-index">5</sup></span>. </li></ul><p>All of these testcases are in pretest.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> lines. Each line consists of <span class="tex-span"><i>n</i></span> characters — the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line represents the content of the tile at the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column, and should be one of these:</p><ul> <li> '<span class="tex-font-style-tt">^</span>', '<span class="tex-font-style-tt">&lt;</span>', '<span class="tex-font-style-tt">&gt;</span>', or '<span class="tex-font-style-tt">v</span>': a rock as described in the problem statement. </li><li> '<span class="tex-font-style-tt">.</span>': an empty tile. </li></ul><p>Then, output two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>r</i>, <i>c</i> ≤ <i>n</i></span>) on the next line — this means that the rock you activate first is located at the <span class="tex-span"><i>r</i></span>-th row from above and <span class="tex-span"><i>c</i></span>-th column from the left. There must be a rock in this cell.</p><p>If there are multiple solutions, you may output any of them.</p>





```input1
5 5

```




```input2
3 2

```




```output1
&gt;...v
v.&lt;..
..^..
&gt;....
..^.&lt;
1 1

```




```output2
&gt;vv
^&lt;.
^.&lt;
1 3

```



## Note

<p>Here's a simulation of the first example, accompanied with the number of sounds produced so far.</p><center> <img class="tex-graphics" src="file://UqxuYCEx.png" style="max-width: 100.0%;max-height: 100.0%;"> 0 sound </center><center> <img class="tex-graphics" src="file://pEGMWoWE.png" style="max-width: 100.0%;max-height: 100.0%;"> 1 sound </center><center> <img class="tex-graphics" src="file://3ibVyWbT.png" style="max-width: 100.0%;max-height: 100.0%;"> 2 sounds </center><center> <img class="tex-graphics" src="file://Rf98AxGC.png" style="max-width: 100.0%;max-height: 100.0%;"> 3 sounds </center><center> <img class="tex-graphics" src="file://kOTgyt7s.png" style="max-width: 100.0%;max-height: 100.0%;"> 4 sounds </center><center> <img class="tex-graphics" src="file://21P4uYwG.png" style="max-width: 100.0%;max-height: 100.0%;"> still 4 sounds </center><p>In the picture above, the activated rock switches between the '<span class="tex-font-style-tt">^</span>' rock and the '<span class="tex-font-style-tt">&lt;</span>' rock. However, no sound is produced since the '<span class="tex-font-style-tt">^</span>' rock didn't move even a single tile. So, still 4 sound.</p><center> <img class="tex-graphics" src="file://z57MjXUD.png" style="max-width: 100.0%;max-height: 100.0%;"> 5 sounds </center><p>At this point, 5 sound are already produced, so this solution is already correct. However, for the sake of example, we will continue simulating what happens.</p><center> <img class="tex-graphics" src="file://3xBa8jZw.png" style="max-width: 100.0%;max-height: 100.0%;"> 6 sounds </center><center> <img class="tex-graphics" src="file://1KqDLUWR.png" style="max-width: 100.0%;max-height: 100.0%;"> 7 sounds </center><center> <img class="tex-graphics" src="file://NrQ06TtJ.png" style="max-width: 100.0%;max-height: 100.0%;"> still 7 sounds </center><center> <img class="tex-graphics" src="file://wcWAdNkn.png" style="max-width: 100.0%;max-height: 100.0%;"> 8 sounds </center><p>And the movement stops. In total, it produces 8 sounds. Notice that the last move produced sound.</p><p>Here's a simulation of the second example:</p><center> <img class="tex-graphics" src="file://XpJsLcYS.png" style="max-width: 100.0%;max-height: 100.0%;"> 0 sound </center><center> <img class="tex-graphics" src="file://iiMo5iqJ.png" style="max-width: 100.0%;max-height: 100.0%;"> 1 sound </center><center> <img class="tex-graphics" src="file://vw5Dhqm2.png" style="max-width: 100.0%;max-height: 100.0%;"> 2 sounds </center><p>Now, the activated stone will switch continuously from one to another without producing a sound until it reaches the <span class="tex-span">10<sup class="upper-index">7</sup></span> limit, after which the movement will cease.</p><center> <img class="tex-graphics" src="file://MauZqy8N.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In total, it produced exactly 2 sounds, so the solution is correct.</p>
