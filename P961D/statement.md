## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> points on Cartesian plane. Every point is a lattice point (i. e. both of its coordinates are integers), and all points are distinct.</p><p>You may draw two straight lines (not necessarily distinct). Is it possible to do this in such a way that every point lies on at least one of these lines?</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of points you are given.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line containing two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>— coordinates of <span class="tex-span"><i>i</i></span>-th point. All <span class="tex-span"><i>n</i></span> points are distinct.</p></div><div class="output-specification"><p>If it is possible to draw two straight lines in such a way that each of given points belongs to at least one of these lines, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of points you are given.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line containing two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span>— coordinates of <span class="tex-span"><i>i</i></span>-th point. All <span class="tex-span"><i>n</i></span> points are distinct.</p>

## Output

<p>If it is possible to draw two straight lines in such a way that each of given points belongs to at least one of these lines, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
5
0 0
0 1
1 1
1 -1
2 2

```




```input2
5
0 0
1 0
2 1
1 1
2 3

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first example it is possible to draw two lines, the one containing the points <span class="tex-span">1</span>, <span class="tex-span">3</span> and <span class="tex-span">5</span>, and another one containing two remaining points.</p><center> <img class="tex-graphics" src="file://jFfFxLq5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
