## Description

<div><p>Roland loves growing flowers. He has recently grown a beautiful rose at point <span class="tex-span">(0, 0)</span> of the Cartesian coordinate system. The rose is so beautiful that Roland is afraid that the evil forces can try and steal it. </p><p>To protect the rose, Roland wants to build <span class="tex-span"><i>n</i></span> watch towers. Let's assume that a tower is a point on the plane at the distance of at most <span class="tex-span"><i>r</i></span> from the rose. Besides, Roland assumes that the towers should be built at points with integer coordinates and the sum of squares of distances between all pairs of towers must be as large as possible. Note, that Roland may build several towers at the same point, also he may build some of them at point <span class="tex-span">(0, 0)</span>.</p><p>Help Roland build the towers at the integer points so that the sum of squares of distances between all towers is maximum possible. Note that the distance in this problem is defined as the Euclidian distance between points.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 8;&nbsp;1 ≤ <i>r</i> ≤ 30)</span>.</p></div><div class="output-specification"><p>In the first line print an integer — the maximum possible sum of squared distances. In the <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines print two integers, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th tower. Each tower must be inside or on the border of the circle with radius <span class="tex-span"><i>r</i></span>. Note that there may be several towers located at the same point of the plane, also some towers can be located at point <span class="tex-span">(0, 0)</span>.</p><p>If there are multiple valid optimal arrangements, choose any of them.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 8;&nbsp;1 ≤ <i>r</i> ≤ 30)</span>.</p>

## Output

<p>In the first line print an integer — the maximum possible sum of squared distances. In the <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines print two integers, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th tower. Each tower must be inside or on the border of the circle with radius <span class="tex-span"><i>r</i></span>. Note that there may be several towers located at the same point of the plane, also some towers can be located at point <span class="tex-span">(0, 0)</span>.</p><p>If there are multiple valid optimal arrangements, choose any of them.</p>





```input1
4 1

```




```input2
3 6

```




```output1
16
0 1
0 1
0 -1
0 -1

```




```output2
312
0 6
5 -3
-5 -3

```


