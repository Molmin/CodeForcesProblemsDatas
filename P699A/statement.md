## Description

<div><p>There will be a launch of a new, powerful and unusual collider very soon, which located along a straight line. <span class="tex-span"><i>n</i></span> particles will be launched inside it. All of them are located in a straight line and there can not be two or more particles located in the same point. The coordinates of the particles coincide with the distance in meters from the center of the collider, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the coordinate of the <span class="tex-span"><i>i</i></span>-th particle and its position in the collider at the same time. All coordinates of particle positions are <span class="tex-font-style-bf">even integers</span>.</p><p>You know the direction of each particle movement&nbsp;— it will move to the right or to the left after the collider's launch start. All particles begin to move simultaneously at the time of the collider's launch start. Each particle will move straight to the left or straight to the right with the constant speed of <span class="tex-span">1</span> meter per microsecond. The collider is big enough so particles can not leave it in the foreseeable time.</p><p>Write the program which finds the moment of the first collision of any two particles of the collider. In other words, find the number of microseconds before the first moment when any two particles are at the same point.</p></div><div class="input-specification"><p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of particles. </p><p>The second line contains <span class="tex-span"><i>n</i></span> symbols "<span class="tex-font-style-tt">L</span>" and "<span class="tex-font-style-tt">R</span>". If the <span class="tex-span"><i>i</i></span>-th symbol equals "<span class="tex-font-style-tt">L</span>", then the <span class="tex-span"><i>i</i></span>-th particle will move to the left, otherwise the <span class="tex-span"><i>i</i></span>-th symbol equals "<span class="tex-font-style-tt">R</span>" and the <span class="tex-span"><i>i</i></span>-th particle will move to the right.</p><p>The third line contains the sequence of pairwise distinct <span class="tex-font-style-bf">even</span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of particles in the order from the left to the right. It is guaranteed that the coordinates of particles are given in the increasing order. </p></div><div class="output-specification"><p>In the first line print the only integer&nbsp;— the first moment (in microseconds) when two particles are at the same point and there will be an explosion. </p><p>Print the only integer <span class="tex-font-style-tt">-1</span>, if the collision of particles doesn't happen. </p></div>

## Input

<p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of particles. </p><p>The second line contains <span class="tex-span"><i>n</i></span> symbols "<span class="tex-font-style-tt">L</span>" and "<span class="tex-font-style-tt">R</span>". If the <span class="tex-span"><i>i</i></span>-th symbol equals "<span class="tex-font-style-tt">L</span>", then the <span class="tex-span"><i>i</i></span>-th particle will move to the left, otherwise the <span class="tex-span"><i>i</i></span>-th symbol equals "<span class="tex-font-style-tt">R</span>" and the <span class="tex-span"><i>i</i></span>-th particle will move to the right.</p><p>The third line contains the sequence of pairwise distinct <span class="tex-font-style-bf">even</span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of particles in the order from the left to the right. It is guaranteed that the coordinates of particles are given in the increasing order. </p>

## Output

<p>In the first line print the only integer&nbsp;— the first moment (in microseconds) when two particles are at the same point and there will be an explosion. </p><p>Print the only integer <span class="tex-font-style-tt">-1</span>, if the collision of particles doesn't happen. </p>





```input1
4
RLRL
2 4 6 10

```




```input2
3
LLR
40 50 60

```




```output1
1

```




```output2
-1

```



## Note

<p>In the first sample case the first explosion will happen in <span class="tex-span">1</span> microsecond because the particles number <span class="tex-span">1</span> and <span class="tex-span">2</span> will simultaneously be at the same point with the coordinate <span class="tex-span">3</span>. </p><p>In the second sample case there will be no explosion because there are no particles which will simultaneously be at the same point.</p>
