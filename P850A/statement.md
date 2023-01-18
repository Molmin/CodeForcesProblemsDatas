## Description

<div><p>You are given set of <span class="tex-span"><i>n</i></span> points in 5-dimensional space. The points are labeled from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. No two points coincide.</p><p>We will call point <span class="tex-span"><i>a</i></span> <span class="tex-font-style-it">bad</span> if there are different points <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>, not equal to <span class="tex-span"><i>a</i></span>, from the given set such that angle between vectors <img align="middle" class="tex-formula" src="file://2g5w9WUk.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://Pjuleh6u.png" style="max-width: 100.0%;max-height: 100.0%;"> is acute (i.e. strictly less than <img align="middle" class="tex-formula" src="file://kxmL0myZ.png" style="max-width: 100.0%;max-height: 100.0%;">). Otherwise, the point is called <span class="tex-font-style-it">good</span>.</p><p>The angle between vectors <img align="middle" class="tex-formula" src="file://rynfEKwZ.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://3GhO2cWQ.png" style="max-width: 100.0%;max-height: 100.0%;"> in 5-dimensional space is defined as <img align="middle" class="tex-formula" src="file://gNP07vAY.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://3Hub4mOn.png" style="max-width: 100.0%;max-height: 100.0%;"> is the scalar product and <img align="middle" class="tex-formula" src="file://bYTXlzTg.png" style="max-width: 100.0%;max-height: 100.0%;"> is length of <img align="middle" class="tex-formula" src="file://HXDbMl0r.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Given the list of points, print the indices of the good points in ascending order.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>)&nbsp;— the number of points.</p><p>The next <span class="tex-span"><i>n</i></span> lines of input contain five integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|, |<i>b</i><sub class="lower-index"><i>i</i></sub>|, |<i>c</i><sub class="lower-index"><i>i</i></sub>|, |<i>d</i><sub class="lower-index"><i>i</i></sub>|, |<i>e</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">3</sup></span>) &nbsp;— the coordinates of the i-th point. All points are distinct.</p></div><div class="output-specification"><p>First, print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of good points.</p><p>Then, print <span class="tex-span"><i>k</i></span> integers, each on their own line&nbsp;— the indices of the good points in ascending order.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>)&nbsp;— the number of points.</p><p>The next <span class="tex-span"><i>n</i></span> lines of input contain five integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|, |<i>b</i><sub class="lower-index"><i>i</i></sub>|, |<i>c</i><sub class="lower-index"><i>i</i></sub>|, |<i>d</i><sub class="lower-index"><i>i</i></sub>|, |<i>e</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">3</sup></span>) &nbsp;— the coordinates of the i-th point. All points are distinct.</p>

## Output

<p>First, print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of good points.</p><p>Then, print <span class="tex-span"><i>k</i></span> integers, each on their own line&nbsp;— the indices of the good points in ascending order.</p>





```input1
6
0 0 0 0 0
1 0 0 0 0
0 1 0 0 0
0 0 1 0 0
0 0 0 1 0
0 0 0 0 1

```




```input2
3
0 0 1 2 0
0 0 9 2 0
0 0 5 9 0

```




```output1
1
1

```




```output2
0

```



## Note

<p>In the first sample, the first point forms exactly a <img align="middle" class="tex-formula" src="file://p3dI5Tvx.png" style="max-width: 100.0%;max-height: 100.0%;"> angle with all other pairs of points, so it is good.</p><p>In the second sample, along the cd plane, we can see the points look as follows:</p><p><img class="tex-graphics" src="file://LIN0OqZI.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>We can see that all angles here are acute, so no points are good.</p>
