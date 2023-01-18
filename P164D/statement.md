## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> points on the plane. You need to delete exactly <span class="tex-span"><i>k</i></span> of them <span class="tex-span">(<i>k</i> &lt; <i>n</i>)</span> so that the diameter of the set of the remaining <span class="tex-span"><i>n</i> - <i>k</i></span> points were as small as possible. The diameter of a set of points is the maximum pairwise distance between the points of the set. The diameter of a one point set equals zero.</p></div><div class="input-specification"><p>The first input line contains a pair of integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 30</span>, <span class="tex-span"><i>k</i> &lt; <i>n</i></span>) — the numbers of points on the plane and the number of points to delete, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the points, one per line. Each description consists of a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 32000</span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th point. The given points can coincide.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> different space-separated integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — the numbers of points to delete. The points are numbered in the order, in which they are given in the input from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. You can print the numbers in any order. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first input line contains a pair of integers <span class="tex-span"><i>n</i>, <i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 30</span>, <span class="tex-span"><i>k</i> &lt; <i>n</i></span>) — the numbers of points on the plane and the number of points to delete, correspondingly.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the points, one per line. Each description consists of a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 32000</span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th point. The given points can coincide.</p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> different space-separated integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — the numbers of points to delete. The points are numbered in the order, in which they are given in the input from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. You can print the numbers in any order. If there are multiple solutions, print any of them.</p>





```input1
5 2
1 2
0 0
2 2
1 1
3 3

```




```input2
4 1
0 0
0 0
1 1
1 1

```




```output1
5 2
```




```output2
3
```


