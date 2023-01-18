## Description

<div><p>Gerald got tired of playing board games with the usual six-sided die, and he bought a toy called Randomizer. It functions as follows.</p><p>A Randomizer has its own coordinate plane on which a strictly convex polygon is painted, the polygon is called a <span class="tex-font-style-bf">basic polygon</span>. If you shake a Randomizer, it draws some nondegenerate (i.e. having a non-zero area) convex polygon with vertices at some vertices of the <span class="tex-font-style-bf">basic polygon</span>. The result of the roll (more precisely, the result of the shaking) is considered to be the number of points with integer coordinates, which were strictly inside (the points on the border are not considered) the selected polygon. Now Gerald is wondering: what is the expected result of shaking the Randomizer?</p><p>During the shaking the Randomizer considers all the possible non-degenerate convex polygons with vertices at the vertices of the <span class="tex-font-style-bf">basic polygon</span>. Let's assume that there are <span class="tex-span"><i>k</i></span> versions of the polygons. Then the Randomizer chooses each of them with probability <img align="middle" class="tex-formula" src="file://eNrH1SEA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000</span>) — the number of vertices of the basic polygon. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the vertices of the basic polygon. The <span class="tex-span"><i>i</i></span>-th of these lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex of the polygon. The vertices are given in the counter-clockwise order.</p></div><div class="output-specification"><p>Print the sought expected value with absolute or relative error at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000</span>) — the number of vertices of the basic polygon. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the vertices of the basic polygon. The <span class="tex-span"><i>i</i></span>-th of these lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex of the polygon. The vertices are given in the counter-clockwise order.</p>

## Output

<p>Print the sought expected value with absolute or relative error at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
4
0 0
2 0
2 2
0 2

```




```input2
5
0 0
2 0
2 2
1 3
0 2

```




```output1
0.2

```




```output2
0.8125

```



## Note

<p>A polygon is called strictly convex if it is convex and no its vertices lie on the same line.</p><p>Let's assume that a random variable takes values <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> with probabilities <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>, correspondingly. Then the expected value of this variable equals to <img align="middle" class="tex-formula" src="file://GEmHUvLI.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
