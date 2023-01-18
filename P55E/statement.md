## Description

<div><p>You are given a convex polygon. Count, please, the number of triangles that contain a given point in the plane and their vertices are the vertices of the polygon. It is guaranteed, that the point doesn't lie on the sides and the diagonals of the polygon.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of vertices of the polygon (<span class="tex-span">3 ≤ <i>n</i> ≤ 100000</span>). The polygon description is following: <span class="tex-span"><i>n</i></span> lines containing coordinates of the vertices in clockwise order (integer <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> not greater than <span class="tex-span">10<sup class="upper-index">9</sup></span> by absolute value). It is guaranteed that the given polygon is nondegenerate and convex (no three points lie on the same line).</p><p>The next line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 20</span>) — the number of points which you should count the answer for. It is followed by <span class="tex-span"><i>t</i></span> lines with coordinates of the points (integer <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> not greater than <span class="tex-span">10<sup class="upper-index">9</sup></span> by absolute value).</p></div><div class="output-specification"><p>The output should contain <span class="tex-span"><i>t</i></span> integer numbers, each on a separate line, where <span class="tex-span"><i>i</i></span>-th number is the answer for the <span class="tex-span"><i>i</i></span>-th point.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cin</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of vertices of the polygon (<span class="tex-span">3 ≤ <i>n</i> ≤ 100000</span>). The polygon description is following: <span class="tex-span"><i>n</i></span> lines containing coordinates of the vertices in clockwise order (integer <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> not greater than <span class="tex-span">10<sup class="upper-index">9</sup></span> by absolute value). It is guaranteed that the given polygon is nondegenerate and convex (no three points lie on the same line).</p><p>The next line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 20</span>) — the number of points which you should count the answer for. It is followed by <span class="tex-span"><i>t</i></span> lines with coordinates of the points (integer <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> not greater than <span class="tex-span">10<sup class="upper-index">9</sup></span> by absolute value).</p>

## Output

<p>The output should contain <span class="tex-span"><i>t</i></span> integer numbers, each on a separate line, where <span class="tex-span"><i>i</i></span>-th number is the answer for the <span class="tex-span"><i>i</i></span>-th point.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cin</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
4
5 0
0 0
0 5
5 5
1
1 3

```




```input2
3
0 0
0 5
5 0
2
1 1
10 10

```




```input3
5
7 6
6 3
4 1
1 2
2 4
4
3 3
2 3
5 5
4 2

```




```output1
2

```




```output2
1
0

```




```output3
5
3
3
4

```


