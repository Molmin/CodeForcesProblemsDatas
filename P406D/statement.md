## Description

<div><p>This problem has nothing to do with Little Chris. It is about hill climbers instead (and Chris definitely isn't one).</p><p>There are <span class="tex-span"><i>n</i></span> hills arranged on a line, each in the form of a vertical line segment with one endpoint on the ground. The hills are numbered with numbers from 1 to <span class="tex-span"><i>n</i></span> from left to right. The <span class="tex-span"><i>i</i></span>-th hill stands at position <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> with its top at height <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>. For every two hills <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, if the top of hill <span class="tex-span"><i>a</i></span> can be seen from the top of hill <span class="tex-span"><i>b</i></span>, their tops are connected by a rope. Formally, the tops of two hills are connected if the segment connecting their top points does not intersect or touch any of the other hill segments. Using these ropes, the hill climbers can move from hill to hill.</p><p>There are <span class="tex-span"><i>m</i></span> teams of climbers, each composed of exactly two members. The first and the second climbers of the <span class="tex-span"><i>i</i></span>-th team are located at the top of the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th hills, respectively. They want to meet together at the top of some hill. Now, each of two climbers move according to the following process:</p><ol> <li> if a climber is at the top of the hill where the other climber is already located or will come eventually, the former climber stays at this hill; </li><li> otherwise, the climber picks a hill to the right of his current hill that is reachable by a rope and <span class="tex-font-style-bf">is the rightmost possible</span>, climbs this hill and continues the process (the climber can also climb a hill whose top is lower than the top of his current hill). </li></ol><center> <img class="tex-graphics" src="file://k4tL9HO0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For each team of climbers, determine the number of the meeting hill for this pair!</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of hills. The next <span class="tex-span"><i>n</i></span> lines describe the hills. The <span class="tex-span"><i>i</i></span>-th of them contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>; <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">11</sup></span>), the position and the height of the <span class="tex-span"><i>i</i></span>-th hill. The hills are given in the ascending order of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, i.e., <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>j</i></sub></span> for <span class="tex-span"><i>i</i> &lt; <i>j</i></span>.</p><p>The next line of input contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of teams. The next <span class="tex-span"><i>m</i></span> lines describe the teams. The <span class="tex-span"><i>i</i></span>-th of them contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the numbers of the hills where the climbers of the <span class="tex-span"><i>i</i></span>-th team are located. It is possible that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>In a single line output <span class="tex-span"><i>m</i></span> space-separated integers, where the <span class="tex-span"><i>i</i></span>-th integer is the number of the meeting hill for the members of the <span class="tex-span"><i>i</i></span>-th team.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of hills. The next <span class="tex-span"><i>n</i></span> lines describe the hills. The <span class="tex-span"><i>i</i></span>-th of them contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>; <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">11</sup></span>), the position and the height of the <span class="tex-span"><i>i</i></span>-th hill. The hills are given in the ascending order of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, i.e., <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>j</i></sub></span> for <span class="tex-span"><i>i</i> &lt; <i>j</i></span>.</p><p>The next line of input contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of teams. The next <span class="tex-span"><i>m</i></span> lines describe the teams. The <span class="tex-span"><i>i</i></span>-th of them contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the numbers of the hills where the climbers of the <span class="tex-span"><i>i</i></span>-th team are located. It is possible that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>In a single line output <span class="tex-span"><i>m</i></span> space-separated integers, where the <span class="tex-span"><i>i</i></span>-th integer is the number of the meeting hill for the members of the <span class="tex-span"><i>i</i></span>-th team.</p>





```input1
6
1 4
2 1
3 2
4 3
6 4
7 4
3
3 1
5 6
2 3

```




```output1
5 6 3 

```


