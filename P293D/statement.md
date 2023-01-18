## Description

<div><p>Ksusha is a vigorous mathematician. She is keen on absolutely incredible mathematical riddles. </p><p>Today Ksusha came across a convex polygon of non-zero area. She is now wondering: if she chooses a pair of distinct points uniformly among all integer points (points with integer coordinates) inside or on the border of the polygon and then draws a square with two opposite vertices lying in the chosen points, what will the expectation of this square's area be?</p><p>A pair of distinct points is chosen uniformly among all pairs of distinct points, located inside or on the border of the polygon. Pairs of points <span class="tex-span"><i>p</i>, <i>q</i></span> <span class="tex-span">(<i>p</i> ≠ <i>q</i>)</span> and <span class="tex-span"><i>q</i>, <i>p</i></span> are considered the same.</p><p>Help Ksusha! Count the required expectation.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of vertices of Ksusha's convex polygon. Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the polygon vertices in clockwise or counterclockwise order. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">6</sup>)</span> — the coordinates of the vertex that goes <span class="tex-span"><i>i</i></span>-th in that order.</p></div><div class="output-specification"><p>Print a single real number — the required expected area. </p><p>The answer will be considered correct if its absolute and relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of vertices of Ksusha's convex polygon. Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the polygon vertices in clockwise or counterclockwise order. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">6</sup>)</span> — the coordinates of the vertex that goes <span class="tex-span"><i>i</i></span>-th in that order.</p>

## Output

<p>Print a single real number — the required expected area. </p><p>The answer will be considered correct if its absolute and relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3
0 0
5 5
5 0

```




```input2
4
-1 3
4 5
6 2
3 -5

```




```input3
3
17 136
859 937
16 641

```




```output1
4.6666666667

```




```output2
8.1583333333

```




```output3
66811.3704155169

```


