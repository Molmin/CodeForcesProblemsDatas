## Description

<div><p>Kevin Sun is ruminating on the origin of cows while standing at the origin of the Cartesian plane. He notices <span class="tex-span"><i>n</i></span> lines <img align="middle" class="tex-formula" src="file://kKBvTl0h.png" style="max-width: 100.0%;max-height: 100.0%;"> on the plane, each representable by an equation of the form <span class="tex-span"><i>ax</i> + <i>by</i> = <i>c</i></span>. He also observes that no two lines are parallel and that no three lines pass through the same point.</p><p>For each triple <span class="tex-span">(<i>i</i>, <i>j</i>, <i>k</i>)</span> such that <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> &lt; <i>k</i> ≤ <i>n</i></span>, Kevin considers the triangle formed by the three lines <img align="middle" class="tex-formula" src="file://3UCBTnir.png" style="max-width: 100.0%;max-height: 100.0%;"> . He calls a triangle <span class="tex-font-style-underline">original</span> if the circumcircle of that triangle passes through the origin. Since Kevin believes that the circles of bovine life are tied directly to such triangles, he wants to know the number of original triangles formed by unordered triples of distinct lines. </p><p>Recall that the <span class="tex-font-style-it">circumcircle</span> of a triangle is the circle which passes through all the vertices of that triangle.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 2000</span>), the number of lines.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe lines <img align="middle" class="tex-formula" src="file://6W6wGHr5.png" style="max-width: 100.0%;max-height: 100.0%;">. The <span class="tex-span"><i>i</i></span>-th of these lines contains three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|, |<i>b</i><sub class="lower-index"><i>i</i></sub>|, |<i>c</i><sub class="lower-index"><i>i</i></sub>| ≤ 10 000, <i>a</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> + <i>b</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> &gt; 0</span>), representing the equation <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><i>x</i> + <i>b</i><sub class="lower-index"><i>i</i></sub><i>y</i> = <i>c</i><sub class="lower-index"><i>i</i></sub></span> of line <img align="middle" class="tex-formula" src="file://mZ2w5Uwh.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>Print a single integer, the number of triples <span class="tex-span">(<i>i</i>, <i>j</i>, <i>k</i>)</span> with <span class="tex-span"><i>i</i> &lt; <i>j</i> &lt; <i>k</i></span> such that lines <img align="middle" class="tex-formula" src="file://GlEyucJj.png" style="max-width: 100.0%;max-height: 100.0%;"> form an original triangle.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 2000</span>), the number of lines.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe lines <img align="middle" class="tex-formula" src="file://6W6wGHr5.png" style="max-width: 100.0%;max-height: 100.0%;">. The <span class="tex-span"><i>i</i></span>-th of these lines contains three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>|, |<i>b</i><sub class="lower-index"><i>i</i></sub>|, |<i>c</i><sub class="lower-index"><i>i</i></sub>| ≤ 10 000, <i>a</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> + <i>b</i><sub class="lower-index"><i>i</i></sub><sup class="upper-index">2</sup> &gt; 0</span>), representing the equation <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub><i>x</i> + <i>b</i><sub class="lower-index"><i>i</i></sub><i>y</i> = <i>c</i><sub class="lower-index"><i>i</i></sub></span> of line <img align="middle" class="tex-formula" src="file://mZ2w5Uwh.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>Print a single integer, the number of triples <span class="tex-span">(<i>i</i>, <i>j</i>, <i>k</i>)</span> with <span class="tex-span"><i>i</i> &lt; <i>j</i> &lt; <i>k</i></span> such that lines <img align="middle" class="tex-formula" src="file://GlEyucJj.png" style="max-width: 100.0%;max-height: 100.0%;"> form an original triangle.</p>





```input1
4
1 0 0
0 1 0
1 1 -1
1 -1 2

```




```input2
3
0 1 1
1 1 2
1 -1 -2

```




```output1
2

```




```output2
1

```



## Note

<p>Note that in the first sample, some of the lines pass through the origin.</p><p>In the second sample, there is exactly one triple of lines: <span class="tex-span"><i>y</i> = 1, <i>x</i> + <i>y</i> = 2, <i>x</i> - <i>y</i> =  - 2.</span> The triangle they form has vertices <span class="tex-span">(0, 2), (1, 1), ( - 1, 1)</span>. The circumcircle of this triangle has equation <span class="tex-span"><i>x</i><sup class="upper-index">2</sup> + (<i>y</i> - 1)<sup class="upper-index">2</sup> = 1</span>. This indeed passes through <span class="tex-span">(0, 0).</span></p>
