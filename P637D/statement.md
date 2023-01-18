## Description

<div><p>A sportsman starts from point <span class="tex-span"><i>x</i><sub class="lower-index"><i>start</i></sub> = 0</span> and runs to point with coordinate <span class="tex-span"><i>x</i><sub class="lower-index"><i>finish</i></sub> = <i>m</i></span> (on a straight line). Also, the sportsman can jump — to jump, he should first take a run of length of not less than <span class="tex-span"><i>s</i></span> meters (in this case for these <span class="tex-span"><i>s</i></span> meters his path should have no obstacles), and after that he can jump over a length of not more than <span class="tex-span"><i>d</i></span> meters. Running and jumping is permitted only in the direction from left to right. He can <span class="tex-font-style-bf">start</span> and<span class="tex-font-style-bf">finish</span> a jump only at the points with integer coordinates in which there are <span class="tex-font-style-bf">no obstacles</span>. To overcome some obstacle, it is necessary to land at a point which is strictly to the right of this obstacle.</p><p>On the way of an athlete are <span class="tex-span"><i>n</i></span> obstacles at coordinates <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. He cannot go over the obstacles, he can only jump over them. Your task is to determine whether the athlete will be able to get to the finish point.</p></div><div class="input-specification"><p>The first line of the input containsd four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>s</i>, <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of obstacles on the runner's way, the coordinate of the finishing point, the length of running before the jump and the maximum length of the jump, correspondingly.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i> - 1</span>)&nbsp;— the coordinates of the obstacles. It is guaranteed that the starting and finishing point have no obstacles, also no point can have more than one obstacle, The coordinates of the obstacles are given in an arbitrary order.</p></div><div class="output-specification"><p>If the runner cannot reach the finishing point, print in the first line of the output "<span class="tex-font-style-tt">IMPOSSIBLE</span>" (without the quotes).</p><p>If the athlete can get from start to finish, print any way to do this in the following format:</p><ul> <li> print a line of form "<span class="tex-font-style-tt">RUN X</span>&gt;" (where "<span class="tex-font-style-tt">X</span>" should be a positive integer), if the athlete should run for "<span class="tex-font-style-tt">X</span>" more meters; </li><li> print a line of form "<span class="tex-font-style-tt">JUMP Y</span>" (where "<span class="tex-font-style-tt">Y</span>" should be a positive integer), if the sportsman starts a jump and should remain in air for "<span class="tex-font-style-tt">Y</span>" more meters. </li></ul><p>All commands "<span class="tex-font-style-tt">RUN</span>" and "<span class="tex-font-style-tt">JUMP</span>" should strictly alternate, starting with "<span class="tex-font-style-tt">RUN</span>", besides, they should be printed chronologically. It is not allowed to jump over the finishing point but it is allowed to land there after a jump. The athlete should stop as soon as he reaches finish.</p></div>

## Input

<p>The first line of the input containsd four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">2 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>s</i>, <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of obstacles on the runner's way, the coordinate of the finishing point, the length of running before the jump and the maximum length of the jump, correspondingly.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i> - 1</span>)&nbsp;— the coordinates of the obstacles. It is guaranteed that the starting and finishing point have no obstacles, also no point can have more than one obstacle, The coordinates of the obstacles are given in an arbitrary order.</p>

## Output

<p>If the runner cannot reach the finishing point, print in the first line of the output "<span class="tex-font-style-tt">IMPOSSIBLE</span>" (without the quotes).</p><p>If the athlete can get from start to finish, print any way to do this in the following format:</p><ul> <li> print a line of form "<span class="tex-font-style-tt">RUN X</span>&gt;" (where "<span class="tex-font-style-tt">X</span>" should be a positive integer), if the athlete should run for "<span class="tex-font-style-tt">X</span>" more meters; </li><li> print a line of form "<span class="tex-font-style-tt">JUMP Y</span>" (where "<span class="tex-font-style-tt">Y</span>" should be a positive integer), if the sportsman starts a jump and should remain in air for "<span class="tex-font-style-tt">Y</span>" more meters. </li></ul><p>All commands "<span class="tex-font-style-tt">RUN</span>" and "<span class="tex-font-style-tt">JUMP</span>" should strictly alternate, starting with "<span class="tex-font-style-tt">RUN</span>", besides, they should be printed chronologically. It is not allowed to jump over the finishing point but it is allowed to land there after a jump. The athlete should stop as soon as he reaches finish.</p>





```input1
3 10 1 3
3 4 7

```




```input2
2 9 2 3
6 4

```




```output1
RUN 2
JUMP 3
RUN 1
JUMP 2
RUN 2

```




```output2
IMPOSSIBLE

```


