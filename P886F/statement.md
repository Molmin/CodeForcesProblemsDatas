## Description

<div><p>You are given a set of <span class="tex-span"><i>n</i></span> points on the plane. A line containing the origin is called good, if projection of the given set to this line forms a symmetric multiset of points. Find the total number of good lines.</p><p>Multiset is a set where equal elements are allowed.</p><p>Multiset is called symmetric, if there is a point <span class="tex-span"><i>P</i></span> on the plane such that the multiset is <a href="https://en.wikipedia.org/wiki/Point_reflection">centrally symmetric</a> in respect of point <span class="tex-span"><i>P</i></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of points in the set.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup>  ≤  <i>x</i><sub class="lower-index"><i>i</i></sub>,  <i>y</i><sub class="lower-index"><i>i</i></sub>  ≤  10<sup class="upper-index">6</sup></span>) — the coordinates of the points. It is guaranteed that no two points coincide.</p></div><div class="output-specification"><p>If there are infinitely many good lines, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, print single integer&nbsp;— the number of good lines.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2000</span>) — the number of points in the set.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup>  ≤  <i>x</i><sub class="lower-index"><i>i</i></sub>,  <i>y</i><sub class="lower-index"><i>i</i></sub>  ≤  10<sup class="upper-index">6</sup></span>) — the coordinates of the points. It is guaranteed that no two points coincide.</p>

## Output

<p>If there are infinitely many good lines, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, print single integer&nbsp;— the number of good lines.</p>





```input1
3
1 2
2 1
3 3

```




```input2
2
4 3
1 2

```




```output1
3

```




```output2
-1

```



## Note

<p>Picture to the first sample test:</p><p><img class="tex-graphics" src="file://V3D9MQ7b.png" style="max-width: 100.0%;max-height: 100.0%;"> </p><p>In the second sample, any line containing the origin is good.</p>
