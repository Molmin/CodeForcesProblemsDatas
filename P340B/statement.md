## Description

<div><p>Iahub has drawn a set of <span class="tex-span"><i>n</i></span> points in the cartesian plane which he calls "special points". A quadrilateral is a simple polygon without self-intersections with four sides (also called edges) and four vertices (also called corners). Please note that a quadrilateral doesn't have to be convex. A special quadrilateral is one which has all four vertices in the set of special points. Given the set of special points, please calculate the maximal area of a special quadrilateral. </p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 300</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the cartesian coordinates of <span class="tex-span"><i>i</i></span>th special point. It is guaranteed that no three points are on the same line. It is guaranteed that no two points coincide. </p></div><div class="output-specification"><p>Output a single real number — the maximal area of a special quadrilateral. The answer will be considered correct if its absolute or relative error does't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 300</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers: <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the cartesian coordinates of <span class="tex-span"><i>i</i></span>th special point. It is guaranteed that no three points are on the same line. It is guaranteed that no two points coincide. </p>

## Output

<p>Output a single real number — the maximal area of a special quadrilateral. The answer will be considered correct if its absolute or relative error does't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
5
0 0
0 4
4 0
4 4
2 3

```




```output1
16.000000
```



## Note

<p>In the test example we can choose first <span class="tex-span">4</span> points to be the vertices of the quadrilateral. They form a square by side <span class="tex-span">4</span>, so the area is <span class="tex-span">4·4 = 16</span>.</p>
