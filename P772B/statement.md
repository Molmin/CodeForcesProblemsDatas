## Description

<div><p>You are given a convex polygon <span class="tex-span"><i>P</i></span> with <span class="tex-span"><i>n</i></span> distinct vertices <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>. Vertex <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> has coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> in the 2D plane. These vertices are listed in clockwise order.</p><p>You can choose a real number <span class="tex-span"><i>D</i></span> and move each vertex of the polygon a distance of at most <span class="tex-span"><i>D</i></span> from their original positions.</p><p>Find the maximum value of <span class="tex-span"><i>D</i></span> such that no matter how you move the vertices, the polygon does not intersect itself and stays convex.</p></div><div class="input-specification"><p>The first line has one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 1 000</span>)&nbsp;— the number of vertices.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the vertices. Line <span class="tex-span"><i>i</i></span> contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex. These points are guaranteed to be given in clockwise order, and will form a strictly convex polygon (in particular, no three consecutive points lie on the same straight line).</p></div><div class="output-specification"><p>Print one real number <span class="tex-span"><i>D</i></span>, which is the maximum real number such that no matter how you move the vertices, the polygon stays convex.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely, let's assume that your answer is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://BgGJ2ouB.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line has one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 1 000</span>)&nbsp;— the number of vertices.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the vertices. Line <span class="tex-span"><i>i</i></span> contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex. These points are guaranteed to be given in clockwise order, and will form a strictly convex polygon (in particular, no three consecutive points lie on the same straight line).</p>

## Output

<p>Print one real number <span class="tex-span"><i>D</i></span>, which is the maximum real number such that no matter how you move the vertices, the polygon stays convex.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely, let's assume that your answer is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://BgGJ2ouB.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4
0 0
0 1
1 1
1 0

```




```input2
6
5 0
10 0
12 -4
10 -8
5 -8
3 -4

```




```output1
0.3535533906

```




```output2
1.0000000000

```



## Note

<p>Here is a picture of the first sample</p><p><img class="tex-graphics" src="file://SFsS3pFZ.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Here is an example of making the polygon non-convex.</p><p><img class="tex-graphics" src="file://lXtFdEjD.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>This is not an optimal solution, since the maximum distance we moved one point is <span class="tex-span"> ≈ 0.4242640687</span>, whereas we can make it non-convex by only moving each point a distance of at most <span class="tex-span"> ≈ 0.3535533906</span>.</p>
